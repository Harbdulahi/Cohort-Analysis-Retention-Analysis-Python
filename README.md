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

And spans between 01/12/2010 and 09/12/2011 (13 months) for a UK-based and registered non-store online retail.

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

### Insight 
- Our December 2010 cohort (948), on average, **31%** of them keep coming back across the 13 months (December 2010 - December 2011)
- January cohort (421), on average, **23%** of them keep coming back across the 12 months (January 2011 - December 2011)
- February cohort (380), on average, **23%** of them keep coming back across the 12 months (February 2011 - December 2011)
- March on average, **23%** of them keep coming back across the 12 months (March 2011 - December 2011)
- April on average, **23%** of them keep coming back across the 12 months (April 2011 - December 2011)
- May on average, **23%** of them keep coming back across the 12 months (May 2011 - December 2011)
- June on average, **23%** of them keep coming back across the 12 months (June 2011 - December 2011)
- July on average, **23%** of them keep coming back across the 12 months (July 2011 - December 2011)
- August on average, **23%** of them keep coming back across the 12 months (August 2011 - December 2011)
- September on average, **23%** of them keep coming back across the 12 months (September 2011 - December 2011)
- October on average, **23%** of them keep coming back across the 12 months (October 2011 - December 2011)
- November on average, **23%** of them keep coming back across the 12 months (November 2011 - December 2011)
- December on average, **23%** of them keep coming back across the 12 months (December 2011)
