🖥️ Guardian Live Dashboard
Guardian Dashboard is the centralized monitoring web interface for the Guardian safety ecosystem. It provides trusted contacts with a high-fidelity, real-time command center to track active SOS alerts, view live locations, and access critical audio evidence.

🚀 Key Features
Real-Time SOS Monitoring: Instantly populates active emergency alerts as they are triggered from the mobile app.

Live Map Integration: Tracks the user's precise coordinates with high-frequency updates during an active SOS event using Leaflet.js.

Evidence Vault: Stream and download the 15-second audio chunks uploaded by the Guardian mobile app for immediate situational awareness.

Secure Access: Uses UID-based secure links to ensure only invited trusted contacts can view live tracking data.

Responsive Web Design: Fully optimized for desktop, tablet, and mobile browsers so guardians can help from any device.

🎨 System Integration
The dashboard acts as the primary receiver in the Guardian ecosystem:

SOS Triggered: Mobile app sends data to Firebase.

Live Sync: Dashboard listens to Firestore changes using the Firebase Web SDK and updates the UI instantly.

Actionable Data: Trusted contacts use the dashboard to coordinate with emergency services.

🛠️ Technical Stack
Frontend: Vanilla HTML5, CSS3, and JavaScript (ES6+)

Maps: Leaflet.js (OpenStreetMap)

Backend Integration: Firebase Firestore (Compat SDK)

Media Handling: Firebase Storage

⚙️ Setup & Local Development
Since this project is built using vanilla web technologies, no complex installation is required:

Clone the Repo: ```bash
git clone https://github.com/kaifansari-11/guardian_dashboard.git

Firebase Configuration:

Open index.html.

Replace the firebaseConfig object with your own credentials from the Firebase Console.

Run the Project:

Simply open index.html in any modern web browser.

Or, use the Live Server extension in VS Code for hot-reloading.

🌐 Live Demo
The dashboard is hosted at: https://guardian-live.netlify.app

Note: For security, the dashboard requires a User ID (uid) in the URL to display data. In a real emergency, this link is automatically generated and sent to trusted contacts via SMS.

To view the interface layout, use this demo link:
https://guardian-live.netlify.app/?uid=DEMO_USER_ID