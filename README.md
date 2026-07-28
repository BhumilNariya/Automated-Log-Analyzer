# 📊 Automated Log Analyzer

> A lightweight Bash-based log analysis tool that automates system log monitoring, detects critical events, generates HTML reports, and archives logs for future reference.

## 📖 Overview

Automated Log Analyzer is a Linux shell scripting project designed to simplify system log monitoring. The tool scans log files, identifies important events such as errors, warnings, failed login attempts, and suspicious activities, then generates a detailed HTML report for easier analysis.

It is intended for Linux administrators, DevOps engineers, students, and anyone learning shell scripting and system administration.

---

## ✨ Features

- 🔍 Analyze Linux log files
- ❌ Detect errors and warnings
- 🔐 Identify failed login attempts
- 🚨 Detect suspicious security events
- 📈 Display log statistics
- 📄 Generate HTML reports
- 📁 Archive analyzed log files
- 📧 Optional email notification support
- ⏰ Supports scheduled execution using Cron
- 💻 Simple command-line interface

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Bash | Core scripting language |
| Linux Utilities | grep, awk, sed, sort, uniq |
| HTML | Report generation |
| Cron | Task scheduling |
| Mailx (Optional) | Email notifications |

---

## 📂 Project Structure

```text
Automated-Log-Analyzer/
│
├── log_analyzer.sh          # Main analysis script
├── README.md
│
├── sample_logs/             # Sample log files
│   ├── auth.log
│   ├── syslog
│   ├── application.log
│   └── ...
│
├── reports/                 # Generated HTML reports
│
└── archive/                 # Archived log files
```

---

# 🚀 Getting Started

## Prerequisites

- Linux Operating System
- Bash
- grep
- awk
- sed
- sort
- uniq

Optional:

- mailx (for email notifications)

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/Automated-Log-Analyzer.git

cd Automated-Log-Analyzer
```

Grant execute permission:

```bash
chmod +x log_analyzer.sh
```

---

## Usage

Run the analyzer by providing a log file:

```bash
./log_analyzer.sh /path/to/logfile.log
```

Example:

```bash
./log_analyzer.sh sample_logs/syslog
```

---

## 📊 Report Output

After execution, the analyzer generates:

- Total Errors
- Total Warnings
- Failed Login Attempts
- Security Events
- Most Frequent Log Messages
- HTML Report

Example:

```
================================

Log Analysis Summary

================================

Errors Found           : 15
Warnings Found         : 9
Failed Login Attempts  : 5
Security Alerts        : 2

HTML Report Generated Successfully

================================
```

---

## 📁 Output Files

Generated reports are stored in:

```text
reports/
```

Processed log files are archived in:

```text
archive/
```

---

## ⏰ Automate with Cron

Run every day at midnight:

```cron
0 0 * * * /home/user/Automated-Log-Analyzer/log_analyzer.sh /var/log/syslog
```

---

## 📌 Use Cases

- Linux System Administration
- Server Monitoring
- Security Auditing
- Failed Login Detection
- Log File Analysis
- DevOps Automation
- Learning Bash Scripting

---

## 🚀 Future Improvements

- PDF report generation
- Interactive dashboard
- Multi-log analysis
- Real-time log monitoring
- Docker support
- Slack/Discord notifications
- Severity-based filtering
- CSV export

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a new feature branch

```bash
git checkout -b feature/new-feature
```

3. Commit your changes

```bash
git commit -m "Add new feature"
```

4. Push your branch

```bash
git push origin feature/new-feature
```

5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more details.

---

## 👨‍💻 Author

**Your Name**

- GitHub: https://github.com/yourusername
- LinkedIn: https://linkedin.com/in/yourusername

---

## ⭐ Support

If you found this project useful, consider giving it a **⭐ Star** on GitHub.

It helps others discover the project and motivates future improvements.
