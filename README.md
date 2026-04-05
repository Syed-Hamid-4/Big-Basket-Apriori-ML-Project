🛒 Big Basket: Market Basket Analysis & Supply Chain Optimization

📌 Project Overview

This project applies Association Rule Mining (Apriori Algorithm) to Big Basket customer transaction data to uncover hidden purchasing patterns. Rather than just suggesting "Frequently Bought Together" items for marketing, this analysis pivots the data to solve complex Supply Chain, Quick Commerce (10-min delivery), and Customer Experience (CX) challenges.

By shifting from traditional "category-based" warehousing to "affinity-based" operations, this project proposes data-driven strategies to reduce picking times, prevent recipe-breaking stockouts, and maximize Average Order Value (AOV).

🎯 Business Problems Addressed

Fulfillment Delays in Quick Commerce: Traditional warehouse slotting increases picker travel time, risking 10-minute delivery SLAs.

Cold-Chain Degradation: Mixing ambient and cold picking sequences reduces the freshness of premium items.

"Recipe-Breaking" Stockouts: If a core ingredient is out of stock, customers abandon the entire meal's basket.

In-Transit Damage: Heavy items packed with fragile items lead to high refund rates and poor CX.

🧠 Methodology & Tech Stack

Algorithm: Apriori (Association Rule Mining)

Metrics Evaluated: Support, Confidence, and Lift

Tech Stack: Python, Pandas, Apyori, Jupyter Notebook

Dataset: Big Basket.com Cart.csv (Customer transaction records containing 7,500+ unique baskets)

📊 Key Strategic Insights & Actions

1. "Immediate Consumption" Micro-Slotting

Data: Quick-prep items show intense correlations (e.g., Maggi + Pasta + Eggs + Mineral Water).

Action: Create fast-pick zones where these items are binned adjacent to each other.

Impact: Reduces picker travel paths by up to 30%, ensuring consistency in 10-minute delivery windows.

2. Synchronized Cold-Chain Picking

Data: High correlation exists within the "Premium Protein" cluster (Turkey + Salmon + Chicken + Eggs).

Action: Update WMS routing logic to sequence ambient/dry goods first, forcing pickers to gather cold-chain items at the absolute end of their route.

Impact: Minimizes time outside temperature control, guaranteeing peak freshness and driving down spoilage.

3. Recipe-Centric Inventory & Substitutes

Data: Customers buy distinct meal clusters (e.g., Spaghetti + Paneer + Knor).

Action: Link safety stocks in the ERP. If a "recipe-breaker" like Paneer is Out-Of-Stock, the app instantly prompts the picker with a highly-rated substitute (e.g., Tofu).

Impact: Saves the customer's dinner plan, reducing order cancellations and improving On-Time In-Full (OTIF) metrics.

4. End-of-Line "Impulse" Staging

Data: Items like Parle-G and Kinley are often isolated, single-item additions.

Action: Stage these items directly at the dispatch tables and enable a 60-second "Forgot Something?" prompt on the app post-checkout.

Impact: Captures last-minute revenue without requiring a picker to re-enter the aisles.

📂 Repository Structure

Big_Basket_Apriori_code.ipynb: The core Python notebook containing the Apriori model implementation and data processing.

Big Basket.com Cart.csv: The dataset used for the analysis.

Market-Basket-Analysis-Strategic-and-Supply-Chain-Insights.pdf: Executive presentation deck summarizing supply chain actions.

Big Basket Insights.pdf: Detailed analytical report of the identified clusters and business impact.
