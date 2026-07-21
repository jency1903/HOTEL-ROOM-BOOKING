# Hotel Room Booking Report (Power BI)

A single-page Power BI dashboard that analyzes hotel room booking performance — revenue, profit, quantity, discount, and rating — across categories, regions, cities, and time, built on top of a `25_Hotel_Bookings` dataset.

## 📄 File

- **`HOTEL_ROOM_BOOKING.pbix`** — Power BI Desktop report file

## 📊 Data Model

The report is built on a single table:

| Table | Fields |
|---|---|
| `25_Hotel_Bookings` | Category, Sub_Category, Region, City, Status, Transaction_Date, Revenue, Profit, Quantity, Discount, Rating |

`Transaction_Date` uses Power BI's built-in Date Hierarchy (Year, Month) to power the time-based visuals.

## 🖥️ Report Page — "Report of Hotel Room Booking" (5000 × 3500)

| Visual | Type | Details |
|---|---|---|
| **KPI Card** | Card | Displays Sum of Profit, Sum of Quantity, Sum of Rating, and Sum of Revenue |
| **City-Wise Profit Analysis** | Treemap | Sum of Profit sized by City |
| **Total Discounts Across Regions** | Pie Chart | Sum of Discount broken down by Region |
| **Regional Sub-Category Trends** | Clustered Column Chart | Count of Sub_Category by Category, split by Status and Region |
| **Trend of Sub-Category Counts by Year** | Line Chart | Count of Sub_Category trended across Transaction Date (Year and Month) |
| **Annual Financial Performance by Region and Category** | Scatter Chart | Sum of Revenue (X) vs. Sum of Profit (Y), played over Transaction Year, categorized by (First) Category and colored by Region |
| **Region Count by Quantity** | Ribbon Chart | Sum of Quantity ranked by Region |
| **Aggregate Metrics Gauge - Rating & Quantity** | Gauge | Sum of Rating as the value, Sum of Quantity as the target |
| **Slicer** | Slicer | Filter by Status |
| **Slicer** | Slicer | Filter by Region |
| **Slicer** | Slicer | Filter by Category |
| **Slicer** | Slicer | Filter by Transaction_Date (Year) |
| **Title Textbox** | Textbox | "Report of Hotel Room Booking" |
| **Background Shape** | Shape | Decorative layout element |

## 🎨 Theme

Built-in Power BI theme **Accessible Tidal** applied to the report for consistent, accessibility-friendly colors across visuals.

## 🔍 Key Insights the Report Enables

- Track **profit, quantity, rating, and revenue** at a glance via KPI cards
- Identify the **most profitable cities** using the treemap
- Compare **discount distribution across regions**
- Analyze **sub-category booking trends by category, status, and region**
- Monitor **sub-category counts over time** (year and month)
- Explore the **relationship between revenue and profit** across regions and categories, animated by year
- Rank **regions by booking quantity** with the ribbon chart
- Track **rating performance against quantity targets** using the gauge
- Filter the entire report interactively by **Status, Region, Category, and Year**

## 🛠️ Requirements

- [Power BI Desktop](https://powerbi.microsoft.com/desktop/) to open and edit `HOTEL_ROOM_BOOKING.pbix`
- No external data source connections required beyond the embedded dataset

## 📂 Usage

1. Clone/download this repository
2. Open `HOTEL_ROOM_BOOKING.pbix` in Power BI Desktop
3. Use the slicers (Status, Region, Category, Year) to filter the report
4. Play the scatter chart's year animation to see revenue vs. profit trends evolve over time
