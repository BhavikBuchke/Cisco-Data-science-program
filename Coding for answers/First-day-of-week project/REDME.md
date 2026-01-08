# First Day / Week — Data & download instructions

Purpose
- Small warm-up exercises to verify environment and run simple EDA examples.

Datasets used
- sample_attendance.csv (small CSV used for in-notebook examples)
- sample_timeseries.csv (tiny timeseries for plotting exercises)

Download instructions
1. If the dataset is included in the repo:
   - Place the files in this folder's `data/` subfolder:
     ```
     Coding for answers/First-day-of-week project/data/first-day-of-week.csv
     Coding for answers/First-day-of-week project/data/four-regions.csv
     Coding for answers/First-day-of-week project/data/population.csv
     ```
2. If you need to re-download the sample files from a remote location:
   - Using curl:
     ```
     mkdir -p "Coding for answers/First-day-of-week project/data"
     curl -L -o "Coding for answers/first day week/data/sample_attendance.csv" "https://example.com/sample_attendance.csv"
     ```
   - Or using wget:
     ```
     wget -O "Coding for answers/first day week/data/sample_attendance.csv" "https://example.com/sample_attendance.csv"
     ```
Notes
- Notebooks expect relative paths like `data/sample_attendance.csv`. If you place files elsewhere, update the path at the top of the notebook.
