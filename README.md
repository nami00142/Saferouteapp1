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
### Safe Zone Mapping
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
## Application Screens

### 1️⃣ Login Screen
- User enters name and phone number to authenticate.  
- Redirected to **Home Screen** after login.  

 ![Splash Screen](https://github.com/nami00142/Saferouteapp1/blob/main/WhatsApp%20Image%202026-01-31%20at%206.42.53%20PM%20(1).jpeg)

---

### 2️⃣ Home Screen
- Three main options: **Safe Route**, **Emergency**, **Safe Zone**.  
- Clean, user-friendly layout for quick access to safety features.

 ![Splash Screen](https://github.com/nami00142/Saferouteapp1/blob/main/SafeRoute%20Homescreen.jpeg)

---

### 3️⃣ Emergency Screen
- Automatically triggered by phone shaking.  
- 10-second countdown before sending SOS.  
- Buttons for **Police** and **Women’s Help Line** calls.  

 ![Splash Screen](https://github.com/nami00142/Saferouteapp1/blob/main/emergency%20screen%201.jpeg)
 
 ![Splash Screen](https://github.com/nami00142/Saferouteapp1/blob/main/SOS%20message.jpeg)

 ![Splash Screen](https://github.com/nami00142/Saferouteapp1/blob/main/Emergency%20screen%202.jpeg)

---

### 4️⃣ Safe Zone Map
- Shows **nearest police stations** relative to user location.  
- Interactive Google Maps interface.  

![Splash Screen](https://github.com/nami00142/Saferouteapp1/blob/main/SafeZone.jpeg)

---

### 5️⃣ Navigation Map Screen

- Allows users to access real-time navigation services.  
- Redirects the user to **Google Maps** using the ActivityStarter component.  
- Users can choose their destination directly in Google Maps.

![Splash Screen](https://github.com/nami00142/Saferouteapp1/blob/main/mapscreen1.jpeg)

![Splash Screen](https://github.com/nami00142/Saferouteapp1/blob/main/mapscreen2.jpeg)

---

## Frontend Design

- Simple, intuitive UI with **clear icons** for safety features.  
- Easy navigation between Home, Emergency, and Safe Zone screens.  
- Responsive layout suitable for real-time use.  
- Focus on **minimal steps** to trigger safety actions.  

---

## Backend Logic / Data Handling

### Authentication
- User credentials stored in **TinyDB**.  
- Name and phone number used for identity verification.  

### Emergency Detection Logic
- **Accelerometer sensor** detects continuous phone shaking.  
- Notification prompts user confirmation.  
- **Countdown logic** triggers automatic SOS if not canceled.

### Location Sharing
- GPS coordinates fetched in real-time using **LocationSensor**.  
- SOS message includes a **Google Maps clickable link**.  
- Automatic messaging sent via SMS or social component.  

### Safe Zone Logic
- Maps component calculates nearest police stations using current location.  
- Real-time display ensures actionable routing during emergencies.  

---

## Installation & Setup

This project is developed using **MIT App Inventor** and is provided as a `.aia` project file.

### Steps to Access the Application

1. Download the [SafeRoute.aia](https://github.com/nami00142/Saferouteapp1/blob/main/SafeRoute%20(2).aia) file from this GitHub repository.
2. Open your web browser and go to the MIT App Inventor website:  [MIT App Inventor](https://appinventor.mit.edu)
3. Sign in using your Google account.
4. Click on **Projects** → **Import project (.aia) from my computer**.
5. Select the downloaded **SafeRoute.aia** file.
6. The project will be loaded into MIT App Inventor and is ready to run or modify.

### To Run the Application on a Mobile Device

1. Install the **MIT AI2 Companion** app from the Google Play Store.
2. Connect your mobile phone and computer to the same Wi-Fi network.
3. In MIT App Inventor, click **Connect** → **AI Companion**.
4. Scan the QR code using the MIT AI2 Companion app.
5. The application will launch on your mobile device for testing.

---
