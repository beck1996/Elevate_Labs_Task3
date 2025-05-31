# Elevate_Labs_Task3
This Repo is related to the internship at Elevate Labs and this is task 3 and this task involves use of nesus on local machine  

Step 1: Install Nessus Essentials
Go to Nessus Essentials Download Page

Register for a free account and get your activation code via email.

Download the Windows installer.

Run the installer and follow the prompts to complete installation.

After installation, open your browser and go to:
https://localhost:8834

Create a Nessus user account.

Enter the activation code to enable Nessus Essentials.

Wait while Nessus downloads all plugins (may take several minutes).

Step 2: Set Up Scan Target
Find your machine’s local IP address:

Open Command Prompt (Windows + R, type cmd)

Type ipconfig and press Enter.

Note the IPv4 Address (e.g., 192.168.1.100) or use 127.0.0.1 for localhost.

Open Nessus web interface.

Click “New Scan” → Select Basic Network Scan (or Advanced Scan).

Enter a name for your scan (e.g., "Local Machine Scan").

In the Targets field, enter your IP address (e.g., 127.0.0.1).

Step 3: Start Full Vulnerability Scan
Click Save to save the scan configuration.

Click the Play (▶) button next to your saved scan to start scanning.

Step 4: Wait for Scan to Complete
The scan will take about 30 to 60 minutes depending on your machine and network.

Keep your browser window open until the scan finishes.

Step 5: Review the Report
Once the scan finishes, click on the scan name.

Look at the summary which categorizes vulnerabilities by severity:

Critical

High

Medium

Low

Click on each vulnerability to view details, including CVSS score and plugin information.

Step 6: Research Simple Fixes or Mitigations
For each critical and medium vulnerability, note down the vulnerability name and plugin ID.

Search for fixes on:

Tenable Plugins

Official software/security vendor sites

General web resources for mitigation steps.

Examples of common fixes:

Updating software/OS

Enabling security features like SMB signing

Replacing untrusted SSL certificates

Step 7: Document the Most Critical Vulnerabilities
Make a report that includes:

| Vulnerability Name                | Plugin ID | Severity | CVSS Score | Description                               | Fix / Mitigation Summary                   |
| --------------------------------- | --------- | -------- | ---------- | ----------------------------------------- | ------------------------------------------ |
| SSL Certificate Cannot Be Trusted | 51192     | Medium   | 6.5        | SSL certificate is self-signed or expired | Replace with trusted certificate           |
| SMB Signing Not Required          | 57608     | Medium   | 5.3        | SMB packets are not digitally signed      | Enable SMB signing in Windows Group Policy |

Step 8: Take Screenshots of Scan Results
Open the detailed scan report in Nessus.

Take screenshots of:

The overall vulnerabilities summary page.

Each critical/medium vulnerability detail page (showing Plugin ID, CVSS score, and description).

Save screenshots for your documentation.
