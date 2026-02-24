Amazon Product Performance Analysis (Power BI)
Project Overview
This project analyzes Amazon product data to uncover insights about pricing, discounts, ratings, and category
performance using Power BI.

Data Cleaning (Power Query)
• Removed currency symbols and converted price columns to decimal.
• Cleaned discount percentage values.
• Replaced null ratings with 0.
• Split category column into main and subcategories.
• Removed duplicate products using product ID and name.

DAX Measures
Total Products = COUNTROWS(amazon)
Avg Rating = AVERAGE(amazon[rating])
Avg Discount = AVERAGE(amazon[discount_percentage])
Discount Amount = SUMX(amazon, actual_price - discounted_price)
Revenue Potential = SUMX(amazon, discounted_price * rating_count)

Dashboard Components
• KPI Cards: Total Products, Avg Rating, Avg Discount
• Category Product Distribution
• Rating Distribution Histogram
• Discount vs Rating Scatter Plot
• Product Performance Table

Key Business Insights
• Electronics has the highest product volume, showing strong competition.
• Higher discounts do not always lead to higher ratings.
• Some categories rely on aggressive discounting strategies.
• Quality impacts ratings more than pricing in many cases.
• High rating-count products drive revenue potential.
• Electronics has mixed quality despite large inventory.

Author: Sairaju Bathula
