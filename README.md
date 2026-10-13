Project Description

This project generates a structured JSON report by analyzing log data and producing summaries and individual entries. The main objective is to process raw log files and convert them into a clear, machine-readable report for further analysis.

Installation Steps

Follow these steps to set up and run the project.

1. Clone the Repository

git clone https://github.com/thakreganesh43-collab/log-report-fixed.git

2. Navigate to the Project Directory

cd log-report-fixed

3. Install Dependencies

Install the required dependencies using the appropriate package manager for the project.

bash
git clone https://github.com/thakreganesh43-collab/log-report-fixed.git
cd log-report-fixed
Dependencies install karo:

bash
pip install -r requirements.txt
python solution/solve.sh data/access.log
{
  "summary": {
    "total_requests": 2,
    "unique_ips": 2,
    "status_codes": {
      "200": 1,
      "302": 1
    }
  },
  "entries": [
    {
      "ip": "127.0.0.1",
      "timestamp": "21/Jul/2026:16:40:00 +0000",
      "method": "GET",
      "endpoint": "/index.html",
      "status": 200,
      "size": 1024
    },
    {
      "ip": "192.168.0.1",
      "timestamp": "21/Jul/2026:16:41:00 +0000",
      "method": "POST",
      "endpoint": "/login",
      "status": 302,
      "size": 512
    }
  ]
}
