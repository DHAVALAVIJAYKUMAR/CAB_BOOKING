# 🚗 Ride-PK — Full Stack Cab Booking App

**A modern mobile ride-booking app inspired by inDrive and Yango — built with real-world full-stack technologies.**

![Expo](https://img.shields.io/badge/Expo-000020?style=for-the-badge&logo=expo&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Stripe](https://img.shields.io/badge/Stripe-635BFF?style=for-the-badge&logo=stripe&logoColor=white)
![Google Maps](https://img.shields.io/badge/Google_Maps-4285F4?style=for-the-badge&logo=googlemaps&logoColor=white)
![Clerk](https://img.shields.io/badge/Clerk-6C47FF?style=for-the-badge&logo=clerk&logoColor=white)

---

## 🚀 Project Overview

**Ride-PK** is a mobile ride-booking application that lets users book a ride the same way they would on **inDrive** or **Yango** — from setting a pickup point and destination, to choosing a nearby driver and paying securely, all inside one smooth mobile experience.

The app handles the complete ride journey: secure login, live location on the map, ride search, driver selection, fare confirmation, and payment — with the full ride history saved for the user.

It is built using **Expo (React Native)** for the mobile app, **Clerk** for authentication, **NeonDB (PostgreSQL)** for the database, **Stripe** for payments, and **Google Maps + Geoapify** for live maps, directions, and place autocomplete.

**What users can do:**

- 🔐 Register & log in securely (Email or Google)
- 📍 Set pickup & drop-off with live map tracking
- 🔎 Search and view nearby available rides
- 🚗 Select a ride & confirm full fare details
- 💳 Pay securely using Stripe
- 🕓 View ride history & manage profile

---

## 📸 Screenshots

| Onboarding & Auth | Home with Live Map | Recent Rides |
| :---: | :---: | :---: |
| ![Preview 1](screenshots/3.png) | ![Preview 2](screenshots/9.png) | ![Preview 3](screenshots/11.png) |

| Find Rides | Select Ride from Map | Confirm Ride Details |
| :---: | :---: | :---: |
| ![Preview 4](screenshots/5.png) | ![Preview 5](screenshots/7.png) | ![Preview 6](screenshots/10.png) |



## 🛠 Tech Stack & Engineering Skills Applied

### Mobile & Frontend Engineering
![React Native](https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Expo](https://img.shields.io/badge/Expo-000020?style=for-the-badge&logo=expo&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-000000?style=for-the-badge&logo=react&logoColor=white)

* **Frameworks & UI:** React Native (with Expo), NativeWind (Tailwind CSS), TypeScript.
* **State Management:** Zustand — lightweight and scalable state handling.
* **Design:** Fully responsive cross-platform UI (Android & iOS) designed in Figma.

### Backend, Services & Integrations
![NeonDB](https://img.shields.io/badge/NeonDB-00E599?style=for-the-badge&logo=postgresql&logoColor=white)
![Stripe](https://img.shields.io/badge/Stripe-635BFF?style=for-the-badge&logo=stripe&logoColor=white)
![Google Maps](https://img.shields.io/badge/Google_Maps-4285F4?style=for-the-badge&logo=googlemaps&logoColor=white)
![Geoapify](https://img.shields.io/badge/Geoapify-2C7A7B?style=for-the-badge&logo=mapbox&logoColor=white)
![Clerk](https://img.shields.io/badge/Clerk-6C47FF?style=for-the-badge&logo=clerk&logoColor=white)

* **Database:** Serverless PostgreSQL via **NeonDB**.
* **Authentication:** **Clerk** — Email/Password + Google OAuth.
* **Payments:** **Stripe** — secure card & multi-method payments.
* **Maps & Location:** **Google Maps & Places API** for rendering maps, directions, and autocomplete.
* **Map Rendering:** **Geoapify** for advanced map visualizations.

---

## 📁 Project Structure

```text
ryde/
├── app/                        # Expo Router screens & navigation
│   ├── (auth)/                 # Auth screens (sign-in, sign-up, verify)
│   ├── (root)/                 # Main app screens (home, ride, confirm, history)
│   └── _layout.tsx             # Root layout & providers
│
├── components/                 # Reusable UI components (Map, RideCard, Button…)
│
├── constants/                  # Static config (images, icons, colors)
│
├── lib/                        # Helper functions & service layer
│   ├── map.ts                  # Google Maps / Geoapify helpers
│   ├── stripe.ts               # Stripe client setup
│   └── fetch.ts                # API fetcher
│
├── store/                      # Zustand global state (user, ride, location)
│
├── types/                      # TypeScript type definitions
│
├── assets/                     # Fonts, images, icons
│
├── screenshots/                # App screenshots for README
│
├── .env                        # Environment variables (not committed)
├── app.json                    # Expo app configuration
├── tailwind.config.js          # NativeWind / Tailwind config
├── tsconfig.json               # TypeScript config
└── README.md                   # Project documentation
```

---

## 🚀 Quick Start & Installation

Follow these steps to set up the project locally on your machine.

### Prerequisites

Make sure you have the following installed:

* **Git**
* **Node.js**
* **npm** (Node Package Manager)
* **Expo Go** app (on your Android/iOS device)

---

### Cloning the Repository

```bash
git clone https://github.com/waleedkhokar/Rdye.git
cd Rdye
```

### Installation

Install the project dependencies using npm:

```bash
npm install
```

### Set Up Environment Variables

Create a new file named `.env` in the root of your project and add the following:

```env
EXPO_PUBLIC_CLERK_PUBLISHABLE_KEY=

EXPO_PUBLIC_PLACES_API_KEY=
EXPO_PUBLIC_DIRECTIONS_API_KEY=

DATABASE_URL=

EXPO_PUBLIC_SERVER_URL=https://uber.dev/

EXPO_PUBLIC_GEOAPIFY_API_KEY=

EXPO_PUBLIC_STRIPE_PUBLISHABLE_KEY=
STRIPE_SECRET_KEY=
```

Replace the placeholder values with your actual **Clerk**, **Stripe**, **NeonDB**, **Google Maps**, and **Geoapify** credentials. You can obtain these credentials by signing up on the Clerk, Stripe, NeonDB, Google Maps, and Geoapify websites respectively.

### Running the Project

```bash
npx expo start
```

Download the **Expo Go** app and scan the QR code on your device to view the project.



## 👨‍💻 Developer

**Waleed Khokhar**

### *Full-Stack AI Engineer*

Full-Stack Developer with 1+ year of experience building scalable **Web Applications** and **mobile apps (Android & iOS)** with AI-powered features. Specializing in making intelligent AI solutions and products using **Generative AI, LLMs, Agentic AI, RAG, and LangChain automation**, alongside expert proficiency in **Next.js, MERN stack, and Python/FastAPI backends**.

## 🌐 Connect With Me

<div align="center">

[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://waledkhokar.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/waleedkhokhar)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/waleedkhokar)

</div>


## 📄 License

Currently a personal/private portfolio and development project.

---

⭐ **If you liked this project, drop a ⭐ on the repo and share it with others!**