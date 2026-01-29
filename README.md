# International sales marketing strategy

## Project Overview
This repository contains a tablea dashboard developed to create several visualizations to create effective global marketing strategies. It will analyze historical trends, product populatiry, and regional performance and preferences.


## Repository Purpose
This repository contains
- Data cleaning and preparation scripts
- Interactive Tableau workbook with dashboards and at least one story
- Project documentation
- data dictionary
- Team contributions
- AI usage documentation

## Business Objective:
Use data insights to create effective targeted marketing strategies for different global regions based on historical sales trends including sales volume and type of product.

## Expected Uses:
The dashboard will incorporate visualizations to help better understand product popularity and sales trendlines. The interactive nature of the dashboard will allow for filtering of sales numbers by product category, geographical region, cancellations of orders, and other pertinent factors.

## How to use this Repository

### Prerequisites
- Python 3.x
- Tableau Desktop
- Tableau Prep (for cleaning data)

### Setup instructions:

1. **Clone the repository**
```bash
   git clone https://github.com/BunnyBea83/DAB-Project-1-Sales-Tracking-Dashboard.git
   cd [DAB-Project-1-Sales-Tracking-Dashboard]
```

2. **Review the raw data**
   - Original dataset is located in `sales_data_sample.csv`
   -Check out `data_dictionary.md` for further information behind the data columns

3. **Open the Tableau Prep flow (optional)**
   - Open Tableau Prep Builder
   - Open `sales_data_sample.csv`
   - Review the cleaning steps applied
   - Run the flow to generate cleaned data (if modifications needed)
   - NOTE: the Phone column may require additonal python scripting and steps in order to clean the data

4. **Open the Tableau workbook**
   - Navigate to `Sales_Tracking_Dashboard.twbx`
   - Open with Tableau Desktop
   - The packaged workbook should include already cleaned data from the original source.

5. **About the Tableau workbook**
   - There are color coded worksheets. These colors represent who created the visualization
      - Blue = Kainen Osborne
      - Purple = Bea Sauve
      - Yellow = Elton Nichols
   - There are dashboards with accumulated visualizations that give us our company insights
   - To display the accumulated project select the "Sales Tracker Story" Story Board, and select the present button
      - The story board is interactable, you can hover your mouse above elements to view greater details, and select certain portions of data to highlight that specific element.

## Team Information
See `CONTRIBUTING.md` for detailed breakdown of team member responsibilities.

## AI Usage
See `AI.md` for documentation of AI tools used in this project.


## Authors

| Name            | Role(s)                                   | Username         |
|-----------------|-------------------------------------------|------------------|
| Bea Sauve       | Code Developer, Project Manager          | bunnybea83       |
| Elton Nichols   | Code Developer, Version Control Manager            | oi12bu           |
| Kainen Osborne  | Code Developer, Analysis Auditor Manager    | kosborne00       |