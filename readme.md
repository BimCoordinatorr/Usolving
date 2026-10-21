
CodeLab — Code Quality Analyzer

An online coding workspace for writing, executing, and analyzing Python and Go code.

Launch CodeLab · View Repository · Report an Issue

Overview

CodeLab is a browser-based coding workspace that combines a code editor, online code execution, and a rule-based static analysis engine in one interface.

It helps developers and learners identify common coding issues, review code quality, and discover opportunities to improve readability, safety, and maintainability.

The application runs directly in your browser without requiring a local development environment.

Features
Code Editor: Write and edit Python 3 and Go source code.
Online Code Execution: Submit code to the Judge0 API and review execution output, compilation messages, and runtime errors.
Static Code Analysis: Detect selected coding patterns and potential issues using configurable rule-based checks.
Quality Score: Generate a heuristic score based on detected findings and their assigned penalties.
Quality Metrics: Review readability, safety indicators, and maintainability estimates.
Actionable Recommendations: Get suggestions for improving code structure, error handling, naming conventions, and more.
Project Management: Save and load project data using browser storage.
Coding Guidelines: Display language-specific coding rules and best practices.
Responsive Interface: Use the application on desktop and mobile devices.
No AI API Required: The built-in static analyzer uses predefined rules rather than an AI API.
Supported Languages
Language	Execution	Static Analysis
Python 3	Yes	Yes
Go	Yes	Yes
Getting Started
Use the Online Application
Open CodeLab.
Select Python 3 or Go from the language selector.
Enter your source code in the Code Editor.
Click Run Code to submit your program for execution.
Click Analyze Code to generate a code quality report.
Review the detected issues, quality metrics, and recommendations.
Use Save Project and Load Project to manage your work in the same browser.
Run Locally
Clone the repository:
git clone https://github.com/bimcoordinatorr/Usolving.git

Open the project directory:
cd Usolving

Open index.html in a modern web browser.

No package installation or build process is required for the basic application.

Technology Stack
HTML5 — Application structure.
CSS3 — Responsive layout and visual styling.
JavaScript — Code execution requests, static analysis, and browser-side project management.
Judge0 API — Online code execution service.
Local Storage — Browser-based project persistence.
Google Fonts (Inter) — Application typography.
GitHub Pages — Static website hosting.
Code Quality Analysis

The built-in analyzer performs heuristic, rule-based checks for selected patterns, including:

Long lines and trailing whitespace.
Unresolved TODO, FIXME, and XXX markers.
Potentially risky exception handling.
Dynamic code execution patterns in Python.
Mutable default arguments in Python.
Potentially ignored results and concurrency concerns in Go.
Repeated source lines and large code blocks.
Naming conventions and maintainability indicators.

The analyzer calculates a score starting at 100 and subtracts predefined penalties for detected findings.

Important: The score is a heuristic indicator, not a probability of correctness, a formal security assessment, or a performance benchmark. The analyzer does not understand every possible program behavior and may produce false positives or miss real issues. Always review its findings and test your code independently.

Execution and Privacy
Online execution depends on the availability of the Judge0 API and your network connection.
Code submitted through Run Code is sent to the configured execution service.
Project data saved using Save Project is stored in the browser's local storage.
Saved projects are not automatically synchronized across browsers or devices.
Clearing browser storage may remove saved project data.
Do not submit passwords, API keys, confidential source code, or other sensitive information unless you have reviewed the execution service's privacy and retention policies.
Project Structure
Usolving/
├── index.html
├── README.md
└── LICENSE

Limitations
Static analysis is based on predefined patterns and cannot guarantee correctness, security, or performance.
Online code execution requires a working Judge0 API endpoint.
Execution behavior may depend on service limits, language support, and standard-input configuration.
Project saving and loading depend on browser local storage.
The application does not currently provide server-side project synchronization or user accounts.
Contributing

Contributions, suggestions, and bug reports are welcome.

Fork the repository.
Create a branch for your changes.
Make and test your changes.
Open a pull request describing your improvements.

For bugs or feature requests, use the GitHub Issues page.

License

This project is licensed under the MIT License. See the LICENSE file for the full license text.

Acknowledgments
Judge0 for online code execution infrastructure.
GitHub Pages for hosting the application.
Google Fonts for the Inter typeface.

CodeLab — Online Code Runner · Code Quality Analyzer · Improvement Advisor
