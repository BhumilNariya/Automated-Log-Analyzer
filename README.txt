# 📊 Automated Log Analyzer

> **A lightweight Bash-based log monitoring and reporting tool for Linux systems.**

Automated Log Analyzer is a command-line utility designed to simplify system log monitoring by automatically scanning log files for critical events such as errors, warnings, failed login attempts, unauthorized access, and crashes. It generates detailed HTML reports, archives analyzed logs, and supports email notifications, making it suitable for system administrators, DevOps engineers, and Linux enthusiasts.

---

## ✨ Features

- 🔍 Analyze Linux system log files
- ❌ Detect errors and warnings
- 🔐 Identify failed login attempts
- 🚫 Detect unauthorized access events
- 💥 Monitor application crashes
- 📊 Generate HTML reports
- 📁 Archive analyzed log files
- 📧 Email generated reports
- 🖥️ Colorized terminal output
- ⏰ Cron job support for scheduled execution

---

## 🚀 Tech Stack

| Component | Technology |
|-----------|------------|
| Language | Bash Shell |
| Platform | Linux |
| Utilities | grep, awk, sort, uniq, mailx |
| Reports | HTML |
| Automation | Cron |

---

## 📂 Project Structure

```text
Automated-Log-Analyzer/
│
├── log_analyzer.sh          # Main Bash script
├── README.txt               # Basic project guide
│
├── sample_logs/             # Sample log files
│   ├── auth_log.txt
│   ├── syslog.txt
│   ├── application_log.txt
│   ├── security_log.txt
│   ├── network_log.txt
│   ├── performance_log.txt
│   └── ...
│
├── logs/
│   └── archive/             # Archived log files
│
├── reports/                 # Generated HTML reports
│
└── README.md
```

---

# 🚀 Getting Started

## Prerequisites

- Linux operating system
- Bash
- grep
- awk
- sort
- uniq
- mailx (optional, for email reports)

---

## Clone Repository

```bash
git clone https://github.com/yourusername/Automated-Log-Analyzer.git

cd Automated-Log-Analyzer
```

---

## Make the Script Executable

```bash
chmod +x log_analyzer.sh
```

---

## Run the Analyzer

Analyze a log file:

```bash
./log_analyzer.sh /path/to/logfile.log
```

Example:

```bash
./log_analyzer.sh sample_logs/syslog.txt
```

---

# 📊 Analysis Performed

The analyzer scans log files for:

- Errors
- Warnings
- Failed Password Attempts
- Unauthorized Access
- Crash Events
- Frequently occurring log messages

It also displays:

- Summary statistics
- Top 5 frequent log messages
- Matching log entries
- HTML report location

---

# 📄 Generated Reports

After execution, the tool automatically:

- Generates an HTML report
- Archives the analyzed log
- Displays a terminal summary
- Sends the report via email (if configured)

Reports are stored in:

```text
reports/
```

Archived logs are stored in:

```text
logs/archive/
```

---

# 📧 Email Configuration

Configure the recipient email inside the script:

```bash
EMAIL_RECIPIENT="your-email@example.com"
```

Ensure `mailx` is installed and configured before using email notifications.

---

# ⏰ Schedule with Cron

Run the analyzer every day at **9:00 AM**:

```cron
0 9 * * * /path/to/log_analyzer.sh /path/to/syslog
```

---

# 🖥️ Sample Output

```text
==== Log Analysis Report ====

Errors: 15
Warnings: 8
Failed Logins: 4
Unauthorized Access: 2
Crashes: 1

Top 5 Frequent Log Messages

...
```

---

# 🔒 Use Cases

- Linux System Monitoring
- Server Log Analysis
- Security Monitoring
- Failed Login Detection
- DevOps Automation
- System Administration
- Incident Reporting

---

# 🚀 Future Improvements

- PDF report generation
- Email attachments with compressed logs
- Multi-log analysis
- Interactive dashboard
- Real-time log monitoring
- Slack and Discord notifications
- Docker support
- Severity-based filtering

---

# 🤝 Contributing

Contributions are welcome.

1. Fork the repository
2. Create a feature branch

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

# 📄 License

This project is licensed under the **MIT License**.

---

# 👨‍💻 Author

**Your Name**

GitHub: https://github.com/yourusername

---

⭐ If you found this project useful, consider giving it a **Star** on GitHub.
