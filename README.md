# Superstore Sales & Profitability Dashboard part 2

An interactive data analytics dashboard built with Python and Streamlit for BAN-461: Advanced Data Modeling Systems.

**Analytical Question:** *Which product categories and regions drive the most profit — and how have margin trends shifted from 2011 to 2014?*

**Live App:** *(paste your Streamlit Community Cloud URL here)*
**GitHub Repo:** *(paste your GitHub repository URL here)*

---

## Project Structure

```
├── app.py               # Main Streamlit application
├── requirements.txt     # Python dependencies
├── superstore.xlsx      # Dataset (9,994 retail transactions, 2011–2014)
└── README.md            # This file
```

---

## Dashboard Features

- **4 KPI metrics** — Total Revenue, Total Profit, Avg Profit Margin, and Top Profit Region, all updating dynamically with filters
- **4 sidebar filters** — Region, Product Category, Year Range, and Customer Segment
- **3 visualizations** — Grouped bar chart, profit margin trend line, and Sales vs. Profit bubble scatter plot
- **Key Findings section** — Analytical conclusions tied to business decisions
- **Filtered data table** — Raw data view that reflects active filters
- **CSV export** — Download the filtered dataset with one click

---

## Running Locally

### Prerequisites

- Python 3.9 or higher
- pip

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. **Create and activate a virtual environment** *(recommended)*
   ```bash
   python -m venv venv

   # macOS / Linux
   source venv/bin/activate

   # Windows
   venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the app**
   ```bash
   streamlit run app.py
   ```

5. **Open in your browser**
   Streamlit will automatically open the app. If it doesn't, navigate to:
   ```
   http://localhost:8501
   ```

---

## Dataset

The Superstore dataset contains 9,994 retail transactions from a fictional U.S. office supply company spanning 2011–2014. Key fields used in this dashboard:

| Column | Description |
|---|---|
| `Order Date` | Date the order was placed |
| `Region` | U.S. sales region (Central, East, South, West) |
| `Category` | Product category (Furniture, Office Supplies, Technology) |
| `Sub-Category` | Product sub-category (17 total) |
| `Segment` | Customer segment (Consumer, Corporate, Home Office) |
| `Sales` | Revenue for the order line ($) |
| `Profit` | Profit for the order line ($) |
| `Profit Ratio` | Profit as a proportion of sales |
| `Quantity` | Units sold |

---

## Dependencies

| Package | Purpose |
|---|---|
| `streamlit` | Web app framework |
| `pandas` | Data loading and transformation |
| `plotly` | Interactive charts |
| `openpyxl` | Reading the `.xlsx` data file |
