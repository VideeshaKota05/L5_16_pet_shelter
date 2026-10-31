
# Lab 5 – Static Code Analysis

**Student ID:** PES1UG24AM140

**Project:** Animal Shelter Adoption Register

**File:** pet_shelter.py

## Issues Identified and Fixed

| Issue | Tool | Original Finding | Fix Applied |
|---|---|---|---|
| Mutable default argument | Pylint | Shared default list in registerPet(). | Replaced [] with None. |
| Missing documentation | Pylint | Missing module and function docstrings. | Added docstrings. |
| Naming conventions | Pylint | Function names used camelCase. | Changed to snake_case. |
| Global statement | Pylint | Used global adoption_count. | Encapsulated functionality in a class. |
| Exception handling | Pylint | Bare and broad exception handling. | Removed unnecessary exception handling. |
| SQL injection | Bandit B608 | SQL values inserted using string formatting. | Used parameterized SQL queries. |
| Insecure random generation | Bandit B311 | Used random.randint(). | Replaced random with secrets. |
| Silent exception handling | Bandit B110 | Used try-except-pass. | Removed silent exception handling. |
| Long lines | Flake8 E501 | Lines exceeded 79 characters. | Reformatted long lines. |
| Bare except | Flake8 E722 | Used unspecified exception handler. | Removed bare except. |
| Multiple statements | Flake8 E701 | Multiple statements on one line. | Separated statements. |

## Conclusion

The original program was analyzed using Pylint, Bandit and Flake8. The identified code quality, security and formatting issues were corrected and the tools were executed again to verify the improvements.
