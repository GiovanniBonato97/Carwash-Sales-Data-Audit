# Carwash-Sales-Data-Audit
Excel data audit of a car wash business: cleaning customer and sales tables, reconciling $141.9K revenue, auditing discounts and benchmarking service times against standards.

# Sales Data Audit & Validation – Casey's Carwash

## Business problem
A car wash business needed its customer and sales records validated before using them for reporting. The task: clean and standardise the data, check that revenue and pricing were accurate, and find operational issues.

## Data
- **Customer Master:** 564 customers (ID, name, location, membership).
- **Raw Records:** 1,100+ sales transactions (date, service, car size, price, discount, service time, banking date).

## What I did
- **Cleaned and standardised** customer names, IDs and formats using text functions, lookups and IF logic.
- **Tested data integrity** by building unique customer and transaction IDs and checking for duplicates (none found).
- **Reconciled revenue:** confirmed sales total matched the $141,900 revenue bookings using pivot tables.
- **Audited pricing:** recalculated every final price with the correct discount rules.
- **Checked banking compliance** against the first-working-day rule, allowing for public holidays.
- **Benchmarked service times** by car size against operating standards (±7.5% tolerance).

## Key findings
- **147 pricing mismatches:** 58 members did not receive their discount and 88 non-members wrongly received it.
- **2 cash deposits** were banked late without a public-holiday reason.
- **14.9%** of customers hold a membership; **48.9%** used the service only once, which points to a retention opportunity.
- **Inner West** is the biggest market (51% of customers); **Hills District** is the smallest (5.9%).
- **Eastern Suburbs** grew most in average sale value from Q1 to Q4 (+$12.88); **Southern Beaches** fell most (−$13.99).
- **Saturday** had the highest total revenue ($35.1K); **Thursday** had the highest average sale ($121.69).
- Many services finished more than 7.5% faster than standard, suggesting the time standards need reviewing.

## Tools
Excel · pivot tables · XLOOKUP/VLOOKUP · IF logic · text functions · date/time functions

## Files
- `carwash_audit.xlsx` – cleaned data with all workings
- `summary.pdf` – findings
