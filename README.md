# DEIVS
## Digital Evidence Integrity & Verification System

DEIVS is a Python-based Digital Forensics desktop application designed to register, manage and verify the integrity of digital evidence using SHA-256 cryptographic hashing.

The system provides a graphical user interface for evidence management, integrity verification, verification history tracking, evidence archiving and PDF investigation report generation.

---

## Latest Release – v1.0.0

**DEIVS Desktop Application for macOS**

[**Download DEIVS v1.0.0**](https://github.com/pranavagrawalll/DEIVS-Digital-Evidence-Integrity-System/releases/download/v1.0.0/DEIVS-macOS.zip)

[View Release Details](https://github.com/pranavagrawalll/DEIVS-Digital-Evidence-Integrity-System/releases/tag/v1.0.0)

### Installation

1. Download `DEIVS-macOS.zip`.
2. Extract the downloaded ZIP file.
3. Open the extracted folder.
4. Launch `DEIVS.app`.
5. If macOS displays a security warning, follow the appropriate macOS security approval process.

**Note:** The application is packaged with its required runtime dependencies. A separate Python installation is not required to run the packaged application.

---

## Features

- Register digital evidence files.
- Generate SHA-256 cryptographic hash values.
- Store evidence records in an SQLite database.
- Verify digital evidence integrity.
- Detect modified or missing evidence files.
- Maintain verification history.
- Search and view registered evidence.
- Soft-delete evidence records.
- View deleted evidence records.
- Restore archived evidence.
- Permanently delete archived evidence records.
- Generate PDF investigation reports.
- Choose a custom location to save generated reports.
- Open generated reports directly.
- Open the folder containing generated reports.
- Reset the database for a fresh start.

---

## Technologies Used

- **Python** – Core application development.
- **Tkinter** – Graphical User Interface.
- **SQLite** – Local database management.
- **SHA-256 (Hashlib)** – Cryptographic hashing and integrity verification.
- **ReportLab** – PDF investigation report generation.
- **PyInstaller** – Desktop application packaging.

---

## Project Team

| Sr. No. | Team Member Name | PRN Number |
|:---:|---|:---:|
| 1 | Pranav Mohan Agrawal | 1272260373 |
| 2 | Rujula Jadhav | 1272261758 |
| 3 | Swayam Dakare | 1272261583 |
| 4 | Samruddhi Salunke | 1272261145 |

## Team Contributions

| Team Member | Contribution |
|---|---|
| Pranav Mohan Agrawal | Software Development & Code Implementation |
| Rujula Jadhav | Presentation (PPT) Preparation |
| Swayam Dakare | Project Poster Design |
| Samruddhi Salunke | Project Presentation |

---

## Requirements

- Python 3.10 or later.
- Required Python packages listed in `requirements.txt`.
- Tkinter and SQLite support in the Python installation.

*These requirements apply when running the project from source. The packaged desktop application includes its required runtime dependencies.*

---

## Installation – Run from Source

### 1. Clone the repository

```bash
git clone https://github.com/pranavagrawalll/DEIVS-Digital-Evidence-Integrity-System.git
```

### 2. Open the project folder

```bash
cd DEIVS-Digital-Evidence-Integrity-System
```

### 3. Create a virtual environment

```bash
python3 -m venv .venv
```

### 4. Activate the virtual environment

```bash
source .venv/bin/activate
```

### 5. Install dependencies

```bash
pip install -r requirements.txt
```

### 6. Run the application

```bash
python gui.py
```

---

## Project Structure

```text
DEIVS/
│
├── app_paths.py
├── gui.py
├── database.py
├── hashing.py
├── report.py
├── evidence_manager.py
├── verification.py
├── reset_project.py
├── main.py
├── requirements.txt
└── README.md
```

---

## Database and Data Storage

DEIVS uses SQLite for local evidence record management.

Application data is stored in the user's application support directory, keeping database records separate from the application installation.

Generated PDF investigation reports are saved in the default reports directory. Users can also select a custom location when generating a report.

Original evidence files are not deleted when an evidence record is archived or permanently removed from the DEIVS database.

---

## Disclaimer

DEIVS is an educational project developed for academic purposes. It demonstrates digital evidence management and hash-based integrity verification.

It is a prototype and is not intended to replace professional digital forensic tools or legally validated evidence-handling procedures. The integrity verification result is based on SHA-256 hash comparison and does not independently establish the authenticity or legal admissibility of evidence.

---

## Author

**Pranav Mohan Agrawal**

GitHub: [@pranavagrawalll](https://github.com/pranavagrawalll)

**Project:** Digital Evidence Integrity & Verification System (DEIVS)

**Project Type:** Group Academic Project

---

If you find this project useful, consider giving the repository a ⭐.