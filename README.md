# 🍽️ Zomato Data Analysis

Exploratory Data Analysis (EDA) of a Zomato restaurant dataset, uncovering insights about restaurant types, ratings, votes, cost trends, and online ordering behavior using Python, Pandas, Matplotlib, and Seaborn.

---

## 📁 Project Structure

```
zomato-data-analysis/
│
├── zomato_DA.ipynb       # Main Jupyter Notebook with full EDA
├── Zomato_data_.csv      # Dataset used for analysis
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
```

---

## 📊 Dataset Overview

The dataset contains **148 rows** and **7 columns** with information about restaurants listed on Zomato:

| Column | Description |
|---|---|
| `name` | Name of the restaurant |
| `online_order` | Whether the restaurant accepts online orders (Yes/No) |
| `book_table` | Whether the restaurant allows table booking (Yes/No) |
| `rate` | Customer rating (e.g., 4.1/5) |
| `votes` | Number of votes/reviews received |
| `approx_cost(for two people)` | Approximate cost for two people (in INR) |
| `listed_in(type)` | Type of restaurant (e.g., Buffet, Dining, Cafes) |

---

## 🔍 Analysis Performed

The notebook covers the following steps:

1. **Data Loading** — Loading the CSV into a Pandas DataFrame
2. **Data Preview** — Examining the first few rows, shape, and column info
3. **Data Preprocessing** — Cleaning the `rate` column by extracting numeric values
4. **Visualizations** (using Matplotlib & Seaborn):
   - **Restaurant type distribution** — Count plot of restaurant types (`listed_in(type)`)
   - **Votes by restaurant type** — Line plot showing total votes per type
   - **Rating distribution** — Histogram of restaurant ratings
   - **Couple spending** — Count plot of approximate cost for two people
   - **Online order vs Rating** — Box plot comparing ratings by order mode
   - **Heatmap** — Pivot table heatmap of restaurant type vs. online order availability

---

## 📈 Key Insights

- **Dining** restaurants receive the most votes, indicating higher customer engagement.
- **Most restaurants** have ratings between **3.5 and 4.0**.
- The majority of couples prefer restaurants with an approximate cost of **₹300**.
- Restaurants that accept **online orders** tend to receive **higher ratings** compared to those that don't.

---

## 🛠️ Tech Stack

- **Python 3.x**
- **Pandas** — data manipulation and preprocessing
- **NumPy** — numerical operations
- **Matplotlib** — static visualizations
- **Seaborn** — statistical visualizations
- **Jupyter Notebook** — development environment (Google Colab compatible)

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/zomato-data-analysis.git
cd zomato-data-analysis
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the notebook

```bash
jupyter notebook zomato_DA.ipynb
```

> **Note:** If using Google Colab, update the file path in the data loading cell from `/content/Zomato data .csv` to the appropriate path after uploading the dataset.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
