# OSINT Intelligence Platform

**Note:** This project was originally developed by [tarouka02/osint-app](https://github.com/tarouka02/osint-app).  
This fork highlights my personal contributions to the **risk analysis and scoring algorithm**, which evaluates the threat level of IPv4 addresses using data from multiple intelligence sources.

---

## Project Overview

The OSINT Intelligence Platform is a web application built with Flask that automates the collection and analysis of open-source intelligence (OSINT) for IP addresses.  
The platform aggregates data from several public APIs and generates a visual risk report to help analysts assess potential threats.  
It features an interactive web interface and integrates multiple data points into a single, comprehensive dashboard.

---

## My Contribution

I developed the **Risk Analysis and Scoring System**, which performs the following:

- Aggregates data from **VirusTotal**, **AbuseIPDB**, and **Shodan** APIs.  
- Computes a **composite risk score** based on severity levels, confidence scores, and historical data.  
- Implements a **weighted algorithm** that prioritizes reliable threat indicators.  
- Designed a **color-coded risk display** for easier interpretation of results.  
- Built error handling to maintain reliability during API rate limits or connection failures.

This work transformed raw API outputs into actionable intelligence, improving both analytical accuracy and user experience.

---

## Key Features

- Geolocation, ASN, and organization details from **IPinfo**  
- Abuse reports, confidence scores, and threat history from **AbuseIPDB**  
- Threat statistics and malware detections from **VirusTotal**  
- Open ports, ISP, and hostnames from **Shodan**  
- Integrated **risk scoring algorithm** combining multi-source signals  
- Responsive web interface with a professional design  
- Front-end enhancements (Typed.js, Swiper.js, AOS.js) for clarity and usability

---

## Technology Stack

**Backend**
- Python 3  
- Flask  
- Requests

**Frontend**
- HTML5, CSS3  
- Bootstrap 5  
- Swiper.js (slide animations)  
- Typed.js (typing header animation)  
- AOS.js (scroll-triggered animations)

**External APIs**
- IPinfo — https://ipinfo.io/  
- AbuseIPDB — https://abuseipdb.com/  
- VirusTotal — https://www.virustotal.com/  
- Shodan — https://www.shodan.io/

---

## Setup Instructions

### 1) Clone the repository
```bash
git clone https://github.com/tarouka02/osint-app.git
cd osint-app


### 2. Create and activate a virtual environment

#### Create virtual environment
```bash
python -m venv venv
```

#### Windows (PowerShell)
```bash
.\venv\Scripts\Activate
```

#### macOS/Linux
```bash
source venv/bin/activate
```

### 3. Install dependencies
```bash
pip install flask requests
```

### 4. Run the App
```bash
flask run
```

### 5. Project Structure
```bash
osint-intel-platform/
├── static/
│   └── styles.css, scripts/
├── templates/
│   ├── index.html
│   ├── loading.html
│   └── result.html
├── app.py or routes.py
├── requirements.txt
└── README.md
```

