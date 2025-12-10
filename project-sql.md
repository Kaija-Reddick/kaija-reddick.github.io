# SQL Log Filtering for Threat Detection

## 🎯 Objective
Use SQL queries to filter and analyze security-related events from a log dataset in order to identify potential Indicators of Compromise (IoCs).

## 🧰 Tools & Technologies
- SQL
- Security event/log dataset (from Google Cybersecurity course)
- Spreadsheet or database environment

## 🧠 Skills Demonstrated
- Writing SQL queries with `WHERE`, `AND`, `OR`, and `LIKE`
- Filtering large log datasets efficiently
- Identifying suspicious IPs, users, or activities
- Supporting investigations with data-driven evidence

## 🔍 What I Did
- Reviewed a dataset of security-related events (logins, access attempts, etc.).
- Wrote SQL queries to:
  - Filter failed login attempts
  - Isolate unusual access times
  - Identify repeated attempts from the same IP or user
  - Identify attempts from outside specified area
- Highlighted events that could indicate brute-force attempts or unauthorized access.

## 📈 Example SQL Pattern
```sql
SELECT *
FROM login_in_attempts
WHERE login_time > '18:00' AND success = FALSE


  
