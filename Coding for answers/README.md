# Cisco Data Science Essentials — Module 3
Practical Python labs & projects for "Coding for answers"  
This folder contains the notebooks and scripts used to complete Module 3 of the Cisco Data Science Essentials program: hands‑on exercises that apply Python (Pandas, Matplotlib, NumPy and friends) to real, data‑driven problems.

[View folder on GitHub](https://github.com/BhavikBuchke/Cisco-Data-science-program/tree/main/Coding%20for%20answers)

---

Table of contents
- About
- Projects (index + short descriptions)
- Quick start (run locally)
- Recommended environment & dependencies
- How to run the notebooks (dev & CI-friendly)
- Project expectations & assessment checklist
- Tips & common pitfalls
- Datasets & attribution
- Contributing
- License & contact

About
-----
This collection is the Module 3 "Coding for answers" workbook for the Cisco Data Science Essentials course. The emphasis is on:
- reading and cleaning tabular and semi-structured data with Pandas
- exploratory data analysis and visualization (Matplotlib, Seaborn)
- basic geospatial and image/colour analyses where required
- producing reproducible Jupyter notebooks and small scripts suitable for assessment

The exercises encourage reproducible workflows, clear explanations (text + visuals) and code that could be graded or re-run by anyone.

Projects (index)
----------------
The folder contains notebooks and scripts for the projects below. Each entry has a suggested short objective and expected deliverables (notebook/script, short write-up, visual outputs).

1. First day week
   - Objective: onboarding exercises to verify environment, quick Python/Pandas warmups.
   - Deliverables: `first_day_week.ipynb` — basic EDA and demo plots.

2. Skeletal variation
   - Objective: analyze biological/measurement data (statistical summaries, hypothesis checks, plotting distributions).
   - Deliverables: `skeletal_variation.ipynb` — data cleaning, group comparisons, summary tables, histograms/boxplots.

3. Our Connected World
   - Objective: work with geographic or network datasets (mapping points/regions, simple spatial joins or plotting connectivity).
   - Deliverables: `our_connected_world.ipynb` — maps (Matplotlib/GeoPandas/folium), data aggregation by region, short insight summary.

4. Jeans pockets
   - Objective: a small data parsing/ETL challenge (text parsing, pattern matching, or image/dataset inspection).
   - Deliverables: `jeans_pockets.ipynb` or `jeans_pockets.py` — parsed dataset, summary stats, sample visualizations.

5. Largest island
   - Objective: algorithmic grid/graph task (find largest connected component on a grid; flood fill / BFS/DFS).
   - Deliverables: `largest_island.ipynb` — implementation, complexity notes, visual examples.

6. Mondrian art
   - Objective: treat artworks as data (color region detection, composition analysis, recreate Mondrian-like layouts).
   - Deliverables: `mondrian_art.ipynb` — image processing, color quantization, visuals.

7. Naming colors
   - Objective: map RGB or palette values to human-readable color names (nearest color matching; clustering).
   - Deliverables: `naming_colors.ipynb` — algorithm for nearest-name mapping, palette visualizations.

8. People on banknotes
   - Objective: join metadata (people, countries, years) with images/text; produce descriptive statistics by category.
   - Deliverables: `people_on_banknotes.ipynb` — joins/aggregation and supporting visualizations.

Quick start
-----------
Clone the repository and start a notebook environment:

```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Cisco-Data-science-program/Coding for answers"
python -m venv .venv            # optional but recommended
source .venv/bin/activate      # macOS / Linux
.venv\Scripts\activate         # Windows (PowerShell: .venv\Scripts\Activate.ps1)
pip install -r ../requirements.txt || pip install -r requirements.txt
# if there's no requirements.txt, see "Recommended environment & dependencies" below
jupyter lab                    # or jupyter notebook
```

Recommended environment & dependencies
--------------------------------------
Common, recommended packages used in these notebooks:
- Python 3.8+
- pandas, numpy
- matplotlib, seaborn
- scikit-learn (for clustering or numeric tasks)
- pillow / opencv-python (image tasks)
- geopandas, shapely, folium (geospatial tasks — only if used in the notebook)
- jupyterlab / notebook
- nbconvert / papermill (for executing notebooks programmatically)

Example pip install:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn pillow geopandas folium jupyterlab
```

If you plan to run GeoPandas, installation may require system libs — consider using conda:
```bash
conda create -n cisco3 python=3.9 geopandas jupyterlab pandas matplotlib seaborn scikit-learn pillow
conda activate cisco3
```

How to run the notebooks
------------------------
Open interactively:
- Start Jupyter Lab/Notebook and open the required .ipynb file.

Run a notebook end-to-end (useful for grading or CI):
- Using nbconvert:
```bash
jupyter nbconvert --to notebook --execute --inplace "skeletal_variation.ipynb"
```
- Using papermill (keeps parameterization):
```bash
pip install papermill
papermill input.ipynb output.ipynb -p param1 value1
```
Batch-run all notebooks (careful — this will execute code):
```bash
for n in *.ipynb; do jupyter nbconvert --to notebook --execute --inplace "$n"; done
```
Export a notebook to HTML (for submission/preview):
```bash
jupyter nbconvert --to html skeletal_variation.ipynb
```

Project expectations & assessment checklist
------------------------------------------
When preparing each notebook for submission, aim to meet these expectations:

- Reproducibility
  - All code cells required to reproduce results execute top-to-bottom without errors.
  - Dependencies and data sources are listed at the top.

- Clarity & documentation
  - A short problem statement at the top (“Objective”).
  - Explain methods and show intermediate outputs.
  - Present one or two clear takeaways in a “Conclusions” cell.

- Code quality
  - Use vectorized Pandas operations where reasonable.
  - Avoid overly long cells; split logic into functions when useful.
  - Add comments for non-trivial steps.

- Visualizations
  - Axis labels, titles, and legends where applicable.
  - Use color thoughtfully; include captions or short interpretation.

- Analysis & insights
  - Don’t only show code; explain what the results mean and why they matter.
  - If performing hypothesis tests or comparisons, state the test and interpret results.

Assessment checklist (use before submission):
- [ ] Notebook runs from top to bottom without errors
- [ ] Key assumptions and data sources documented
- [ ] Visualizations are readable and correctly labeled
- [ ] Code is reasonably efficient and commented
- [ ] Short conclusions / next steps included

Tips & common pitfalls
---------------------
- If notebooks fail in CI but work locally, check for hidden state (variables defined in earlier runs). Restart kernel and run all to verify.
- Large datasets: do not commit big raw files to the repo. Instead, provide a small sample or instructions to download.
- For geospatial notebooks: include coordinate reference system (CRS) details when saving/sharing maps.
- When comparing floating-point results, avoid exact equality checks; use tolerances.
- Use relative paths (e.g., `data/myfile.csv`) so notebooks work across local/CI environments.

Datasets & attribution
----------------------
- Keep a `data/` folder for small sample datasets used by notebooks. For large/original datasets, include a `DATASET_LICENSES.md` or a README section that describes where to download them and any license terms.
- Typical sources for these modules:
  - Natural Earth (for simple maps)
  - Kaggle or course-provided CSVs
  - UCI Machine Learning Repository
- Always cite the dataset source and include a URL and license in your notebook.

Contributing
------------
If you want to improve these notebooks or add tests/examples:
1. Fork the repository
2. Create a feature branch: `git checkout -b feat/<short-desc>`
3. Add or improve a notebook, include a short `README_NOTEBOOK.md` inside that notebook's folder explaining dataset requirements
4. Run the notebooks end-to-end
5. Create a pull request with a clear description of changes

If you add dependencies, update `requirements.txt` and add a short note about any system libraries required.

License & contact
-----------------
- Maintainer: [BhavikBuchke](https://github.com/BhavikBuchke)  
- For questions or collaboration, open an issue in the repo or mention me in a PR.

Acknowledgements & learning outcomes
-----------------------------------
This module is designed to build practical skills in:
- data ingesting, cleaning and transformation with Pandas
- exploratory visualization and storytelling with plots
- small algorithmic solutions to problem statements (grid search, connected components)
- elementary geospatial and image/color analysis
- writing reproducible notebooks for assessment and sharing

Thank you — happy analyzing!
