# DataViz-Baby-Names

Visualizations of French baby names (1900-2020), based on the INSEE dataset
[dpt2020.csv](https://perso.telecom-paristech.fr/eagan/class/igr204/data/dpt2020.csv).

## Notebook

- `baby_names.ipynb` : main notebook with the three visualizations

## Setup

```bash
pip install -r requirements.txt
```

Then open the notebooks and run all cells. The dataset and the France GeoJSON are downloaded at
runtime (with retries) and **cached locally** as `dpt2020.csv` / `france.json` (both git-ignored, so
re-runs are instant) — delete them to force a fresh download.

Running all cells writes each visualization to a **self-contained, interactive HTML file** in the
`exports/` folder (`Viz1.html`, `Viz2.html`, `Viz2_comparison.html`, `Viz3.html`). Open them in any
browser — the Vega libraries are embedded inline, so they work offline (no notebook renderer needed).