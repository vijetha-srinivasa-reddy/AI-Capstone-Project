# 💊 MediMind: AI Medication Reminder Assistant

**SDG 3 – Good Health and Well-Being**
Lenovo LEAP NextGen Scholar Program – AI Capstone Project
Submitted by: Vijetha Srinivasa Reddy

MediMind is a simple AI-powered web assistant that helps people take their medicines on time and understand their adherence. It runs in any modern browser, works on mobile, and keeps all data on the user's own device.

## Problem

About half of patients with long-term illnesses do not take their medicines as prescribed (WHO estimate). People forget doses, take them at the wrong time, run out of stock, or cannot track what they have taken. Elderly people, chronic-disease patients and caregivers are affected most.

## Features

- **Add medicines** by form (name, dose, time, type, doses left, optional doctor/pharmacy phone) or by typing a sentence such as `Aspirin 75 mg at 8 pm`
- **Alarm reminders** with sound, vibration and a browser notification when a dose is due, plus a *Test alarm* button and a sound on/off switch
- **Snooze** a reminder for 10 minutes, from the alarm card or the schedule
- **Status tracking:** Upcoming, Snoozed, Taken or Missed
- **Daily insights:** taken, pending and adherence percentage
- **Weekly adherence chart** with a 7-day average
- **Weekly report export:** *Download report* (text file) and *Copy report*
- **Refill alerts** when 3 or fewer doses are left, with a one-tap call link
- **AI assistant** that answers "what's next?", "missed doses", "refill" and "weekly progress", and can add a medicine from a typed sentence
- **Private by design:** data is stored in the browser (localStorage), nothing is sent to a server
- Works in light and dark mode

## Technology stack

- HTML5, CSS3, JavaScript (single file, no frameworks)
- Browser localStorage for storage
- Web Notifications API, Web Audio API and Vibration API for alerts
- Inline SVG for the weekly chart, Blob API for the report file
- Rule-based NLP intent matching for the assistant
- Playwright used to capture the screenshots

## How to run

1. Download `medimind.html` (or `index.html`) from this repository.
2. Open it in Chrome, Edge or any modern browser, on a phone or computer.
3. Allow notifications when asked, so reminders can appear.
4. Add a medicine and press **Test alarm** to hear the alarm and try **Snooze**.

> Reminders ring while the page is open in the browser. Background reminders are listed under future scope.

## Screenshots

Add your screenshots to a `screenshots/` folder and link them here, for example:

```
![Dashboard](screenshots/dashboard.png)
![Alarm with Snooze](screenshots/alarm.png)
![Weekly report](screenshots/weekly.png)
```

## Future scope

- Generative AI model (for example the OpenAI API) for natural conversations
- Background reminders even when the page is closed (service worker and push notifications)
- Mobile app with SMS/WhatsApp reminders and voice alerts in regional languages
- Caregiver alerts when a dose is missed, and prescription scanning using OCR
- Weekly report export as PDF and direct sharing with a doctor; customisable snooze time

## Note

This is a learning prototype and is **not medical advice**. The earlier days in the weekly chart are sample data for demonstration.

## Author

Vijetha Srinivasa Reddy
