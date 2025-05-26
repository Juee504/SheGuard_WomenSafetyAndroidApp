# SheGuard_WomenSafetyAndroidApp
SheGuard is a women’s safety app that sends SOS alerts with real-time location via SMS, calls, and notifications. Users can trigger emergencies by shaking their phone, even when locked. Emergency contacts are easily managed within the app. It runs securely in the background for constant protection.

🚩 Problem Statement
In emergencies, women often don’t have time or freedom to dial for help or share their location. Most apps require manual input, which isn't always possible during distress.

🎯 Goal
To create a hands-free, real-time, and reliable women safety solution using automated SOS triggers, location tracking, and cloud communication.

🧠 Key Features
Shake-to-Alert: Uses accelerometer sensor to detect phone shake and auto-activate SOS.

📍 Real-time GPS Tracking: Sends user location instantly to emergency contacts.

📞 Multi-mode SOS: Sends SMS, initiates calls, and pushes Firebase notifications.

🔒 Background Service: SOS works even if the app is minimized or screen is off.

🛠 Firebase Integration: Secure real-time database (Firestore) for user data and notifications.

👩‍💻 Personalized Dashboard: Add/manage emergency contacts, toggle settings (siren/SMS/FCM).

🧰 Tech Stack
Tool / Component	Description
Android Studio	Development IDE
Java	Core logic
XML	UI layout design
Firebase Firestore	Real-time NoSQL DB for user/contact data
Firebase Messaging	Push notifications
Sensor APIs	Shake detection
Background Services	Keep app active silently
Data Binding	Clean UI & logic separation
Runtime Permissions	For SMS, Call, Location

📋 User Workflow
Open App → Onboarding (ViewPager2 intro)

Login/Register → Phone number verification via Firebase

Dashboard → Add emergency contacts from phonebook

Enable Shake-to-SOS → App listens for motion in background

Trigger SOS (Shake/Button) → SMS, Call, FCM Notification with location

Settings → Manage siren, push, SMS preferences

🧩 Modular Architecture
Module	Description
Onboarding	Explains app flow & features
Authentication	Firebase Phone Auth + UID mapping
Dashboard	Main control panel, contact addition
SOS Module	Shake detection → Emergency services
Firebase Module	Firestore (UserList, Tokens, PhoneToUid), FCM

🎨 Material Components Used
Buttons → SOS, Login, Registration

CardView → Display contacts/instructions

TextInput → Input phone number

Snackbar/Toast → Feedback messages

Toolbar → Dashboard header & actions

🔐 Security & Privacy
Phone number mapped securely with Firebase UID

Push tokens mapped by UID to avoid spoofing

User data stored in Firestore with rules in place

📦 Data Collections
UserList → User info & contact list

PhoneToUid → Maps phone to UID

Tokens → Device tokens for FCM

📈 Impact
SheGuard aims to reduce the delay in emergency response and provide peace of mind to women. It’s more than just an app — it’s a silent, always-ready companion.
