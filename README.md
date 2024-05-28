Overview
This project involves conducting performance tests using Apache JMeter to evaluate the performance and reliability of the "E-Commerce" system. The tests are designed to measure various performance metrics, including response times, error rates, and throughput, to ensure the system can handle the expected load under different conditions.

Key Components
Source File: Results_Purchase_Order.csv
Test Tools: Apache JMeter, Apache JMeter Dashboard
Metrics Evaluated:
APDEX (Application Performance Index)
Request Summary
Detailed Statistics
Error Analysis
Top 5 Errors by Sampler
Instructions to Run the Performance Tests
Prerequisites
Ensure you have the following software installed on your system:

Apache JMeter: Download and Installation Guide
Java Runtime Environment (JRE): JMeter requires JRE to run. Make sure JRE is installed and configured properly.
Web Browser: To view the generated dashboard report.
Setup
Clone the Repository

sh
Copy code
git clone https://github.com/your-repo/performance-test.git
cd performance-test
Place the Test Plan
Ensure the JMeter test plan (.jmx file) is placed in the root directory of the project. For example:

Copy code
performance-test/
├── Purchase_Order_Test_Plan.jmx
└── README.md
Place the Source File
Ensure the source file Results_Purchase_Order.csv is placed in the appropriate directory if required by the test plan.

Running the Tests
Open JMeter
Launch JMeter by executing the following command from the terminal:

sh
Copy code
jmeter
Alternatively, you can double-click the JMeter executable file.

Load the Test Plan

In the JMeter GUI, go to File -> Open and select the Purchase_Order_Test_Plan.jmx file.
Configure Test Parameters

Adjust the number of threads (users), ramp-up period, and loop count as per your testing requirements in the Thread Group section of the test plan.
Run the Test

Click the green start button (▶) to begin the test.
Generating and Viewing the Report
Generate the Dashboard Report
After the test completes, generate the dashboard report by running the following command:

sh
Copy code
jmeter -g results.jtl -o /path/to/dashboard-folder
results.jtl: The JTL file containing the results of the test.
/path/to/dashboard-folder: The directory where the dashboard report will be generated.
View the Report

Open the index.html file in the generated dashboard folder using a web browser to view the detailed performance test report.
