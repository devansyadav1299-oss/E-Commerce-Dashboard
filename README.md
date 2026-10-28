# E-Commerce-Dashboard
An end-to-end e-commerce data analytics project featuring an interactive Power BI dashboard designed using the Fluent 2 UI framework to track sales velocity, profitability channels, and regional customer demographics across India.

# E-Commerce Sales & Profit Performance Dashboard

An end-to-end data analytics project featuring an interactive Power BI report built to analyze sales, transaction amounts, profitability, and customer behavior across various categories and geographic regions in India.

## 📁 Repository Structure

*   `List of Orders.csv` - Contains regional and customer demographics details (Order Date, Customer Name, State, City).
*   `Order Details.csv` - Contains transactional, item-level breakdowns (Amount, Profit, Quantity, Category, Payment Mode).
*   `Fluent2-CY26SU09.pbix` (Extracted layout package) - Power BI layout blueprint template utilizing the Fluent 2 responsive design framework.

---

## 📊 Data Architecture & Schema

The dataset uses a star/snowflake-adjacent schema normalized across transaction records and regional mapping tables, joined securely via `Order ID`.

### 1. Order Details (`Order Details.csv`)
Tracks transactional performance and logistical dynamics at the sub-category level.
*   **Order ID:** Unique alphanumeric transaction token.
*   **Amount:** Gross transactional value in local currency.
*   **Profit:** Net financial gain or loss derived per transaction.
*   **Quantity:** Unit volume per order line.
*   **Category / Sub-Category:** High-level groupings (Electronics, Clothing, Furniture) broken down into item specifications (Printers, Sarees, Chairs, etc.).
*   **Payment Mode:** Method of payment fulfillment (COD, UPI, Credit Card, EMI, Debit Card).

### 2. Customer Registry (`List of Orders.csv`)
Provides dimensional context mapping transactions to temporal and geographic vectors.
*   **Order ID:** Unique key linking details to customer attributes.
*   **Order Date:** Temporal stamp mapping purchase windows throughout the fiscal calendar.
*   **Customer Name:** Standardized client identity ledger.
*   **State / City:** Geospatial points representing Indian market distribution (e.g., Maharashtra, Uttar Pradesh, Delhi).

---

## 🛠️ Power BI Design Framework

The visual interface configuration details contained within the zipped bundle reference `Fluent2-CY26SU09.json` and `Tidal.json` theme definitions. The design features:
*   **Color Theme:** Tidal suite styling incorporating cohesive, responsive dark-to-light gradient components.
*   **Typography & UI Elements:** Implements modern Fluent 2 styles to create a highly corporate, clean dashboard layout.

---

## 🚀 How to Setup and Run

1. **Clone the Repository:**
   ```bash
   git clone https://github.com
   ```
2. **Launch Dashboard:**
   * Open the `.pbix` file in **Power BI Desktop**.
   * If paths break, navigate to `Home` > `Transform Data` > `Data Source Settings` and remap the source files to your local paths for `Order Details.csv` and `List of Orders.csv`.
