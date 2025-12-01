# RadioDJ_Butler_v1.07 Readme

## 👋 RadioDJ Database Maintenance Utility

Welcome to **RadioDJ_Butler_v1.07**!

This is a helpful tool designed to keep your RadioDJ database running smoothly.

This program is released as **FreeWare**. Feel free to use it as you wish, just please don't modify or sell it (like anyone would pay for this. Ha Ha). It was done primarily as a learning project for coding GUI based programs. I know it's kind of clunky looking.

---

## ✨ Key Features

* **Color-Coded Progress:** Get status updates with color-coded reports.
* **Connection Test:** Easily perform MySQL connection testing.
* **Full Backup:** Create a full database backup/restore.
* **Maintenance:** Table optimization & analysis.
* **Automation:** CLI parameter support for scheduled tasks.

---

## 🛠️ Database Tasks (What Each Button Does)

| Task | Description |
| :--- | :--- |
| **Check** | Validates songs table integrity. |
| **Analyze** | Updates table statistics for query optimization. |
| **Backup** | Creates a timestamped SQL backup. |
| **Optimize** | Runs `OPTIMIZE TABLE` on all database tables. |

---

## 🚀 Command Line Interface (CLI) Usage

You can run maintenance tasks automatically by passing a simple parameter:

* **To run a Backup:**
    `RadioDJ_Butler.exe -backup`
* **To run an Optimization:**
    `RadioDJ_Butler.exe -optimize`

*(MySQL paths are auto-detected).*

---

## 🙏 Contact and Support

This program is **© 2025 JackRabbit Radio Software**.

For support or questions:

* **GitHub:** Please leave a message on the GitHub release page.
* **RadioDJ.ro Forums:** I can also be reached in the RadioDJ.ro forums as **'JackRabbit'**.
* **Be Kind:** This is one of my first GUI based programs.
