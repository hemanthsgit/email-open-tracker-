# email-open-tracker-
Track email opens using invisible pixel tracking with Flask, ngrok, and Gmail SMTP.​

Features
Real-time tracking — Logs IP address, timestamp (IST), and open count when emails are viewed​

Web dashboard — View tracking logs in a clean HTML table format​

CSV export — Download logs for further analysis​

1×1 pixel tracking — Invisible GIF embedded in emails for seamless monitoring​

Installation
bash
pip install flask pyngrok pytz requests
Setup
Configure ngrok auth token — Replace with your token in the code​

Update email credentials — Add Gmail address and app password​

Run in Google Colab — Optimized for Colab environment​

Usage
Run the script to start Flask server and generate public URLs:

text
✅ Tracking Pixel URL: https://xxxx.ngrok-free.app/track?id=user123
📊 Dashboard URL: https://xxxx.ngrok-free.app/dashboard
Insert the tracking pixel URL into your email HTML as a hidden image.​

Routes
/track — Logs email opens and serves tracking pixel​

/dashboard — Displays tracking data in table format​

/export — Downloads logs as CSV file​

Tech Stack
Backend: Flask, smtplib, email.mime
Networking: ngrok, requests
Utilities: pytz (IST timezone), defaultdict
Platform: Google Colab
