ERROR: null value in column "email" of relation "club_members" violates not-null constraint

Failing row contains (7, Test, Student, null, Computer Science, 2026-09-10).

SQL state: 23502

Detail: Failing row contains (7, Test, Student, null, Computer Science, 2026-09-10).

Explanation

PostgreSQL rejected the row because the email column was defined with NOT NULL, so a student record must contain an email address.
