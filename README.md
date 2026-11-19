# DEIVS
## Digital Evidence Integrity & Verification System

DEIVS (Digital Evidence Integrity & Verification System) is a Python-based desktop application developed as a group academic project. It is designed to register, manage, and verify the integrity of digital evidence using SHA-256 cryptographic hashing.

The application provides a graphical user interface (GUI) for managing digital evidence, maintaining verification records, and generating PDF investigation reports.

---

## Project Team

| Sr. No. | Team Member Name | PRN Number |
|:---:|---|:---:|
| 1 | Pranav Mohan Agrawal | 1272260373 |
| 2 | Rujula Jadhav | 1272261758 |
| 3 | Swayam Dakare | 1272261583 |
| 4 | Samruddhi Salunke | 1272261145 |

---

## Features

### 1. Digital Evidence Management
- Register digital evidence files.
- Store evidence details in a local SQLite database.
- View and search registered evidence records.
- Track evidence information using unique Evidence IDs.

### 2. SHA-256 Integrity Verification
- Generate SHA-256 hash values for registered evidence.
- Verify the integrity of digital evidence.
- Detect modifications to evidence files.
- Identify missing or inaccessible evidence files.
- Maintain a verification history with timestamps and results.

### 3. Evidence Archiving and Recovery
- Soft-delete evidence records without immediately removing them permanently.
- View deleted evidence records.
- Restore previously deleted evidence records.
- Permanently delete evidence records when required.

### 4. PDF Investigation Reports
- Generate PDF investigation reports for registered evidence.
- Include evidence details, SHA-256 hash information, and verification results.
- Maintain verification history in generated reports.
- Choose a custom location to save generated reports.
- Open the generated PDF directly or open its containing folder.

### 5. Database Management
- Store application data locally using SQLite.
- Maintain a persistent database across application sessions.
- Reset the database when required.

---

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core application development |
| Tkinter | Graphical User Interface |
| SQLite | Local database management |
| Hashlib | SHA-256 cryptographic hashing |
| ReportLab | PDF investigation report generation |
| PyInstaller | Packaging the application as a desktop app |

---

## Application Release

<escape>**</escape>Current Release:** DEIVS v1.0.0

**Platform:** macOS

**Download:** [Download DEIVS v1.0.0](https://github.com/pranavagrawalll/DEIVS-Digital-Evidence-Integrity-System/releases/tag/v1.0.0)

### Installation (macOS)

1. Visit the [GitHub Releases](https://github.com/pranavagrawalll/DEIVS-Digital-Evidence-Integrity-System/releases) page.
2. Download `DEIVS-macOS.zip`.
3. Extract the downloaded ZIP file.
4. Open the extracted `DEIVS.app` application.

### macOS Security Notice

DEIVS is an academic project and is currently not signed with an Apple Developer ID certificate or notarized by Apple.

Therefore, macOS Gatekeeper may display a security warning when opening the application for the first time.

If macOS displays a warning that the developer cannot be verified or Apple cannot check the application for malicious software, follow these steps:

1. First, try opening `DEIVS.app`.
2. Open the **Apple Menu** and navigate to **System Settings**.
3. Select **Privacy & Security**.
4. Scroll down to the **Security** section.
5. Locate the message indicating that DEIVS was blocked.
6. Click **Open Anyway**.
7. Confirm the action by clicking **Open** in the confirmation dialog.
8. Enter the Mac login password if requested.

After completing these steps, DEIVS should open normally on subsequent launches.

**Important:** Only use this procedure if DEIVS was downloaded from the official project GitHub Releases page and the downloaded application is trusted. Do not bypass warnings stating that an application will damage your computer or that it is damaged.

For additional information, refer to [Apple's official security instructions](https://support.apple.com/en-in/102445).

---

## Running from Source Code

To run the project directly from its source code:

### Requirements
- Python 3.10 or later
- Required packages listed in `requirements.txt`
- Tkinter support in the Python installation

### Installation Steps

1. Clone the repository:

   ```bash
   git clone https://github.com/pranavagrawalll/DEIVS-Digital-Evidence-Integrity-System.git
   ```

2. Navigate to the project directory:

   ```bash
   cd DEIVS-Digital-Evidence-Integrity-System
   ```

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Launch the desktop application:

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
│
├── main.py
├── evidence_manager.py
├── verification.py
├── reset_project.py
│
├── requirements.txt
├── README.md
└── .gitignore
```

### Core Modules

| File | Description |
|---|---|
| `gui.py` | Main desktop application and graphical interface |
| `app_paths.py` | Manages application data and report storage locations |
| `database.py` | Handles SQLite database operations |
| `hashing.py` | Generates SHA-256 hash values |
| `report.py` | Generates PDF investigation reports |
| `main.py` | Original command-line application |
| `evidence_manager.py` | Evidence management operations |
| `verification.py` | Evidence verification operations |
| `reset_project.py` | Database reset functionality |

---

## Data Storage

DEIVS stores application data locally on the user's computer.

- Evidence records and verification history are maintained in an SQLite database.
- Application data is stored in the operating system's application support/data directory.
- Generated PDF reports are saved in the default reports directory or another location selected by the user.
- Evidence files remain at their original locations; DEIVS stores their recorded details and hashes.

**Note:** Users should maintain appropriate backups of their evidence files and application database.

---

## Disclaimer

DEIVS is an educational project developed for academic purposes as a digital forensic demonstration tool.

It is a prototype and is not an independently certified forensic platform. It does not independently establish the authenticity, legal admissibility, or complete chain of custody of digital evidence.

The application provides hash-based integrity verification and evidence management features, but its results should not be treated as a substitute for professional digital forensic tools, validated forensic procedures, or expert examination.

---

## Author

**Pranav Mohan Agrawal**

GitHub: [@pranavagrawalll](https://github.com/pranavagrawalll)

**Project:** Digital Evidence Integrity & Verification System (DEIVS)

**Project Type:** Group Academic Project

---

If you find this project useful, consider giving the repository a ⭐.