
# GPTmod - Advanced Vulnerability Assessment Tool

## Features

- Reconnaissance: DNS enumeration, port scanning, technology detection.
- Brute Force: FTP, SSH, HTTP (Basic Auth) brute-force attacks.
- Automated Exploitation: SQL Injection, XSS exploitation.
- Reporting: Generate detailed reports with attack statistics.
- REST API: Integrate scanning into pipelines using Flask.
- Anomaly Detection: Future integration for detecting unusual patterns in data.

## Installation

1. Clone the repository.
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Ensure tools like Hydra, sqlmap, and nmap are installed on your system.

## Usage

1. Start the Flask server:
    ```bash
    python main.py
    ```
2. Use the API to trigger scans:
    ```bash
    curl -X POST -H "x-api-key: your_secret_key" -d '{"scan_type": "quick"}' http://localhost:5000/api/scan
    ```

## Future Enhancements

- Add support for more protocols in brute-force attacks.
- Expand machine learning-based anomaly detection.
- Introduce more comprehensive reporting with vulnerability categorization.

