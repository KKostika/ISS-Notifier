# 🛰 ISS Overhead Notifier

**ISS Overhead Notifier** is a Python project that tracks the real-time location of the International Space Station (ISS) using public APIs. Whenever the ISS is flying near your location and it's dark enough to see it, the program sends you an email reminder to look up and catch a glimpse!

---

## 🚀 Project Overview

This script:
- Connects to the [Open Notify API](http://open-notify.org/) to get the current coordinates of the ISS
- Checks if the ISS is **close to your location** (based on latitude and longitude)
- Verifies if it's currently **nighttime** at your location (so the ISS is visible)
- Sends an **email alert** when both conditions are met

---

## 🛠 Technologies Used

- Python 3
- `requests` for API calls
- `smtplib` for sending emails
- `datetime`, `pytz` for time and timezone handling
- Sunrise-Sunset API for light condition checks

---


1. Clone the repository:

bash
Set your environment variables:

MY_LAT: your latitude

MY_LONG: your longitude

EMAIL: sender email address

PASSWORD: email password or app-specific password

📧 Sample Notification
Subject: Look Up! 👀 The ISS is currently passing over your location. Step outside and look up!

⏱ Scheduling
You can run the script periodically using:

A while True loop with time.sleep(60)

A cron job or scheduled task depending on your OS

🌐 APIs Used
ISS Location API

Sunrise-Sunset API

💡 Future Enhancements
SMS or Telegram notifications

ISS trajectory visualization with matplotlib

Web dashboard using Flask or Django

👩‍💻 Author
Kyriaki Kostika – GitHub From chef to developer 🚀, passionate about building real-world applications that connect tech with everyday life.
