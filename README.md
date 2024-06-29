# Overview
This project focuses on analyzing historical exchange rates between Australian Dollar (AUD) and New Zealand Dollar (NZD) using data fetched from an external API. The main objectives include retrieving exchange rate data for the past 30 days, identifying the best and worst exchange rates within this period, and calculating the average exchange rate for the month.

# Approach
## Data Retrieval
Exchange rate data is fetched from the Exchange Rates API using Python's requests library. The get_past_exchange_data function handles the API interaction, retrieving daily exchange rates for the specified duration.

# Data Analysis
Finding Best and Worst Rates: The find_best_and_worst_rates function identifies the highest and lowest exchange rates from the fetched data.
Calculating Average Rate: The calculate_average_rate function computes the average exchange rate based on the fetched data.

# Error Handling
Error handling is implemented to manage potential issues such as missing data and API errors. Specific exceptions are caught and logged using Python's logging module to facilitate debugging and monitoring and displayed in on the standard output.

# Logging
Logging is integrated throughout the application to capture important events, errors, and informational messages. The logging.basicConfig function is utilized to configure logging settings such as log level, format, and output destinations (app.log file and console).

# Unit Testing
Unit tests are implemented using Python's unittest framework to ensure the correctness of functions:
- Data Integrity: Tests verify that the fetched data includes expected fields (date and rates).
- Functionality: Tests validate the behavior of functions like get_past_exchange_data, find_best_and_worst_rates, and calculate_average_rate under various scenarios, including normal operation and error conditions.
