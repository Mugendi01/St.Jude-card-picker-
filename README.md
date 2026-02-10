ST Jude Chama Picker

A responsive, web-based Chama card picker for the ST Jude group. Members can pick a random payout position, and picks are saved online so everyone can see them in real-time. Only the admin (Mary Wanjiku) can reset the picks.

Features

Random card picking: Each member picks a card once; the number corresponds to their payout position.

Persistent storage: Picks and names are stored in Firebase Realtime Database, so everyone sees the current status.

Luxury card design: Elegant, rounded, soft gradient cards with subtle shadow.

Responsive: Works perfectly on mobile and desktop.

Top-falling confetti: Adds a mini-game celebratory effect when a user picks a card.

Admin-only reset: Only Mary Wanjiku can reset all picks.

Colors

Primary palette: #6CA651, #BBCB2E, #839705, #6B7445

Getting Started
Prerequisites

A web browser (Chrome, Edge, Safari, Firefox)

Internet connection to access Firebase

Setup

Clone or download this repository.

Firebase: Make sure you have a Realtime Database setup. Replace the firebaseConfig in the HTML file with your project’s config.

const firebaseConfig = {
  apiKey: "...",
  authDomain: "...",
  databaseURL: "...",
  projectId: "...",
  storageBucket: "...",
  messagingSenderId: "...",
  appId: "...",
  measurementId: "..."
};


Open index.html in a browser.

Usage

Enter your name in the input field.

Tap Start Picking to reveal your card.

After picking, a thank you message is displayed with your name.

Only Mary Wanjiku sees the Reset All Cards button.

Resetting Cards

Click Reset All Cards (visible only to Mary Wanjiku).

Confirm to remove all picks from Firebase.

Customization

Card colors: Change the gradients in the CSS .card class.

Confetti colors: Adjust in the launchConfetti() function.

Number of cards: Update TOTAL in the script.

Tech Stack

HTML / CSS / JS — Frontend

Firebase Realtime Database — Backend persistence

License

This project is for internal use only for the ST Jude Chama group.
