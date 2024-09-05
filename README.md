# YemekSepetiAnalyzes

This project performs analysis on customer orders from YemekSepeti. It calculates metrics such as Contact Rate, Self-Service Rate, Seamless Order Rate, NPS (Net Promoter Score), and CSAT (Customer Satisfaction) scores. Additionally, it visualizes data to provide deeper insights into customer satisfaction based on order size and payment method preferences.

## Project Structure

```bash
YemekSepetiAnalyzes/
│
├── .venv/                             # Python virtual environment
├── data/
│   └── task1-dataset-1723704917.xlsx  # Excel dataset file
├── src/
│   └── main.py                        # Main Python script for analysis
├── correlation_matrix.png             # Correlation matrix visualization
├── order_size_vs_csat.png             # Scatterplot: Order Size vs CSAT
├── csat_by_payment_method.png         # Bar chart: CSAT by Payment Method
└── README.md                          # Project documentation (this file)
```

## Dependencies

Before running the script, install the necessary dependencies:

- pandas
- matplotlib
- seaborn
- openpyxl

You can install all required packages using the following command:

```bash
pip install pandas matplotlib seaborn openpyxl
```

## How to Run the Project

Clone the repository:

```bash
git clone https://github.com/yourusername/YemekSepetiAnalyzes.git
```

Navigate to the project folder:

```bash
cd YemekSepetiAnalyzes
```

Activate the virtual environment:

For macOS/Linux:

```bash
source .venv/bin/activate
```

For Windows:

```bash
.venv\Scripts\activate
```

Run the Python script:

```bash
python src/main.py
```

The script will load the dataset from the data folder and perform the following operations:

- Calculate various rates (Contact Rate, Self-Service Rate, Seamless Order Rate).
- Calculate average NPS and CSAT scores.
- Perform analysis for Self-Service channels, including correlations between order size, NPS, and CSAT.
- Generate and save visualizations to .png files.

## Output Visualizations

- **Correlation Matrix (correlation_matrix.png):** Displays the correlations between order_size_TRY, SelfServiceCSAT, and NPS-Q-Score for Self-Service orders.
- **Order Size vs CSAT (order_size_vs_csat.png):** Scatterplot showing the relationship between order size (in TRY) and Self-Service CSAT.
- **CSAT by Payment Method (csat_by_payment_method.png):** Bar chart showing the average Self-Service CSAT for different payment methods.

## Dataset

The project uses the following dataset, located in the data folder:

- **task1-dataset-1723704917.xlsx:** An Excel file containing detailed information about each order, such as whether it was a contact or self-service order, the order size, NPS score, CSAT ratings, and the preferred payment method.

Make sure the dataset is available at the correct path (data/task1-dataset-1723704917.xlsx) before running the script.