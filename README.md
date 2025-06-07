# Airbnb-Listing-Analysis
#### DOMAIN : Travel & Hospitality
## Project Overview

The project explores Airbnb data from Paris to:
- Understand listing prices across neighborhoods
- Investigate the impact of regulatory changes in 2015
- Analyze host trends over time
- Examine how accommodation size affects pricing

#### DATA OVERVIEW:
For this analysis, we utilized the Comprehensive dataset of - <a href="https://github.com/siva151988/Airbnb-Listing-Analysis/blob/main/Listings.zip">Listings.csv</a>

#### DATA DICTIONARY:
| Column Name           | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| `id`                  | Unique identifier for the listing                                           |
| `name`                | Title of the listing                                                        |
| `host_id`             | Unique identifier for the host                                              |
| `host_since`          | Date when the host started listing                                          |
| `neighbourhood`       | Name of the neighborhood/area                                               |
| `room_type`           | Type of accommodation (Entire home, Private room, Shared room)             |
| `price`               | Price per night in USD or EUR                                               |
| `minimum_nights`      | Minimum number of nights per booking                                        |
| `availability_365`    | Number of days available in a year                                          |
| `number_of_reviews`   | Total number of reviews received                                            |
| `last_review`         | Date of the most recent review                                              |
| `reviews_per_month`   | Average number of reviews per month                                         |
| `calculated_host_listings_count` | Number of listings the host has in total                        |


### Data Cleaning Insights
- **Missing Values:**  
  - Some listings have missing values.These missing review data points were handled by either imputing with zero (assuming no reviews) or filtering out during analysis based on the context.

- **Date Formatting:**  
  - The columns `host_since` were initially stored as strings and needed conversion to datetime format to allow time series and duration analysis.
    
- **Outlier Detection:**  
  - Price data contained extreme outliers with very high nightly prices. These were flagged for further investigation or removal to avoid skewing analysis.

### 📈 EDA Insights
- **Listings Distribution**:  
  - Certain neighborhoods had a higher density of listings, indicating popular tourist zones.

- **Room Type Trends**:  
  - Entire homes dominate the market, followed by private rooms.
   
- **Decline in New Hosts After 2015**  
  A significant drop in the number of new hosts was observed starting in 2015. This suggests that regulatory measures (such as zoning laws, host registration, or tax enforcement) may have discouraged new entries into the short-term rental market.

## 🔍 Key Highlights

### 🟢 1. **Impact of Regulations**
- In **2015**, Paris implemented stricter short-term rental laws.
- **Result**: 
  - **Fewer new hosts** joining after 2015.
  - **Sharp increase in average prices** post-2015.

### 🟢 2. **Price by Accommodation Capacity**
- Listings that accommodate **more guests** tend to charge **higher prices**.
- Clear linear correlation between accommodation size and price.

### 🟢 3. **Price by Neighborhood**
- Premium neighborhoods like **Elysee, Bourse, Louvre** have **higher average prices**.
- Budget areas include **Menilmontant, Gobelins**, and **Reuilly**.
  ![screenshot1](https://github.com/user-attachments/assets/38a9887f-2d2d-452e-91af-8105df430370)
  ![screenshot2](https://github.com/user-attachments/assets/294ec6ed-0082-4e85-8c3d-26f0755998a6)
  ![screenshot3](https://github.com/user-attachments/assets/91f20d66-0466-480d-8b84-cc6c951213c0)



