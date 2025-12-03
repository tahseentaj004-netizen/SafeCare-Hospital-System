# SafeCare-Hospital-System
"A comprehensive safety and management system design for a 700-bed hospital, featuring SQL prototypes and UML process modeling."

# SafeCare Hospital Management System

## 🏥 Project Overview
[cite_start]SafeCare Hospital is a 700-bed medical institution facing critical challenges with unauthorized access, manual patient tracking, and fragmented emergency responses[cite: 36, 42, 46]. [cite_start]This project delivers a comprehensive software engineering solution to modernize operations, ensuring patient safety and operational efficiency[cite: 38].

**Project Type:** First-Year Software Engineering Coursework
**Role:** Systems Analyst & Database Designer
**Tools Used:** Microsoft Access (SQL), Draw.io (UML/DFD), SSAD Methodology.

---

## 🚀 Key Features Designed
* [cite_start]**Digital Identity Management:** A mobile app design allowing patients and visitors to pre-register and receive digital QR badges for access[cite: 49, 50].
* [cite_start]**Access Control:** A rigorous logic model using RFID/Biometrics to secure restricted zones like ICUs[cite: 54].
* [cite_start]**Emergency Response Automation:** An event-driven architecture where wearable sensors detect distress and automatically trigger "Code Blue" alerts to the emergency team[cite: 57, 58].
* [cite_start]**Real-Time Tracking:** A relational database prototype capable of locating any patient or visitor within the hospital instantly[cite: 90].

---

## 📂 Repository Structure
* **/database:** Contains the SQL scripts used to prototype the system (DDL for tables and DML for queries).
* **/diagrams:**
    * **ERD (Entity Relationship Diagram):** Conceptual data model showing relationships between Patients, Visitors, and Access Logs.
    * **DFD (Data Flow Diagram):** Level 1 process model illustrating data movement across the hospital.
    * **UML Sequence Diagrams:** Interaction modeling for "Visitor Registration" and "Emergency Response" scenarios.

---

## 🛠️ Technical Implementation
The system prototype was implemented using **SQL** to validate core functionalities.

### 1. Database Schema
Designed a normalized schema to handle complex relationships:
* `Patient` (1) ↔ (N) `Visitor`
* `Patient` (1) ↔ (1) `WearableDevice`
* `Zone` (1) ↔ (N) `AccessLog`

### 2. Key SQL Functions
The prototype successfully demonstrated the following queries:
* **User Registration:** Inserting visitor data linked to specific patients.
* **Live Location Tracking:** Joining `AccessLog` and `User` tables to view real-time location.
* **Automated Alerting:** Querying `VitalSignLog` to identify critical health thresholds.

---

## 📈 Methodologies Applied
* [cite_start]**SSAD (Structured Systems Analysis and Design):** Used for the preliminary design phase (DFD, ERD)[cite: 81].
* [cite_start]**OOAD (Object-Oriented Analysis and Design):** Used for the flexible system design phase (UML Sequence Diagrams)[cite: 92].
* [cite_start]**LSEPI Analysis:** Evaluated Legal, Social, Ethical, and Professional Issues, including GDPR compliance for patient data[cite: 78].
