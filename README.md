🛡️ IOC Reputation Checker (Single-File React Demo)

This is a dynamic, single-page web application designed to simulate the batch processing and reputation checking of Indicators of Compromise (IOCs). It can parse lists of IOCs (MD5, SHA1, SHA256 hashes, IPv4 addresses, and domains) from a text file, query multiple simulated threat intelligence sources, calculate a composite risk score, and generate detailed reports.

The entire application—including React, component logic, and styling (via Tailwind CSS)—is contained within a single index.html file for easy deployment and portability.

🌟 Features

Batch Processing: Upload a text or CSV file containing multiple IOCs (one per line).

IOC Type Detection: Automatically detects file hashes (MD5, SHA1, SHA256), IPv4 addresses, and domains.

Multi-Source Simulation: Simulates lookups across four key threat intelligence platforms:

VirusTotal (simulated threat score and detection counts)

AbuseIPDB (simulated abuse confidence score for IPs)

AlienVault OTX (simulated pulse counts)

ThreatFox (simulated threat type detection)

Composite Risk Scoring: Calculates a weighted risk score and assigns a risk level (Low, Medium, High).

Reporting: Export results to detailed text reports or CSV files.

🚀 How to Use

Since this application is built into a single HTML file using CDN scripts, running it is extremely simple.

Download: Clone the repository or simply download the index.html file.

Run: Double-click the index.html file in your file explorer. It will open directly in your web browser.

Performing an Analysis

API Keys: The API key fields are present for UI context but are non-functional in this demo. The application uses simulated data.

Prepare File: Create a plain text file (.txt) where each line is a single IOC (e.g., a hash, an IP address, or a domain name).

8.8.8.8
google.com
1a2b3c4d5e6f7a8b9c0d1e2f3a4b5c6d
malware-c2.xyz


Upload: Click the Choose File button and select your IOC list.

Analyze: Click the Start Analysis button. The application will simulate the API calls, show a progress bar, and display the final summary and detailed results.

⚠️ Important Note: Demo Mode

This application is intended as a full-stack front-end demonstration of the user interface and threat intelligence processing logic.

All API calls are simulated using JavaScript functions (mockAPICall). No actual network requests are made to VirusTotal, AbuseIPDB, or any other external service, and no real API keys are required or used. The results are randomly generated for demonstration purposes only
