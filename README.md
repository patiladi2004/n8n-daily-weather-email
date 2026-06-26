# 🌤️ Daily Morning Weather Summary Email (n8n)

## Overview

This project is an automated n8n workflow that sends a daily weather summary for Mumbai to your Gmail inbox every morning at **7:00 AM**.

The workflow retrieves real-time weather information using the OpenWeatherMap API and generates a clean HTML email containing temperature, weather conditions, humidity, and wind speed.

This project demonstrates how n8n can automate repetitive tasks by integrating scheduling, external APIs, and email services without writing extensive code.

---

## Features

- ⏰ Automatically runs every day at 7:00 AM
- 🌍 Fetches real-time weather data for Mumbai
- ☁️ Uses the OpenWeatherMap API
- 📧 Sends a beautifully formatted HTML email via Gmail
- 🌡️ Displays:
  - Temperature
  - Feels Like Temperature
  - Weather Conditions
  - Humidity
  - Wind Speed
- ⚡ Fully automated using n8n

---

## Workflow

```
Schedule Trigger
        │
        ▼
Fetch Weather (OpenWeatherMap)
        │
        ▼
Generate HTML Weather Summary
        │
        ▼
Send Email using Gmail
```

---

## Technologies Used

- n8n
- OpenWeatherMap API
- Gmail OAuth2
- HTML Email Templates

---

## Prerequisites

Before importing the workflow, make sure you have:

- n8n installed (Cloud or Self-hosted)
- OpenWeatherMap API credentials
- Gmail OAuth2 credentials configured in n8n

---

## Setup

1. Clone this repository.

2. Import the `workflow.json` file into n8n.

3. Configure your credentials:
   - OpenWeatherMap API
   - Gmail OAuth2

4. Update:
   - City name (optional)
   - Recipient email address

5. Activate the workflow.

The automation will now send a weather update every morning.

---

## Email Preview

The email includes:

- Good Morning greeting
- Current temperature
- Feels Like temperature
- Weather description
- Humidity
- Wind speed

Example:

Good Morning! 🌤️

Temperature: 29°C  
Feels Like: 33°C  
Conditions: Scattered Clouds  
Humidity: 78%  
Wind Speed: 3.5 m/s

---

## Project Structure

```
daily-weather-email-automation-n8n/
│
├── workflow.json
├── README.md
└── images/
    └── workflow.png
```

---

## Future Improvements

- Support multiple cities
- Dynamic city selection
- Weekly weather forecast
- AI-generated weather summary
- Telegram or WhatsApp notifications
- Weather alerts for rain or extreme temperatures

---

## License

This project is open source and available under the MIT License.
