
# DEIVS
## Digital Evidence Integrity & Verification System

DEIVS is a Python-based Digital Forensics project designed to register digital evidence and verify its integrity using SHA-256 cryptographic hashing.

## Features

- Register digital evidence files.
- Generate SHA-256 hash values.
- Store evidence records in an SQLite database.
- Verify evidence integrity.
- Detect modified or missing evidence.
- Maintain verification history.
- Search evidence using its ID.
- Soft-delete evidence records.
- View deleted evidence records.
- Generate PDF investigation reports.
- Reset the database for a fresh start.

## Technologies Used

- Python
- SQLite
- SHA-256 (Hashlib)
- Tkinter
- ReportLab

## Requirements

- Python 3.10 or later
- Required Python packages listed in `requirements.txt`

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/R-pranavagrawalll/DEIVS-Digital-Evidence-Integrity-System.git
   ```

2. Open the project folder:

   ```bash
   cd DEIVS-Digital-Evidence-Integrity-System
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Run the application:

   ```bash
   python main.py
   ```

## Project Structure

```text
DEIVS/
├── main.py
├── hashing.py
├── database.py
├── verification.py
├── evidence_manager.py
├── report.py
├── reset_project.py
├── requirements.txt
└── README.md
```

## Disclaimer

DEIVS is an educational project developed for academic purposes. It is a prototype and is not intended to replace professional digital forensic tools or legally validated evidence-handling procedures.
