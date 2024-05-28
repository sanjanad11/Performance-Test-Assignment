# Overview

This project involves conducting performance tests using Apache JMeter to evaluate the performance and reliability of the "E-Commerce" system. The tests are designed to measure various performance metrics, including response times, error rates, and throughput, to ensure the system can handle the expected load under different conditions. There are three modules(scenarios)
1. Purchase Product (Purchase_Order.jmx)
2. Search Product (Search_Products.jmx)
3. View My Orders (My_orders.jmx)


# Key Components
 Web Application:https://advantageonlineshopping.com/
 
 Test Tool: Apache JMeter 5.6.3
 Reason: Versatile, open-source, extensive 
 community support, and suitable for various 
 types of applications

 # Metrics Evaluated:
 1. APDEX (Application Performance Index)
 2. Response time
 3. Detailed Statistics
 4. Error Analysis

# Instructions to Run the Performance Tests

1. Open JMeter - Launch JMeter by executing the following command from the terminal: jmeter or alternatively, you can double-click the JMeter executable file
2. Load the Test Plan- In the JMeter GUI, go to File -> Open and select the Purchase_Order.jmx file
3. Run the Test- Click the green start button (▶) to begin the test.
4. After the test completes, generate the dashboard report by running the following command: jmeter -g results.jtl -o /path/to/dashboard-folder
5. Open the index.html file in the generated dashboard folder using a web browser to view the detailed performance test report.
