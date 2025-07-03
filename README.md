# Kultra-Mega-Stores-Inventory
Kultra Mega Stores (KMS), headquartered in Lagos, specialises in office supplies and furniture. Its customer base includes individual consumers, small businesses (retail), and large corporate clients (wholesale) across Lagos, Nigeria.
🔍 Case Scenario 1: Operational Sales Analysis
1. Which product category had the highest sales?
2.
3.  using SQL:

SELECT "Product Category", SUM(Sales) AS Total_Sales
FROM orders
GROUP BY "Product Category"
ORDER BY Total_Sales DESC
LIMIT 1; 
The product category with the highest total sales isTechnology with a Total Sales of ₹5,984,248.18

Question 2: Top & Bottom Regions by Sales
Top 3 Regions:

West — ₹3,597,549

Ontario — ₹3,063,212

Prarie — ₹2,837,305

Bottom 3 Regions:

Yukon — ₹975,867

Northwest Territories — ₹800,847

Nunavut — ₹116,376

These results show significant sales disparities across regions

Question 3: Total Sales of Appliances in Ontario
Total Sales: ₹0.00
According to the dataset, no appliance sales were recorded in the Ontario region between 2009–2012.

Question 4: Bottom 10 Customers by Sales
Here are the customers with the lowest total sales from 2009 to 2012:

Customer Name	Total Sales (₹)
Jeremy Farry	85.72
Natalie DeCherney	125.90
Nicole Fjeld	153.03
Katrina Edelman	180.76
Dorothy Dickinson	198.08
Christine Kargatis	293.22
Eric Murdock	343.33
Chris McAfee	350.18
Rick Huthwaite	415.82
Mark Hamilton	450.99

Recommendation to Increase Revenue:
Customer Segmentation & Profiling
Understand why these customers bought so little: were they new? one-time buyers? Is there a pattern in their industry or region?

Reactivation Campaigns
Send personalized offers, discounts, or loyalty incentives to these customers based on products they previously viewed or purchased.

Bundle Upgrades
Promote value bundles that include higher-margin items — may encourage larger purchases.

Feedback Loop
Reach out via surveys to discover pain points or missed expectations that might have hindered their buying activity.

Sales Rep Targeting
Assign sales teams to re-engage these accounts with tailored product suggestions.

Question 5: Shipping Method with the Highest Cost
Shipping Method: Delivery Truck
Total Shipping Cost: ₹51,971.94

Insight: The Delivery Truck method, while potentially more economical per unit, incurred the highest total shipping expense — possibly due to bulk or frequent usage.

-------CASE SCENARIO II

Question 6: Most Valuable Customers & Their Typical Purchases
Top 5 customers by total sales:

Customer Name	Total Sales (₹)
Emily Phan	₹117,124.44
Deborah Brumfield	₹97,433.14
Roy Skaria	₹92,542.15
Sylvia Foulston	₹88,875.76
Grant Carroll	₹88,417.00

What They Buy:
Customer	Top Category	Major Purchase Focus
Emily Phan	Technology (₹110K+)	Heavy tech investment
Deborah Brumfield	Technology	Mainly tech products
Roy Skaria	Furniture	High-value office setups
Sylvia Foulston	Furniture	Large furniture orders
Grant Carroll	Office Supplies	Bulk office consumables

The most valuable customers are predominantly engaged in technology and furniture purchases, suggesting a strong demand for office setups and IT infrastructure.

Question 7: Top Small Business Customer by Sales
Customer Name: Dennis Kane
Total Sales: ₹75,967.59

Dennis Kane is the highest-spending customer in the Small Business segment over the 2009–2012 period.

Question 8: Corporate Customer with Most Orders
Customer Name: Roy Skaria
Total Orders Placed (2009–2012): 18

Roy Skaria is the most active Corporate segment customer in terms of order volume.

Question 9: Most Profitable Consumer Customer
Customer Name: Emily Phan
Total Profit Generated: ₹34,005.44

Insight: Emily Phan not only tops sales but also delivers the highest profit among all Consumer segment customers — a prime candidate for loyalty programs or premium services.

Question 10: Returned Items & Customer Segment

The dataset does not contain a direct indicator for returns
Insight: Based on the provided data, we cannot determine which customers returned items

Question 11: Was Shipping Cost Appropriately Spent Based on Order Priority?
Let’s evaluate the logic:

Order Priority	Shipping Method	Total Shipping Cost (₹)
Critical	
Delivery Truck	₹10,784
Regular Air	₹8,587
Express Air	₹1,742

High
Delivery Truck	₹11,207
Regular Air	₹10,005
Express Air	₹1,454

Low	
Delivery Truck	₹11,132
Regular Air	₹10,264
Express Air	₹1,552

Medium	
Delivery Truck	₹9,462
Regular Air	₹9,419
Express Air	₹1,634

Not Specified	
Regular Air	₹9,734
Delivery Truck	₹9,388
Express Air	₹1,470

Interpretation:
Critical orders were mostly shipped via Delivery Truck and Regular Air, with very little Express Air use.

Express Air, the most expensive method, was least used, even for critical/high priority — which is cost-efficient, but potentially risky for delays.

Delivery Truck, the most used and most expensive cumulatively, was heavily used even for Low and Medium priority.

Conclusion:
Shipping cost does not align well with order priority:

High-priority orders should use Express Air more, despite the cost.

Low-priority orders still incurred high delivery truck costs — an inefficiency.

Recommendation:
Recalibrate shipping policy to ensure:

- Express Air for Critical/High priority orders when speed is essential.

- Delivery Truck/Regular Air reserved for Low/Medium orders to minimize cost

- ![image](https://github.com/user-attachments/assets/b9985910-3883-4c5e-b234-d8545e2b97a9)
