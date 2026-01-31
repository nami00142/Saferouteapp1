# Safe Route

**Safe Route** is a mobile application developed using **MIT App Inventor** that focuses on personal safety during navigation. It combines real-time location tracking, emergency alerts, and safe-zone mapping to provide users with a secure and practical navigation experience, similar to Google Maps but with added safety-focused features.  

---
## Project Overview

Safe Route is designed for **real-world safety**, giving users confidence while traveling. The app detects emergency situations automatically, shares location with authorities, and provides information about nearby police stations. It prioritizes **ease of use, responsive UI, and actionable safety features**.  

---
## Problem Statement

While many navigation apps help with directions, few focus on **user safety in emergencies**. Real-life situations can require **quick emergency notifications** and **location sharing**. Safe Route addresses this problem by integrating navigation with automated safety alerts and direct emergency contact options.  

---
### User Experience
- Secure **login with name and phone number**.  
- Home screen with three options: **Safe Route**, **Emergency**, **Safe Zone**.  

### Emergency Detection & Alerts
- Uses **phone accelerometer** to detect continuous shaking.  
- Triggers an **emergency notification** asking for confirmation.  
- Starts a **10-second countdown** before sending an **SOS message** automatically.  
- Sends **live location** via a clickable Google Maps link to authorities.  
- Quick-call buttons for **Police** and **Women’s Help Line**.
- ### Safe Zone Mapping
- Displays **nearest police stations** using Google Maps component.  

### Future Enhancements
- Incident reporting for user contributions.  
- Smart route analysis considering lighting and crowd density.  
- Enhanced safety notifications.  

---
## MIT App Inventor Components Used

### Sensors
- **LocationSensor**  - Fetches the user’s real-time GPS latitude and longitude.
- **Accelerometer** - For shake detection.
- **Clock** - Implements the 10-second emergency countdown timer and controls time-based actions such as automatic SOS triggering if not canceled by the user.

### User Interface & Utility Components
- **Notifier** - Displays emergency confirmation alerts when continuous phone shaking is detected and used to inform users about SOS countdown and emergency actions.

### Storage
- **TinyDB** - Stores user details such as name and phone number.  

### Maps & Location Visualization
- **Map** - Displays the user’s current location.  

### Connectivity & Social
- **Texting** - Sends SOS messages automatically to authorities or emergency contacts.  
- **PhoneCall** - Enables one-tap calling to Police or Women’s Help Line from the Emergency screen.
- **ActivityStarter** - Opens external applications such as the phone dialer or Google Maps when required.  
---


---
