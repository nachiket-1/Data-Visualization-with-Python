<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=24,18,3,17,12&height=220&section=header&text=📊%20Data%20Visualization&fontSize=52&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=with%20Python%20—%20The%20Complete%20Visual%20Guide&descAlignY=58&descSize=20" width="100%"/>

<br/>

[![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-11557C?style=for-the-badge&logo=python&logoColor=white)](https://matplotlib.org)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.12%2B-4c72b0?style=for-the-badge&logo=python&logoColor=white)](https://seaborn.pydata.org)
[![Plotly](https://img.shields.io/badge/Plotly-5.x-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)](https://plotly.com/python)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org)
[![Kaggle](https://img.shields.io/badge/Open%20in-Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://kaggle.com)
[![License](https://img.shields.io/badge/License-MIT-06d6a0?style=for-the-badge)](LICENSE)

<br/>

> *"The greatest value of a picture is when it forces us to notice what we never expected to see."*
> — John W. Tukey

<br/>

**10 chart types. 3 libraries. 1 notebook. Zero boring visuals.** 🎨

<br/>

</div>

---

## 📖 About

This notebook is a **hands-on, colorful guide to data visualization in Python** — built for anyone who wants to turn raw data into charts that actually tell a story. No prior visualization experience needed.

Every section covers a different chart type, explains *when* to use it (not just *how*), and comes with live `# TRY:` experiments so you can explore and customize immediately.

---

## 🗺️ Table of Contents

- [What's Inside](#-whats-inside)
- [Chart Gallery](#-chart-gallery)
- [Quick Start](#-quick-start)
- [The Chart Chooser](#-the-chart-chooser)
- [Requirements](#-requirements)
- [Run on Kaggle](#-run-on-kaggle)
- [Run Locally](#-run-locally)
- [Libraries Compared](#-libraries-compared)
- [Experiment Ideas](#-experiment-ideas)
- [What's Next](#-whats-next)

---

## 📦 What's Inside

| # | Section | Library | Key Concepts |
|---|---------|---------|-------------|
| 0 | **Setup** | — | Imports, global theme, custom palette |
| 1 | **Line Chart** | Matplotlib | Multi-series, filled areas, value annotations |
| 2 | **Bar Chart** | Matplotlib | Grouped bars, horizontal bars, sorted ordering |
| 3 | **Scatter / Bubble** | Matplotlib | 4-variable encoding, trend lines, alpha blending |
| 4 | **Histogram** | Matplotlib | 4 distribution shapes explained with examples |
| 5 | **Pie & Donut** | Matplotlib | Exploded slices, center text, legend placement |
| 6 | **Heatmap** | Seaborn | Correlation matrix, masking, color divergence |
| 7 | **Box + Violin** | Seaborn | IQR, outliers, density comparison side by side |
| 8 | **Interactive Chart** | Plotly | Hover tooltips, unified mode, zoom & pan |
| 9 | **Dashboard Layout** | Matplotlib | `subplot_mosaic`, KPI cards, multi-panel design |
| 10 | **Chart Chooser** | — | Quick-reference table for picking the right chart |

---

## 🎨 Chart Gallery

```
📈  Line Chart        ╱‾‾╲_╱‾‾╲___╱‾        Trends over time
📊  Bar Chart         ▌ ▌▌ ▌▌ ▌▌             Compare categories
🔵  Scatter / Bubble  · ·  · ·  ·  ·         Two-variable relationships
📉  Histogram         ▁▃▇█▇▅▃▁               Data distribution shapes
🥧  Pie / Donut       ◔ ◑ ◕ ●                Part-to-whole breakdown
🟥  Heatmap           🟩🟨🟥🟥🟩🟨          Correlation between variables
📦  Box / Violin      |—[  |  ]—|            Statistical summaries
🌐  Plotly            ≋≋≋ (hover me!) ≋≋≋   Interactive exploration
🖥️  Dashboard         [line ][KPI]           Multi-chart layouts
              [donut][bar   ]
```

---

## ⚡ Open Notebook in Kaggle

[![Open in Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code/nachikettalekar/data-visualization-with-python))

---

## 🧭 The Chart Chooser

Not sure which chart to use? Use this table:

| I want to show... | Best Chart | One-liner |
|-------------------|-----------|-----------|
| Change over time | Line Chart | `ax.plot(x, y)` |
| Compare categories | Bar Chart | `ax.bar(x, y)` |
| Relationship between 2 variables | Scatter Plot | `ax.scatter(x, y)` |
| How data is distributed | Histogram | `ax.hist(data, bins=30)` |
| Part-to-whole breakdown | Pie / Donut | `ax.pie(sizes)` |
| Correlation between many variables | Heatmap | `sns.heatmap(df.corr())` |
| Statistical summary | Box / Violin | `sns.boxplot()` |
| Interactive web chart | Plotly | `px.line(df, x=..., y=...)` |
| Multiple charts together | Dashboard | `plt.subplot_mosaic(...)` |

---

## 📋 Requirements

```txt
matplotlib>=3.5.0
seaborn>=0.12.0
plotly>=5.0.0
numpy>=1.21.0
pandas>=1.3.0
```

Install everything at once:

```bash
pip install -r requirements.txt
```

> ✅ All dependencies are **pre-installed** on Kaggle and Google Colab.

---

## 🏁 Run on Kaggle

1. Upload the notebook via **File → Import Notebook**
2. No additional installs needed — all libraries are available
3. Plotly charts render inline in the notebook output
4. Any saved files (PNG exports) appear in `/kaggle/working/`

To save a chart as an image:
```python
plt.savefig('my_chart.png', dpi=150, bbox_inches='tight')
```

---

## 💻 Run Locally

```bash
# 1. Clone the repo
git clone https://github.com/nachiket-1/data-visualization-python.git
cd data-visualization-python

# 2. (Recommended) Create a virtual environment
python -m venv venv
source venv/bin/activate        # macOS / Linux
venv\Scripts\activate           # Windows

# 3. Install dependencies
pip install -r requirements.txt

# 4. Launch Jupyter
jupyter notebook
# or JupyterLab:
jupyter lab
```

---

## ⚖️ Libraries Compared

| Feature | Matplotlib | Seaborn | Plotly |
|---------|-----------|---------|--------|
| Output type | Static image | Static image | Interactive HTML |
| Learning curve | Medium | Low | Low–Medium |
| Best for | Full control, custom layouts | Statistical charts | Web & dashboards |
| Works with DataFrames | Manually | Natively | Natively |
| Default aesthetics | Basic | Beautiful | Beautiful |
| Animations | Yes (FuncAnimation) | No | Yes |
| 3D charts | Yes | No | Yes |

**Rule of thumb:**
- Start with **Seaborn** for quick EDA
- Use **Matplotlib** when you need full control or custom layouts
- Use **Plotly** when your audience will interact with the chart

---

## 🧪 Experiment Ideas

After going through the notebook, try these challenges:

- 📅 **Real data** — load `sns.load_dataset('titanic')` and recreate every chart with real data
- 🌍 **Choropleth map** — use `px.choropleth()` to make an interactive world map
- 🎨 **Custom theme** — create your own `plt.rcParams` style and apply it globally
- 📐 **Annotation master** — add arrows, text boxes, and highlights to explain chart insights
- 📦 **Pair plot** — use `sns.pairplot(df)` to explore all variable relationships at once
- 🌡️ **Diverging bar chart** — show positive vs negative values with color coding
- 🕸️ **Radar chart** — compare multi-attribute profiles in a spider web layout

---

## 📁 Repository Structure

```
data-visualization-python/
│
├── 📓 data_visualization_python.ipynb   ← Main notebook
├── 📋 README.md                          ← This file
└── 📦 requirements.txt                   ← Dependencies
```

---

## 🚀 What's Next?

| Topic | Resource |
|-------|---------|
| More chart types | [Matplotlib Gallery](https://matplotlib.org/stable/gallery/) |
| Statistical deep dive | [Seaborn Tutorial](https://seaborn.pydata.org/tutorial.html) |
| Interactive dashboards | [Plotly Dash](https://dash.plotly.com/) |
| No-code dashboards | [Streamlit](https://streamlit.io/) |
| Geographic maps | [Folium](https://python-visualization.github.io/folium/) |
| Practice datasets | [Kaggle Datasets](https://www.kaggle.com/datasets) |

---

## 🤝 Contributing

Have a chart type that should be added? Found a bug?

1. Fork the repository
2. Create a branch: `git checkout -b feature/add-radar-chart`
3. Make your changes and submit a Pull Request

---

## 📄 License

This project is open source under the **MIT License** — free to use, share, and build on.

---

<div align="center">

**Made with ❤️, Python, and way too many color gradients**

If this helped you learn something new, a ⭐ on the repo means the world!

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=24,18,3,17,12&height=120&section=footer" width="100%"/>

</div>
