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

## 🌟 Key Features & Enhancements

### 1. Modern Healthcare Brand Logo
- **Dual-Tone Medical Emblem**: SVG mark with curved shield, clinical cross silhouette, white ECG heartbeat pulse line, and emerald life recovery dot.
- **Refined Typography**: `CarePulse` in bold display lettering with a high-contrast `SUPER-SPECIALITY` badge.
- **Interactive Brand Customizer**: Click **"✏️ Customize Hospital Name"** in the top demo bar to change the brand live across all 30+ pages.

### 2. Interactive Home Hero Slider
- **4 Auto-Advancing High-Impact Slides**:
  1. *Compassionate & World-Class Specialist Care* (NABH/NABL accreditation, 16 specialists on duty).
  2. *24/7 Level-1 Emergency & Trauma Care* (Golden hour response, zero paperwork delays, 65 ICU beds).
  3. *Advanced Robotic & Minimally Invasive Surgery* (12 sterile modular laminar flow operating suites).
  4. *Comprehensive Preventive Health Checkups* (Packages from ₹1,899, same-day reports, 68 tests).
- **Interactive Controls**: Previous/Next frosted glass arrows, progress dot indicators, auto-play with pause-on-hover, and smooth cross-fade animation.

### 3. Enhanced Desktop & Mobile Navigation
- **Specialities Mega-Menu (`#mega`)**:
  - 4-column categorized layout organized by anatomical system (Heart & Vascular, Neurosciences, Orthopaedics, Women's Care, Child Care, Renal & Urology, Lungs & Critical Care, General Surgery).
  - Doctor counts per department and direct 24/7 cardiac & stroke emergency hotline strip.
- **Patients & Visitors Dropdown (`#patientDD`)**:
  - Direct quick-links to Cashless Insurance (20+ TPAs), Visiting Hours, Admission/Discharge Guide, Billing & Estimates, and Medical Records.
- **Enhanced Mobile Drawer**:
  - Branded header, accordion expandable submenus for Specialities and Patient Guides, 1-click consultation booking, and emergency callout.

### 4. Interactive 5-Step Appointment Booking Stepper (`#/book-appointment`)
- **Step 1:** Select from 18+ Medical Specialities.
- **Step 2:** Choose a Specialist Doctor (photo, qualifications, fee, languages, OPD days) or select *"Any available doctor"*.
- **Step 3:** Campus selector, 10-day date picker with Sunday off-day blocking, and morning/evening time slot picker.
- **Step 4:** Patient Details Form with a **⚡ "Autofill Test Patient Data"** button for instant 1-click client testing, plus flexible international and local phone number validation (`+91`, spaces, hyphens).
- **Step 5:** Instant Confirmation Pass with unique reference ID (e.g. `CP-892410`), **📅 Add to Google Calendar**, and **🖨️ Print Confirmation Pass** button.
- **Clickable Stepper:** Completed steps (1–3) in the progress bar are clickable to jump backwards anytime.

### 5. Real-Time Doctor Search & Filtering (`#/doctors`)
- Live text search by doctor name or condition.
- Filter dropdowns by **Speciality**, **Hospital Campus / Branch**, and **OPD Day of Week**.
- Results count badge and clean empty state fallback.
- Comprehensive Doctor Profile (`#/doctors/:id`) with clinical bio, areas of expertise pills, procedures performed, education, registration, and weekly OPD schedule table highlighting "Today".

### 6. Interactive Cashless & Insurance Checker (`#/patient-information/insurance`)
- Real-time search against 20+ insurance companies, TPAs, and Government Health Schemes (CGHS, DGEHS, ECHS, PM-JAY, Star Health, HDFC ERGO, ICICI Lombard, Niva Bupa, Medi Assist, etc.).
- Instant verification badge showing empanelment status, required documents, and dedicated TPA helpdesk extension.
- Step-by-step visual guide to cashless pre-authorisation and discharge settlement.

### 7. Preventive Health Checkup Packages (`#/health-packages`)
- Category filter chips: **All**, **Full Body**, **Women's Health**, **Men's Health**, **Senior Citizen**, **Cardiac Care**, and **Diabetes**.
- Package cards showing included test count, pre-test preparation/fasting instructions, and transparent pricing.
- One-click **"Enquire / Book"** buttons that automatically pre-fill the inquiry form with the package name.

### 8. Complete Prototype Sitemap & Map (`#/prototype-map`)
- Directory of all 30+ pages and 6 core patient journey walkthrough cards with 1-click test links.

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
