Airbnb Listings EDA Project: New York 2024
Project Overview
This project performs Exploratory Data Analysis (EDA) on New York Airbnb data to uncover trends and patterns in rental listings. Leveraging libraries such as Pandas, Numpy, Matplotlib, and Seaborn for data cleaning, visualization, and analysis, we explore both univariate and bivariate trends.



Objective
The aim of this project is to:

Analyze room types, prices, and availability across different neighborhoods.
Examine host behavior and listing patterns.
Identify potential outliers in prices.
Provide actionable recommendations for guests and hosts based on insights.
Dataset
The dataset consists of 20,765 entries and 22 features, including:

id: Unique identifier for each listing
name: Title of the Airbnb listing
host_name: Name of the host
neighborhood_group: Group (borough) where the listing is located
latitude/longitude: Geolocation of listings
price: Nightly rental price
room_type: Type of accommodation (e.g., entire home, private room)
reviews_per_month: Average monthly reviews for the listing
availability_365: Number of available days in the year
Steps and Workflow
1. Data Cleaning
Handle missing data: Addressed null values in price, neighborhood, and beds columns.
Adjust data types: Converted last_review to a datetime object.
Outlier removal: Capped listings with prices > $1,000 to prevent skewed visualizations.
2. EDA (Exploratory Data Analysis)
Room type distribution:

Visualized counts of each room type using bar plots.
Identified Entire home/apt as the most prevalent room type.
Neighborhood group insights:

Analyzed price variations by boroughs.
Observed Manhattan has the highest average prices.
Availability trends:

Created heatmaps to show correlations among price, availability_365, number_of_reviews, and beds.
Price distribution:

Visualized price distribution using histograms.
Majority of listings are priced between $50 - $300.
Host listings:

Analyzed hosts with multiple listings using boxplots to understand key players.
Review behavior:

Used pair plots to explore relationships between number_of_reviews, price, and availability.
3. Data Visualization
Pairplot: Shows correlations among price, availability, and number of reviews.
Heatmap: Displays correlations among numerical features.
Histograms and Boxplots: Helped detect outliers in price.
Bar Charts: Illustrated room type and neighborhood group distributions.
Key Findings and Insights
Price Trends:

Manhattan listings are the most expensive, followed by Brooklyn.
Entire homes/apartments cost significantly more than private or shared rooms.
Room Type Distribution:

Entire homes/apartments are most common, while private rooms offer more budget-friendly options.
Outliers in Price:

A few listings priced at $10,000+ suggest a need to filter extreme values for more accurate insights.
Availability Patterns:

High-availability listings tend to have lower prices and more reviews, suggesting a better guest experience.
Host Behavior:

Certain hosts manage multiple listings, indicating professional hosting trends.
How to Run This Project
Clone the repository:
bash
Copy code
git clone https://github.com/najirh/Python-Project-P2-New-York-AirBnb-Listing-2024.git
Install the required libraries:
bash
Copy code
pip install pandas numpy matplotlib seaborn
Run the Jupyter notebook or Python script:
bash
Copy code
jupyter notebook day23_airbnb_eda.ipynb
Recommendations
For Guests:

Seek listings with high availability and positive reviews for a better experience.
Private rooms in Brooklyn provide cost-effective options compared to Manhattan.
For Hosts:

Focus on availability and review response rates to improve bookings.
Use competitive pricing to stand out in the borough market.
Future Work
Implement machine learning models to predict prices based on room type and location.
Perform sentiment analysis on reviews to understand guest preferences.
Develop an interactive dashboard using Plotly or Tableau for real-time insights.
Conclusion
This EDA project offers in-depth insights into the New York Airbnb market, aiding guests and hosts in making informed decisions. By employing EDA techniques, we discovered key trends and provided actionable recommendations. Future enhancements include advanced analytics and predictive modeling to extend the findings.

License
This project is open-source and licensed under the MIT License. Feel free to use and modify the code.

Contact
For any queries, feel free to reach out at:

GitHub: Your GitHub
LinkedIn: Your LinkedIn
