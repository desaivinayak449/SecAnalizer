SecAnalyzer Pro

AI-Powered Red Team Security Suite for authorized penetration testing and security research.




Overview

SecAnalyzer Pro is a terminal-based offensive security and reconnaissance framework designed for penetration testers, bug bounty hunters, and cybersecurity researchers.

The toolkit combines:

Automated reconnaissance
Web application security testing
Infrastructure scanning
AI-powered security analysis
Reporting and export utilities
Cloud asset enumeration
JWT and authentication testing

The project uses a Rich-powered terminal UI and integrates AI-assisted vulnerability analysis using Google Gemini.

Features
Reconnaissance
WHOIS lookup
DNS enumeration
Subdomain discovery
ASN intelligence gathering
Cloud bucket reconnaissance
Endpoint discovery
JavaScript URL extraction
Web Application Testing
Security header analysis
CORS misconfiguration detection
CSP analysis
Clickjacking checks
Open redirect testing
XSS pattern analysis
Sensitive file discovery
Common vulnerability checks
Exploitation & Assessment Modules
SQL Injection testing
SSRF detection
XXE analysis
SSTI testing
File upload checks
IDOR testing
JWT inspection and decoding
Cookie security analysis
Rate-limit testing
Infrastructure Security
Large-scale port scanning
SSL/TLS auditing
CVE mapping
Nmap integration
Service fingerprinting
DNSRecon integration
AI-Powered Analysis
Attack surface analysis
CVSS scoring assistance
AI-generated security reports
Exploit chain recommendations
Vulnerability explanations
Reporting
ZIP report export
Security report archiving
Audit logs
HTML interface support
Structured JSON outputs
Project Structure
SecAnalyzer/
├── SecAnalyzer.py
├── helpers/
│   ├── SecAnalyzer.py
│   ├── file_ops.py
│   ├── colours.py
│   └── mimetype_map.py
├── model/
│   └── run_model.py
├── TEMPLATES/
│   ├── api_keys_finder.yaml
│   ├── cloud_buckets.yaml
│   ├── common_vulns_checker.yaml
│   ├── endpoint_discovery.yaml
│   ├── js_url_extractor.yaml
│   └── sensitive_files.yaml
├── dnsrecon/
├── security_reports/
├── requirements.txt
└── SecAnalyzer_GUI.html
Installation
Clone the Repository
git clone https://github.com/yourusername/SecAnalyzer.git
cd SecAnalyzer
Create Virtual Environment
python3 -m venv venv
source venv/bin/activate
Install Dependencies
pip install -r requirements.txt
Configuration
Gemini API Setup

Set your Google Gemini API key:

export GEMINI_API_KEY="your_api_key_here"

Or configure it directly in your environment before launching the application.

Usage

Run the main application:

python3 SecAnalyzer.py

The application launches an interactive terminal interface with multiple security modules.

Example Capabilities
Web Security Scan
python3 SecAnalyzer.py

Then choose:

Web Scanning
Target URL
Vulnerability module
Port Scanning
nmap -sV target.com
DNS Enumeration
python3 dnsrecon/dnsrecon.py -d example.com
Dependencies

Main libraries used:

requests
rich
google-generativeai
urllib3
werkzeug
dnspython
flask
numpy
markdown2

See requirements.txt for the complete dependency list.

Security Notice

This project is intended strictly for:

Authorized penetration testing
Educational purposes
Security research
Internal infrastructure assessments

Do NOT use this tool against systems without explicit authorization.

The developers assume no liability for misuse or illegal activities.

Screenshots
Terminal Interface

Add screenshots here:

screenshots/main-ui.png
Report Output
screenshots/report-example.png
Future Improvements
Docker support
Distributed scanning
Multi-user dashboard
Burp Suite integration
API mode
Plugin architecture
SIEM integration
Automated remediation suggestions
Contributing

Contributions are welcome.

Steps
Fork the repository
Create a feature branch
Commit changes
Push the branch
Open a pull request
License

This repository is provided for educational and authorized security testing purposes.

You may add your preferred open-source license here.

Recommended:

MIT License
Apache 2.0
GPLv3
Acknowledgements
Rich Python Library
Google Gemini API
DNSRecon Project
Open-source cybersecurity community
Disclaimer

SecAnalyzer Pro is a security testing framework intended only for legal and authorized environments.

Any unauthorized use against third-party systems is strictly prohibited.
