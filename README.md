**Project Description:** A weather dashboard that integrates External API, cloud storage, and Python development to deliver real-time weather insights. This project demonstrates the following principles:

```
External API Integration (OpenWeather API)
Cloud Storage (AWS S3)
Infrastructure as Code
Version Control (Git)
Python Development
Error Handling
Environment Management
```

**Key Features:**
```
The system uses Open weather API to fetch real-time weather data for multiple cities
It extracts and displays weather details including temperature (°F), humidity, and weather conditions
Automatically stores weather data in JSON format to an AWS S3 bucket for further analysis
Supports multiple cities tracking
Timestamps all data for historical tracking
```

**Prerequisites:**
```
Language: Python 3.x
Cloud Provider: AWS (S3)
External API: OpenWeather API
Git for version control
Dependencies:
  boto3 (AWS SDK)
  python-dotenv
  requests
```

```
Directory Structure:

├── src/                     # Source code directory
│   ├── __init__.py          # Makes src a Python package
│   └── weather_dashboard.py # Main application logic
├── tests/                   # Test cases (future implementation)
├── data/                    # Data storage (if needed locally)
├── .env                     # Environment variables file
├── .gitignore               # Git ignored files
├── requirements.txt         # Python dependencies
└── README.md                # Project documentation
```

**Setup Instructions**

1. Clone the repository: git clone https://github.com/charity-web/DevOps-Challenge-weather-dashboard.git

2. Install dependencies: pip install -r requirements.txt

3. Configure environment variables (.env):
    ```
    OPENWEATHER_API_KEY=your_api_key
    AWS_BUCKET_NAME=your_bucket_name
    ```

4. Configure AWS credentials:
  ```
  AWS_Access_Key_ID=your_aws_access_key
  AWS_Secret_Access_Key=your_aws_secret_access_key
  ```

5. Run the application: python src/weather_dashboard.py

**Lessons Learned:**

```
How to securely store and manage API keys using environment variables.
Using Git for version control and tracking project changes.
Handling errors in distributed systems.
```
**Challenges Faced:**
I ran into an issue installing pip on WSL. I fixed it by updating the requests package from version 2.82.2 to 2.31
