

\# Lab 5 – Static Code Analysis



\*\*Student ID:\*\* PES1UG24AM140



\*\*Project:\*\* Animal Shelter Adoption Register



\*\*File:\*\* pet\_shelter.py



\## Issues Identified and Fixed



| Issue | Tool | Original Finding | Fix Applied |

|---|---|---|---|

| Mutable default argument | Pylint | Shared default list in registerPet(). | Replaced \[] with None and initialized a new list. |

| Missing documentation | Pylint | Missing module and function docstrings. | Added appropriate docstrings. |

| Naming conventions | Pylint | Function names used camelCase. | Converted names to snake\_case. |

| Exception handling | Pylint | Bare and overly broad exception handling. | Removed unnecessary exception handling and checked database results explicitly. |

| Global statement | Pylint | Global adoption\_count was used. | Encapsulated database operations in a class. |

| SQL injection | Bandit B608 | SQL values were inserted using string formatting. | Used parameterized SQL queries. |

| Insecure random generation | Bandit B311 | Used random.randint() for adoption codes. | Replaced random with secrets. |

| Silent exception handling | Bandit B110 | Used try-except-pass. | Removed silent exception handling. |

| Long lines | Flake8 E501 | Lines exceeded 79 characters. | Reformatted long statements. |

| Bare except | Flake8 E722 | Used an unspecified exception handler. | Removed bare except. |

| Multiple statements | Flake8 E701 | Multiple statements appeared on one line. | Separated statements into individual lines. |



\## Conclusion



The original program was analyzed using Pylint, Bandit and Flake8. The identified code quality, security and formatting issues were corrected. All three tools were executed again to verify the improvements.



