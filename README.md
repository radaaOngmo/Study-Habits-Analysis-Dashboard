# Study Habits Analysis Dashboard
Final clean, Bhutan-inspired Streamlit dashboard for the PRG405 project at Samtse College of Education.

## Included
- `app.py` — complete Streamlit application
- `requirements.txt` — Python dependencies
- `data/study_habits_dashboard.csv` — cleaned dataset (146 participants, 39 columns)
- `assets/bhutan_emblem.png` — Samtse College of Education emblem used in the sidebar

No other photographs are used. The header and decorative details are created with CSS.

## Run on Windows (VS Code)
1. Extract the ZIP.
2. In VS Code, choose **File → Open Folder** and select the extracted `Study_Habits_Dashboard_Final` folder.
3. Open **Terminal → New Terminal**. Confirm the terminal is in the folder containing `app.py`.
4. Install dependencies:

```powershell
python -m pip install -r requirements.txt
```

5. Start the dashboard:

```powershell
python -m streamlit run app.py
```

6. Open `http://localhost:8501` if it does not open automatically.

## Dashboard pages
1. Dashboard Home
2. Project Overview
3. Research Objectives
4. Data Analysis
5. Findings & Results
6. Conclusion
7. References

## Interactivity
- Year of study, gender and academic percentage filters apply across all pages.
- The Reset filters button restores the complete sample.
- Use the sidebar **Dark mode** toggle to switch between light and dark themes.
- Plotly chart toolbar supports zoom, pan, reset and PNG export. The Streamlit chart expand control opens a chart in fullscreen; use its close/exit control or press Esc to return.
- Browser zoom can be reset with `Ctrl + 0`.

## Data integrity notes
The dashboard reads the supplied cleaned CSV and does not silently re-clean or change the dataset. The displayed full-sample values are calculated from that file. The supplied dataset does not include a separate before-and-after measure of study-habit improvement, so the dashboard does not claim an improvement percentage. The references page distinguishes the supplied data and software from academic references that the group must add from sources actually consulted.

## Troubleshooting
If PowerShell says it cannot find `requirements.txt`, use VS Code **File → Open Folder** to open the extracted project folder, then open a new terminal. Run `dir` and confirm `app.py` and `requirements.txt` appear in the listing.


## Latest requested refinements
- Added plain-language interpretations beneath the study schedule, bedtime, preferred study environment, learning approaches, exam review frequency and distraction frequency charts.
- Added reading guidance beneath the relationship scatterplots and Spearman correlation heatmap/table.
- Added the supplied classroom photo as the title-bar background only, with a translucent overlay so the title remains readable in both themes.
