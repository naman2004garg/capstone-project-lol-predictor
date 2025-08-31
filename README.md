# capstone-project-lol-predictor
Here is a concise checklist addressing all key criteria for your Capstone Project Peer Review. This will help your submission stand out and also guide your peer review process, aligned with the requested topics:

Capstone Peer Review Checklist
Unit Tests
API: There should be unit tests for all API endpoints, ideally using a Python test framework (pytest, unittest, etc.).

Model: The trained machine learning model should have tests for core logic—such as prediction accuracy and edge cases.

Logging: Logging functionality should be covered by unit tests to guarantee correct behavior (e.g., log message format, severity level).

Test Suite: All unit tests for API, model, and logging must be runnable via a single script (e.g., pytest, Makefile). Confirm all tests pass.

Monitoring & Isolation
Monitoring: There should be a mechanism (Prometheus, Grafana, ELK stack, or custom dashboards) to monitor API/model/log performance: track metrics like response time, error rate, and uptime.

Isolation: Read/write unit tests are isolated from production—achieved via mocking, using test databases, or environmental separation.

Functionality & Data Handling
API Function: The API should respond correctly for predictions for a specific country and for aggregate/global queries. Test with valid/invalid inputs for all scenarios.

Data Ingestion: Data ingestion is implemented as a reusable function or script, supporting automation and repeatable workflows.

Modeling & Comparison
Multiple Models: The project compares performance of multiple models (e.g., baseline logistic regression vs. advanced neural network), with results documented.

EDA Visualizations: The exploratory data analysis uses clear visualizations (matplotlib, seaborn, etc.) to show patterns, distributions, and relationships in the data.

Containerization & Visual Comparisons
Docker: All application components (API, model, tests, etc.) are packaged in a working Docker image. Provide a functioning Dockerfile and demonstrate running the solution in Docker.

Model Comparison Visualization: Model (and baseline) performance should be compared with visualizations—such as bar charts, ROC curves, or accuracy plots.
