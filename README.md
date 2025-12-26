# Retail Revenue Recovery: VIP Ghost Analysis 

I analyzed a massive sales dataset to identify "Ghost VIPs" high value customers who haven't returned in over 2 months. By isolating these customers, we can quantify the revenue at risk and deploy targeted strategies, such as a 10% discount offer, to win them back.

## Project Overview
This project focuses on identifying "at-risk" high-value customers for an online retail business. Using a dataset of over 500,000 transactions, I performed an RFM (Recency, Frequency, Monetary) analysis to pinpoint VIP customers who have stopped purchasing.

## Business Impact
* **the Identified Revenue at Risk was** A whopping **£144,530.82**. Identifying this "leaky bucket" allows the business to prioritize high-value retention.
* **Target Segment:** Identified **14 VIP "Ghost" Customers** (Spent >£1,000, Inactive >60 days).
* **Strategic Outcome:** Generated a targeted list of lapsed VIPs and their favorite products to drive data-led re-engagement campaigns.

## Technical Workflow
1. **Data Sanitization:** - Handled 130,000+ missing Customer IDs.
   - Filtered out cancellations and returns to isolate "Net Sales."
2. **Feature Engineering:** - Engineered a `TotalSpend` metric per customer.
   - Converted date strings to `datetime` objects and calculated `DaysSinceLastPurchase`.
3. **Advanced Segmentation:** - Utilized Boolean Indexing and `.isin()` filters to map VIP IDs back to product history.

## Key Skills Demonstrated
- Python (Pandas & NumPy)
- Data Cleaning & Pre processing
- Customer Segmentation (RFM Logic)
- Business Intelligence & Revenue Projection
