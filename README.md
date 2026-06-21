# Environmental-Vital-Signs-FHIR-IoT
# FHIR-Compliant IoT Middleware for Environmental Vital Signs
### Prototype for Respiratory Care in Bhaktapur, Nepal

## Overview
This project bridges the gap between environmental monitoring and clinical decision support. It fetches real-time PM2.5 data from PurpleAir sensors, calibrates it for local humidity, and transforms it into HL7 FHIR Observation resources.

## Key Features
- **IoT Integration:** Real-time API pipeline for 39 sensors in Bhaktapur.
- **Informatics Standards:** Uses HL7 FHIR R4, LOINC (81245-3), and UCUM units.
- **Clinical Decision Support:** Automated WHO 2021 threshold alerts for Asthma/COPD patients.
- **Privacy-First:** Docker-based architecture to comply with Nepal Privacy Act 2018.

## Tech Stack
- **Language:** Python 3.9
- **Standards:** HL7 FHIR R4
- **Database:** SQLite (local cache) & HAPI FHIR Server
- **Frontend:** HTML5 (SMART on FHIR Dashboard)

## How to Run
1. Clone the repository.
2. Run `pip install -r requirements.txt`.
3. Start the FHIR server: `docker-compose up -d`.
4. Run the middleware: `python Main1.py`.
5. Open `dashboard.html` to view clinical alerts.
