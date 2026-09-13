ERROR: null value in column "email" of relation "club_members" violates not-null constraint

Failing row contains (7, Test, Student, null, Computer Science, 2026-09-10).

SQL state: 23502

Detail: Failing row contains (7, Test, Student, null, Computer Science, 2026-09-10).

Explanation

PostgreSQL rejected the row because the email column was defined with NOT NULL, so a student record must contain an email address.
## Reflection

The failed INSERT tests demonstrated how NOT NULL constraints protect the quality and completeness of the club_members table. When the first_name value was missing, PostgreSQL rejected the record because first_name was defined as NOT NULL. The same occurred when the email value was missing because email was also defined as NOT NULL.

These tests showed that database constraints help prevent incomplete records from being stored. The error messages clearly identified which column violated the constraint and explained why the INSERT statement failed. This confirms that the table was designed correctly according to the assignment requirements.
