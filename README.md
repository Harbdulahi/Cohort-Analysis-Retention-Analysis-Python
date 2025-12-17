# Cohort Analysis (Customer Retention)
The objective of this analysis is to check if our retention efforts are working and what percentage of customers keep coming back month after month.

## Dataset And Data Dictionary:
This dataset is from UCI (retail dataset), containing:

*Columns*

1. InvoiceNo: Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction. If this code starts with the letter 'c', it indicates a cancellation. 
2. StockCode: Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product.
3. Description: Product (item) name. Nominal.
4. Quantity: The quantities of each product (item) per transaction. Numeric.	
5. InvoiceDate: Invoice Date and time. Numeric, the day and time when each transaction was generated.
6. UnitPrice: Unit price. Numeric, Product price per unit in sterling.
7. CustomerID: Customer number. Nominal, a 5-digit integral number uniquely assigned to each customer.
8. Country: Country name. Nominal, the name of the country where each customer resides.

And spans between 01/12/2010 and 09/12/2011 (13 months) for a UK-based, registered non-store online retail.

### Tools And Libraries

- Python
- Jupyter Notebook (VsCode)
- Pandas (Data Analysis Library)
- Matplotlib And Seaborn (Visualization)

### WorkFlow
**Data Cleaning And Exploration** (Not EDA)
- Importing libraries
- Dropped unnecessary columns (needed Invoice Date and Customer ID)
- Dropped duplicated and Null records
- Extract Invoice Month
- Create customer Cohort Month (first purchase month)
- Subtract Invoice Month from Cohort Month to create Activity Month Columns
- Grouped Cohort, Activity Month, and extracted each customer ID count (nunique()) in each grouped month
- Plot Heat Map to get customer count in each cohort and track counts (retention) across activity months

![Cohort Heatmap](https://github.com/Harbdulahi/Cohort-Analysis-Retention-Analysis-Python/blob/main/cohort/Cohort_in.png?raw=true)


### Insight 
- Our December 2010 cohort (948), on average, **31%** of them keep coming back across the 13 months (December 2010 - December 2011)
- January cohort (421), on average, **23%** of them keep coming back across the 12 months (January 2011 - December 2011)
- February cohort (380), on average, **22%** of them keep coming back across the 11 months (February 2011 - December 2011)
- March cohort (440) on average, **21%** of them keep coming back across the 10 months (March 2011 - December 2011)
- April cohort (299) on average, **18%** of them keep coming back across the 9 months (April 2011 - December 2011)
- May cohort (279) on average, **20%** of them keep coming back across the 8 months (May 2011 - December 2011)
- June cohort (235) on average, **19%** of them keep coming back across the 7 months (June 2011 - December 2011)
- July cohort (191) on average, **17%** of them keep coming back across the 6 months (July 2011 - December 2011)
- August cohort (167) on average, **22%** of them keep coming back across the 5 months (August 2011 - December 2011)
- September cohort (298) on average, **25%** of them keep coming back across the 4 months (September 2011 - December 2011)
- October cohort (352) on average, **23%** of them keep coming back across the 3 months (October 2011 - December 2011)
- November cohort (321) on average, **19%** of them keep coming back across the 2 months (November 2011 - December 2011)
- December cohort (41) on average, **100%** of them appear in that 1 month (December 2011)


### Recommendation

To keep retaining customers, send promotional messages, offer discounts, and give early access to top customers, or best create a loyalty program

[Cohort Analysis Video](https://youtu.be/fP4MhYzsaRY?si=fMmuEE1r6Vi2I6Ku)
