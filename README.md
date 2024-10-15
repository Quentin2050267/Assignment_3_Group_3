# Assignment 3: Central Limit Order Book (CLOB) Implementation

During the class, we simulated OTC trading vs. exchange trading games. In the exchange trading game, all the orders submitted were matched using a central limit order book (CLOB). In this assignment, you will be required to implement a basic central limit order book (CLOB) for handling limit orders only. With the CLOB, you will simulate a simplified order book system where orders are matched based on price and time priority.

## Requirements and Evaluation (15%)

### Implementation
- Implement a central limit order book (CLOB) that only handles limit orders.
- Match incoming buy and sell orders according to price priority.
- Simulate the matching process and update the order book accordingly.
- Use the `orders.csv` provided for all the limit orders submitted.

---
### Load and describe the orders data (1%).

### The order book data should capture both buy and sell orders (2%).
- Buy orders should be sorted by descending price (highest bid first).
- Sell orders should be sorted by ascending price (lowest ask first).
- If two orders have the same price, the one that was placed earlier should have priority.

### Limit Order Matching
- When a new buy order is placed, it should be matched with the lowest-priced sell order if the sell price is less than or equal to the buy price (1%).
- When a new sell order is placed, it should be matched with the highest-priced buy order if the buy price is greater than or equal to the sell price (1%).
- If a full match is not possible, partially fill the order and leave the remaining quantity in the order book (1%).
---

### Order Book State
- After each order submission, print the updated order book showing the top buy and sell orders (1%).
- Implement a method to print the full order book for both bid and ask price levels with aggregated size for each level (2%).


### Trade Log
- Record the details of all trades matched with all the necessary information (2%).
---
### Spread and Market Depth
- **Bid-Ask Spread**
    - Calculate the bid-ask spread of the order book (1%).
- **Market Depth**
    - Calculate the dollar value of the average best level bid-ask market depth (1%).
- **Report and Documentation**
    - Report to describe the methodology and results (1%).
    - Documentation of code logic (1%).
---
## Deadline
- 23:59 hours, 26th Oct 2024.

## Submission Instructions
- Submit via Canvas by the deadline. Late submission will be penalized.
- Zip all files into one zip file with the naming format `Assignment_x_Group_x`. Group number should be the same as the project groups you are in on Canvas. No extra folder is needed inside the zip file.
- Python code should be executable and well documented. Both `.py` or `.ipynb` files are acceptable.
- Your report should document your methodology, analysis, and findings clearly and concisely, including all visualizations and statistical test results (if any). The report should be well formatted in A4 size PDF format with no more than 5 pages. In your report, please put all group members’ names and matric numbers.
