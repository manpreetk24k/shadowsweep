# shadowsweep
ShadowSweep – Android Threat Analysis Tool

ShadowSweep is a Python-based forensic tool for Android threat detection and analysis.
It was developed as part of an internship project at Indira Gandhi Delhi Technical University for Women (IGDTUW).

The tool detects hidden apps, malware, and suspicious behavior by analyzing Android device logs.
It also integrates OSINT (Open Source Intelligence) techniques such as WHOIS, IP lookups, and dark web scanning (via Tor), presented through an interactive Streamlit dashboard.

🚀 Features

Log Analysis – Extracts and analyzes Android logs using ADB.

OSINT Integration – WHOIS, IP lookups, and dark web scanning via Tor.

Interactive Dashboard – Streamlit-based UI for easy navigation.

Exportable Reports – Generate CSV reports for documentation.

Network-level Analysis – Supports extended forensic investigation.

🛠️ Tech Stack

Python

Streamlit

Android Debug Bridge (ADB)

Tor Browser / Tor Service (for dark web scanning)

Requests, WHOIS libraries

📂 Project Structure
ShadowSweep/
│
├── app.py         # Main Streamlit app
├── demo/          # Screenshots / demo video
├── requirements.txt
└── README.md

⚡ Installation & Usage
1. Clone the repository
git clone https://github.com/your-username/shadowsweep.git
cd shadowsweep

2. Install dependencies
pip install -r requirements.txt

3. Install & Run Tor

Download Tor Browser or install Tor service:

Tor Project

Start the Tor service so ShadowSweep can connect for dark web scanning.

For Linux (example):

sudo apt install tor
service tor start


For Windows, simply install Tor Browser and keep it running in the background.

4. Connect Android Device

Enable USB debugging on your phone and connect via USB.
Verify connection:

adb devices

5. Run the Application
streamlit run app.py

📊 Outputs

Malware/hidden app detection results

WHOIS/IP lookup information

Dark web scanning results (via Tor)

CSV reports for offline analysis


🧑‍💻 Skills Demonstrated

Digital Forensics

Android Debug Bridge (ADB)

OSINT (WHOIS, IP lookup, dark web scanning)

Python Programming

Streamlit Dashboard Development
