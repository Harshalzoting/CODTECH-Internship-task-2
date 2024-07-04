Name: HARSHAL ZOTING

Company: CODTECCH IT SOLUTIONS

ID:CT08DS2364

Domain: CYBER SECURITY & ETHICAL HACKING

Duration:June to July 2024


Overview of the Vulnerability Scanning Tool
This Python-based vulnerability scanning tool is designed to perform basic security checks on a network or website. It scans for common security vulnerabilities, including open ports, outdated software versions, and misconfigurations. The tool leverages Python's standard libraries and a few additional ones to provide a simple yet effective way to identify potential security issues.

Key Features
Port Scanning:
The tool scans a list of common ports on a specified host to check if they are open. Open ports can indicate potential entry points for attackers.

Outdated Software Check:
It checks the versions of commonly used software (e.g., Python, Node.js, Nginx) on the system. Running outdated software can expose the system to known vulnerabilities.

Website Security Check:
The tool examines the HTTP response headers of a specified website for essential security headers. Missing or misconfigured headers can lead to various security issues such as cross-site scripting (XSS) and clickjacking.

How It Works

Port Scanning:
The scan_open_ports function uses Python's socket library to attempt connections to a list of predefined ports on the target host. If a connection is successful, the port is marked as open.

Outdated Software Check:
The check_outdated_software function runs system commands to get the versions of specified software using Python's subprocess module. It checks for the presence of software and retrieves their versions if installed.

Website Security Check:
The check_website_security function sends an HTTP GET request to the specified URL using the requests library. It then checks the response headers for the presence of common security headers.

Usage
When you run the script, it prompts you to enter the target host (e.g., a domain name or IP address).
It then scans the target for open ports, checks for outdated software, and examines the website's security headers.
The results are displayed on the console, providing a quick overview of potential security issues.
