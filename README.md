# Hotel Booking Cancellation Analysis

## 1. Executive Summary
In recent years, the hospitality industry, specifically City Hotels and Resort Hotels, has experienced unusually high booking cancellation rates. These cancellations lead to suboptimal room utilization and a direct reduction in realized revenue. The primary objective of this data analysis project is to identify the key factors driving these cancellations and to provide actionable, data-driven recommendations to help hotel management mitigate losses and optimize revenue generation.

## 2. Business Problem
High cancellation rates result in vacant rooms and reduced profitability. By analyzing historical booking data, this project aims to understand the underlying causes of cancellations and evaluate pricing and promotional strategies that can improve booking retention.

## 3. Tech Stack
* **Language:** Python
* **Libraries:** Pandas, Matplotlib, Seaborn
* **Environment:** Jupyter Notebook

## 4. Data Assumptions
To ensure the integrity of this analysis, the following assumptions were made:
* The dataset provided (spanning 2015-2017) is a stable representation of general booking trends without massive external anomalies.
* Insights derived from this historical data remain applicable to current hotel strategic planning.
* Implementing suggested pricing and promotional strategies will not yield unanticipated negative consequences for the hotels.
* The hotels are not currently actively utilizing the exact optimization solutions proposed in this report.
* Booking cancellations remain the most significant controllable factor affecting income generation.
* A canceled booking directly equates to a vacant room for the initially requested duration.

## 5. Research Questions & Hypotheses
**Research Questions:**
1. What are the primary variables that influence hotel reservation cancellations?
2. How can hotel management proactively reduce the volume of cancellations?
3. How can pricing and promotional decisions be optimized based on cancellation trends?

**Initial Hypotheses:**
1. Higher accommodation prices directly correlate with higher cancellation rates.
2. Extended waiting lists contribute to increased customer cancellations.
3. The majority of booking cancellations originate from offline travel agents.

## 6. Analysis and Key Findings

**Overall Cancellation Rates**
Initial exploratory data analysis shows a significant cancellation rate overall. Approximately 37% of total reservations in the dataset were canceled, representing a substantial loss in potential earnings.

**Segment Comparison: City Hotel vs. Resort Hotel**
The data indicates that City Hotels handle a higher total volume of bookings compared to Resort Hotels. Consequently, the absolute number of cancellations is also higher for City Hotels.

**Pricing Trends (Average Daily Rate)**
An analysis of the Average Daily Rate (ADR) reveals fluctuations throughout the year. On several days, the ADR for City Hotels is noticeably lower than that of Resort Hotels. Resort hotel pricing spikes significantly, likely corresponding with weekends and holiday seasons.

**Seasonality of Bookings and Cancellations**
When grouped by month, August records the highest absolute volume of both confirmed and canceled reservations. Furthermore, an analysis of pricing (ADR) across the year demonstrates that cancellations are highly sensitive to price peaks.

**Geographic Distribution of Cancellations**
Portugal (PRT) accounts for the vast majority of canceled reservations, representing approximately 70% of the cancellations among the top 10 countries analyzed.

**Market Segment Analysis**
Contrary to the initial hypothesis that offline travel agents drive cancellations, the data shows that approximately 47% of all clients originate from Online Travel Agencies (OTAs), followed by Groups (27%). Only about 4% of clients book directly.

**Price vs. Cancellation Correlation**
Time-series analysis clearly visualizes that reservations are more frequently canceled when the Average Daily Rate is high. This definitively validates the hypothesis: higher pricing leads to higher cancellation rates.

## 7. Strategic Recommendations
Based on the data analysis, the following actionable strategies are recommended to management:

1. **Dynamic Pricing Strategy:** Since cancellation rates rise in tandem with pricing, hotels should evaluate their dynamic pricing algorithms. Offering slightly lower, non-refundable rates for specific high-risk locations can lock in revenue and prevent last-minute cancellations.
2. **Weekend and Holiday Promotions:** Resort hotels experience a higher ratio of cancellations compared to City Hotels, particularly when their prices peak. Implementing targeted, reasonable discounts on room prices for weekends and holidays can incentivize booking retention.
3. **Targeted Seasonal Campaigns:** In months exhibiting high cancellation rates alongside high pricing (such as January), management should launch proactive marketing campaigns. Offering value-adds (e.g., complimentary breakfast, spa credits) rather than just price drops can help maintain the ADR while reducing the incentive to cancel.
4. **Geographic Quality Control:** With Portugal exhibiting an overwhelming 70% cancellation rate within the top 10 segment, targeted efforts must be made for this demographic. Management should investigate the specific root causes for cancellations from Portugal and consider improving localized marketing, tailored services, or adjusting deposit policies specifically for this region.

## 8. How to Run the Project
1. Clone this repository to your local machine.
2. Ensure you have Python installed, along with Jupyter Notebook, Pandas, Matplotlib, and Seaborn.
3. Place the `hotel_bookings 2.csv` file in the same directory as the notebook.
4. Dataset link: https://drive.google.com/file/d/1-QwW.
5. Open `Hotel_booking_code.ipynb` in Jupyter Notebook and run the cells sequentially.
