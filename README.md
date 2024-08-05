# Project Title: Effects of an Event on Barcelona’s Rental Prices
### Overview
This project investigates the impact of a major annual event, the Sónar Festival, on rental prices in Barcelona, using data scraped from "booking.com". The study also includes a comparison with Valencia to provide a control for the analysis. The objective is to identify and quantify the effect of the festival on rental prices, employing various text mining and natural language processing techniques.

### Authors
+ Mathieu Breier
+ Angelo Di Gianvito
+ Daniela Vélez

### Data Collection
Event Dates: June 13-15, 2024
Comparison Dates: June 6-8, 2024
Cities: Barcelona (treatment city) and Valencia (control city)
Scraped Data: Date, room price, hotel name, and hotel description

### Methodology
1. Scraping Pipeline:

+ Organized data requirements and storage format.
+ Automated data scraping using Python and Selenium.
+ Scraped data includes hotel names, descriptions, prices, and dates.

2. Regression Models:

+ Model 1: Impact of treatment city on price.
+ Model 2: Impact of treatment period on price.
+ Model 3: Difference-in-Differences (DiD) model incorporating both treatment period and city.
+ Model 4: Enhanced DiD model with additional controls for luxury and amenities.

### Analysis
#### Regression Analysis:

+ The interaction term in Model 3 captures the net effect of the event on prices.
+ Model 4 includes luxury and amenities as additional controls to refine the analysis.

#### Feature Extraction:

+ Extracted text features from hotel descriptions related to luxury and amenities.
+ Generated dummy variables to represent these features.

### Results

+ Model 1: Average price difference between Barcelona and Valencia during the event period is significant.
+ Model 2: Average price increase in both cities during the event period is significant.
+ Model 3: Significant positive effect of the Sónar Festival on hotel prices in Barcelona.
+ Model 4: The inclusion of luxury and amenities controls confirms the robustness of the event's impact on prices.

### Conclusion
The study demonstrates that the Sónar Festival significantly increases rental prices in Barcelona. The use of a control city (Valencia) and additional text features enhances the reliability of the results. Future research can explore the specific functions of metaphors and their influence on public perception and policy effectiveness.

### File Descriptions
scraping_nb.ipynb: Jupyter Notebook with the data scraping pipeline.
regression_analysis.R: R script with regression models and analysis.
summary_statistics.csv: Summary statistics of luxury and amenities features.
data/: Directory containing raw and processed data files.
figures/: Directory containing visualizations such as word clouds and correlation matrices.
Assignment1_NLP.pdf: Detailed project report.
