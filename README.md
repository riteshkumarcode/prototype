# CarePulse Hospital — Interactive Prototype Website

> A multi-speciality hospital and tertiary healthcare prototype web application designed for client demonstrations, user testing, and instant deployment on **Netlify**.

---

## 🚀 Live Netlify Deployment

This repository is pre-configured for **Netlify** with zero build configuration required:
- **Root Entry Point:** `index.html`
- **SPA Routing Redirects:** `_redirects` (`/*  /index.html  200`)
- **Headers & Security Config:** `netlify.toml` (X-Frame-Options, XSS protection, Cache-Control, and clean routing)

### 3 Ways to Deploy to Netlify:

1. **Option 1: Connect via GitHub (Recommended)**
   - Go to [app.netlify.com](https://app.netlify.com/)
   - Click **"Add new site"** → **"Import an existing project"**
   - Select **GitHub** and choose this repository (`riteshkumarcode/prototype`)
   - Leave build command blank and publish directory as `.` or root.
   - Click **"Deploy site"** — your live hospital website will be live in 10 seconds!

2. **Option 2: Netlify Drop (Drag & Drop)**
   - Open [app.netlify.com/drop](https://app.netlify.com/drop)
   - Drag and drop this folder (`prototype`) into the browser window.
   - It will deploy instantly with a live URL.

3. **Option 3: Netlify CLI**
   ```bash
   npm install -g netlify-cli
   netlify deploy --prod --dir=.
   ```

---

## 🌟 Key Features & Client Workflows

### 1. Interactive 5-Step Appointment Booking Stepper (`#/book-appointment`)
- **Step 1:** Select from 18+ Medical Specialities (Cardiology, Orthopaedics, Neurology, Obs & Gynae, Paediatrics, etc.).
- **Step 2:** Choose a Specialist Doctor (with doctor photo, qualifications, consulting fee, languages, and OPD days) or select *"Any available doctor (earliest appointment)"*.
- **Step 3:** Choose Hospital Campus, Date (next 10 days with automated Sunday/off-day blocking), and Preferred Time Slot (morning and evening slots with full/booked indications).
- **Step 4:** Patient Details Form with a **⚡ "Autofill Test Patient Data"** button for instant 1-click testing by clients, plus flexible mobile phone validation supporting local and international formats (`+91`, spaces, hyphens).
- **Step 5:** Instant Confirmation Pass with unique reference number (e.g. `CP-892410`), **📅 "Add to Google Calendar"** button, **🖨️ "Print Confirmation Pass"** button, and direct navigation links.
- **Clickable Stepper:** Steps 1–3 in the top progress bar are clickable to jump backwards smoothly.

### 2. Real-Time Doctor Search & Filtering (`#/doctors`)
- Live text search by doctor name or condition.
- Filter dropdowns by **Speciality**, **Hospital Campus / Branch**, and **OPD Day of Week**.
- Results count badge and clean empty state fallback.
- Comprehensive Doctor Profile (`#/doctors/:id`) with clinical bio, areas of expertise pills, procedures performed, education, medical council registration, and interactive weekly OPD schedule table highlighting "Today".

### 3. 24/7 Emergency Care Center (`#/emergency-care`)
- High-visibility Red Alert banner with 1-tap emergency dialer (`1800-202-9999`).
- Campus ER entrance landmarks, ambulance direct hotline, and Google Maps navigation.
- Emergency protocol triage guide and "what to bring" checklist.

### 4. Interactive Insurance & Cashless Checker (`#/patient-information/insurance`)
- Real-time search against 20+ insurance companies, TPAs, and Government Health Schemes (CGHS, DGEHS, ECHS, PM-JAY, Star Health, HDFC ERGO, ICICI Lombard, Niva Bupa, Medi Assist, Paramount, etc.).
- Instant verification badge showing empanelment status, required documents, and dedicated TPA helpdesk extension.
- Step-by-step visual guide to cashless pre-authorisation and discharge settlement.

### 5. Preventive Health Checkup Packages (`#/health-packages`)
- Category filter chips: **All**, **Full Body**, **Women's Health**, **Men's Health**, **Senior Citizen**, **Cardiac Care**, and **Diabetes**.
- Package cards showing included test count, pre-test preparation/fasting instructions, and transparent pricing.
- One-click **"Enquire / Book"** buttons that automatically pre-fill the inquiry form with the package name.

### 6. Interactive Hospital Brand Customizer
- Floating top prototype toolbar includes **"✏️ Customize Hospital Name"**.
- The client can enter any hospital name (e.g. *"Apex Health City"*, *"Metro Memorial Hospital"*), and the entire prototype dynamically updates across all headers, titles, footers, booking passes, and 30+ pages in real time!
- Persists via `localStorage` so changes remain during client walkthroughs.

### 7. Complete Prototype Sitemap & Map (`#/prototype-map`)
- Directory of all 30+ pages and 6 core patient journey walkthrough cards with 1-click test links.

---

## 📱 Mobile-First Responsive Design
- Clean, accessible typography using Google Fonts (Manrope for headlines and Inter for clean body text).
- Responsive Mega Menu for desktop body systems (Heart, Brain, Bones, Women, Children, Kidney, Gut, Critical Care).
- Smooth mobile slide-out navigation drawer with quick book and emergency buttons.
- Sticky bottom mobile action bar (Call Emergency, Book Appointment, Get Directions).
- High contrast, WCAG AA accessible color scheme (Clinical Navy, Healthcare Teal, Amber Accent, Alert Red, Ivory & Stone surfaces).

---

## 🛠️ Project Structure

```text
prototype/
├── index.html                     # Primary entry point (optimized for Netlify)
├── hospital-website-prototype.html# Mirror template file
├── _redirects                     # Netlify SPA redirect rules (/* /index.html 200)
├── netlify.toml                   # Netlify build and security headers configuration
└── README.md                      # Documentation and deployment guide
```

---

## 📄 License
Prototype template for presentation, client review, and production customization.
