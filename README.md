# Carwash-Sales-Data-Audit

Excel data audit of a car wash business: cleaning customer and sales tables, removing duplicate records, reconciling $141.9K revenue, auditing discounts and benchmarking service times against standards.

## Sales Data Audit & Validation – Casey's Carwash

### Business problem
A car wash business needed its customer and sales records validated before using them for reporting. The task: clean and standardise the data, check that revenue and pricing were accurate, and find operational issues.

### Data
- **Customer Master:** 564 customer records (ID, name, location, membership, car size). After cleaning: **561 unique customers**.
- **Raw Records:** 1,184 sales transactions (date, service, car size, price, discount, service time, banking date). After cleaning: **1,181 transactions**.


### What I did

* Cleaned and standardised customer names, IDs and formats using text functions, lookups and IF logic.
* Tested data integrity by building unique customer and transaction IDs and checking for duplicates (3 duplicate customers and 3 duplicate transactions found and removed).
* Reconciled revenue: confirmed sales total matched the $141,900 revenue bookings using pivot tables, after removing the duplicate transactions.
* Audited pricing: recalculated every final price with the correct discount rules.
* Checked banking compliance against the first-working-day rule, allowing for public holidays.
* Benchmarked service times by car size against operating standards (±7.5% tolerance).

### Key findings

* 146 pricing mismatches: 57 members did not receive their discount and 88 non-members wrongly received it.
* 2 cash deposits were banked late without a public-holiday reason.
* 14.8% of customers hold a membership; 48.5% used the service only once, which points to a retention opportunity.
* Inner West is the biggest market (50.8% of customers); Southern Beaches is the smallest (5.7%).
* Southern Beaches grew most in average sale value from Q1 to Q4 (+$24.28); Eastern Suburbs fell most (−$7.68).
* Saturday had the highest sales volume (290 sales, $35.1K); Thursday had the highest average sale ($121.69).
* Only Superior–Small services deviated from standard by more than 7.5% (averaging 9.17% over), suggesting that time standard needs reviewing.

### Tools
Excel · pivot tables · XLOOKUP/VLOOKUP · IF logic · text functions · date/time functions

### Files

* `Carwash_sales_audit.xlsx` – cleaned data with all workings
* `Carwash_summary.pdf` – findings
*  [Carwash_summary.pdf](Project_Report.pdf) 
| [customer_data_clean.xlsx](customer_data_clean.xlsx) | Cleaned and aggregated datasets |
