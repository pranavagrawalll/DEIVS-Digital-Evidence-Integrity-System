# DEIVS – Digital Evidence Integrity & Verification System

**A Python-Based Digital Forensics Desktop Application**

DEIVS (Digital Evidence Integrity & Verification System) is a Python-based digital forensics academic project designed to register, manage, archive, restore, and verify the integrity of digital evidence using SHA-256 cryptographic hashing.

The application provides a graphical desktop interface for digital evidence management, integrity verification, verification history tracking, and PDF investigation report generation.

---

## Project Team

| Name | PRN | Contribution |
|---|---|---|
| Pranav Mohan Agrawal | 1272260373 | Software Development & Code Implementation |
| Rujula Jadhav | 1272261758 | Presentation (PPT) Preparation |
| Swayam Dakare | 1272261583 | Project Poster Design |
| Samruddhi Salunke | 1272261145 | Project Presentation |

---

## Features

### 1. Digital Evidence Registration
- Register and manage digital evidence files.
- Generate SHA-256 cryptographic hashes during registration.
- Store evidence information in a local SQLite database.

### 2. SHA-256 Integrity Verification
- Generate and verify cryptographic hashes.
- Detect whether registered evidence has been modified.
- Identify missing or unchanged evidence files.

### 3. Evidence Management
- View, search, and manage registered evidence records.
- Access evidence details.
- Archive registered evidence.
- Restore archived evidence.
- Permanently delete archived evidence when required.

### 4. Verification History
- Maintain a record of previous integrity verification activities.
- Store verification results and timestamps.
- Review historical verification information.

### 5. PDF Investigation Reports
- Generate detailed PDF investigation reports.
- Include evidence information and verification results.
- Select a custom location to save generated reports.
- Open generated reports or their containing folder directly.

### 6. Database Management
- Store evidence records and verification history locally using SQLite.
- Maintain persistent application data across sessions.

### 7. User Interface
- Graphical desktop interface developed using Python Tkinter.
- Dashboard displaying evidence statistics.
- Navigation between different application modules.
- Horizontal and vertical scrollbars that automatically appear when content exceeds the visible area.

---

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core application development |
| Tkinter | Graphical User Interface |
| SQLite | Local database management |
| SHA-256 | Cryptographic hashing |
| ReportLab | PDF report generation |
| PyInstaller | Desktop application packaging |
| Git & GitHub | Version control and project hosting
