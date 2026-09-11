# PostgreSQL Data Type Selection Exercise

| # | Column | PostgreSQL Data Type | Justification |
|---|--------|----------------------|---------------|
| 1 | student_id | BIGINT GENERATED ALWAYS AS IDENTITY | BIGINT provides a large range of numbers, and IDENTITY automatically generates increasing values for each student. |
| 2 | first_name | VARCHAR(50) | VARCHAR(50) is appropriate because most student first names are fewer than 50 characters. |
| 3 | email_address | VARCHAR(255) | VARCHAR(255) is appropriate for storing email addresses because email addresses are variable-length text values. |
| 4 | date_of_birth | DATE | DATE stores the student's birth date without unnecessary time-of-day information. |
| 5 | account_balance | NUMERIC(10,2) | NUMERIC(10,2) stores monetary values accurately with two decimal places for cents. |
| 6 | is_active | BOOLEAN | BOOLEAN is appropriate because the column has only two possible states, true or false. |
| 7 | event_start | TIMESTAMPTZ | TIMESTAMPTZ stores an exact date and time while accounting for time-zone information. |
| 8 | event_description | TEXT | TEXT is appropriate because descriptions can contain several paragraphs and have no fixed maximum length. |
| 9 | maximum_attendees | INTEGER | INTEGER is appropriate for storing the whole-number maximum number of attendees. |
| 10 | student_attended | BOOLEAN | BOOLEAN is appropriate because attendance has only two possible values, yes or no. |
| 11 | phone_number | VARCHAR(25) | VARCHAR(25) is appropriate because phone numbers may contain digits, spaces, parentheses, plus signs, and hyphens. |
| 12 | postal_code | VARCHAR(10) | VARCHAR(10) is appropriate because postal codes can contain leading zeros and other characters. |
| 13 | event_status | VARCHAR(20) | VARCHAR(20) allows the system to store current statuses and add additional statuses later. |
| 14 | student_number | VARCHAR(10) | VARCHAR(10) preserves leading zeros in student numbers such as 001245. |
