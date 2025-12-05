# Franzy -- Smart Finance Categorization Dashboard 💳

Franzy is a Streamlit-powered finance dashboard that helps users upload
bank transaction CSV files, automatically categorize expenses, visualize
spending patterns, and save category rules locally using JSON.\
This tool is ideal for anyone who wants a simple, offline-friendly way
to analyze personal finances.

## 📌 Features

### 🧾 CSV Upload

- Upload bank transaction files in `.csv` format.
- Automatically cleans and parses fields such as:
  - Date\
  - Amount\
  - Details\
  - Debit/Credit

### 🏷 Smart Categorization

- Auto-assign categories based on stored keywords.
- Add unlimited custom categories.
- Save keywords to `categories.json` so future uploads get
  auto-categorized.

### ✏️ Editable Expense Table

- Modify categories directly inside the UI using `st.data_editor`.
- Category changes automatically update your JSON file.

### 📊 Interactive Dashboards

- Expense pie chart (Plotly)
- Category-wise total summary
- Payment summary for Credits

### 💾 Persistent Storage

- No database required\
- All rules stored locally in a JSON file (`categories.json`)

## 🗂 Project Structure

    Franzy/
    │── main.py               # Main Streamlit application
    │── categories.json       # Category rules (auto-updated)
    │── README.md             # Project documentation
    │── sample.csv            # Optional example CSV
    └── assets/               # Optional screenshots or banners

## 🚀 Getting Started

### 1️⃣ Install Dependencies

    pip install streamlit pandas plotly

### 2️⃣ Run the Application

    streamlit run main.py

## 📥 How to Use

### ✔ Step 1 --- Upload CSV

Upload your bank statement containing the following columns:

- Date\
- Details\
- Amount\
- Currency\
- Debit/Credit\
- Status

### ✔ Step 2 --- Categorize

- Add new categories\
- Edit category in the data editor\
- System automatically saves keywords for future auto-categorization

### ✔ Step 3 --- View Visual Dashboard

- Expense pie chart\
- Category totals table\
- Payment (Credit) summary

## 🧰 Technologies Used

Technology Purpose

---

Python Core logic
Streamlit Web UI
Pandas Data handling
Plotly Express Interactive charts
JSON Local storage for categories

## 📂 Category Rules Example (`categories.json`)

```json
{
  "Uncategorized": [],
  "Shopping": [
    "Daraz",
    "Imtiaz Supermarket",
    "Al-Fatah",
    "Apple Services PK",
    "Booking.com Pakistan"
  ],
  "Travel": ["PIA", "PC Hotel Karachi", "Careem"],
  "Insurance": ["Jubilee Insurance"],
  "Bank Fee": ["Bank Fee (PK)"],
  "Subscriptions": ["Netflix Pakistan"],
  "Food & Delivery": ["FoodPanda"]
}
```

## 🤝 Contributing

1.  Fork the repository\
2.  Create a new feature branch\
3.  Commit your changes\
4.  Open a pull request

## 👨‍💻 Author

**Zack / AK-Dev**

## 📜 License

This project is licensed under the **MIT License**.
