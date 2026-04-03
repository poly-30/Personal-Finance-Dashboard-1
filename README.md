# Personal Finance Dashboard (Data Analytics Project)

A dynamic personal finance dashboard built using Python, Streamlit, Pandas, Matplotlib, and Seaborn.  
This project simulates real-time financial transactions and provides interactive visual analytics on spending, income trends, and category-wise insights.

---

## Features

- **Real-time Data Generation:**  
  Automatically generates synthetic financial transactions using `Faker` for continuous updates.
  
- **Interactive Dashboard:**  
  Streamlit interface with live-updating charts and metrics.

- **Visual Analytics:**  
  Uses `Matplotlib` and `Seaborn` for:
  - Monthly income vs expense trends  
  - Expense distribution by category  
  - Correlation heatmap of derived financial features  

- **Categorization Logic:**  
  Smart tagging of transactions as *Income* or *Expense* based on the type of transaction (e.g., salary vs groceries).

- **Modular Structure:**  
  Each component (data generation, analysis, and visualization) is handled through cleanly separated scripts.

---

## Prerequisites

- Python 3.8+ installed
- Command line (PowerShell, CMD, Git Bash, WSL)

## Dependencies

The project uses these Python packages:

- streamlit
- pandas
- faker
- streamlit-autorefresh
- matplotlib
- seaborn

## Install Dependencies

From the project root (`e:\finanical dashboard\Personal-Finance-Dashboard`), run:

```bash
pip install streamlit pandas faker streamlit-autorefresh matplotlib seaborn
```

If you have permission issues on Windows, use:

```bash
pip install --user streamlit pandas faker streamlit-autorefresh matplotlib seaborn
```

## Run the App

```bash
python -m streamlit run main.py
```

Then open the URL shown in the terminal (usually `http://localhost:8501`).

## Optional: save generated data

- Check the sidebar option **Save generated data to CSV** to persist transactions to `data/historical_data.csv`.

## Notes

- If `streamlit` is not found, running as module (`python -m streamlit run main.py`) avoids PATH shell detection issues.
- Keep `main.py` and `analysis.py` in the same folder (as they are now).
