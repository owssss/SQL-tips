# SQL-tips (postgreSQL or MySQL)
You may find these tips too basic. but these tips are for me, and I discovered these while doing some projects


# DATE & TIME
## Group by day,month,Year
✅ Always use ```DATE(timestamp)``` when grouping time-based data per day.  ( This ensures that groups are correctly calculated on a daily basis!)  
✅ use ```DATE_TRUNC('month', timestamp)``` when grouping by month. (truncates the timestamp to the first day of the month while keeping the year.)
✅ use ```DATE_TRUNC('year', timestamp)``` This truncates the timestamp to the first day of the year (January 1st) while keeping the year.

## Good to know 
✅ Use ```DATE_TRUNC('year', timestamp)``` for grouping by year
✅ Use ```EXTRACT(YEAR FROM timestamp)``` if you only need the numeric year 
