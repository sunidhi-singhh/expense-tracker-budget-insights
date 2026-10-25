# expense-tracker-budget-insights
Modern, responsive personal finance dashboard with real-time budget insights, category limits, Recharts analytics, and Firebase integration. Web Development Internship project for Codec Technologies.
# Expense Tracker with Budget Insights

> **Web Development Internship Project**  
> Developed for **Codec Technologies**  
> **Author:** Sunidhi Singh  
> **Tech Stack:** React 18, Vite, Tailwind CSS, Recharts, Lucide Icons, Firebase Auth & Firestore

---

## 🌟 Project Overview

**Expense Tracker with Budget Insights** is a responsive, modern personal finance web application built to help individuals monitor income, track daily expenditures, establish category-specific monthly budget caps, and visualize spending habits through interactive analytical charts.

The application features a responsive design (desktop sidebar navigation and mobile-friendly drawer navigation), dual-mode data persistence (seamless Firebase Cloud Firestore with a 1-click Local Demo Mode fallback), CSV statement exports, printable financial summaries, and real-time threshold warnings (80% warning and 100% exceeded budget alerts).

---

## 🚀 Key Features

### 1. 📊 Financial Dashboard
- **Real-time Summary Cards:** Live display of Monthly Income, Monthly Expenses, Net Monthly Savings (with savings rate %), and Remaining Budget.
- **Income vs. Expense Analytics:** Interactive month-over-month comparison bar chart with custom hover tooltips.
- **Category Spending Doughnut Chart:** Breakdown of current month spending with percentage distribution and categorized color coding.
- **Recent Transactions:** Quick-access list showing transaction badges, dates, payment methods, and inline Edit/Delete actions.
- **Smart Budget Alert Banner:** Prominent warning banner triggered dynamically when total or category spending hits 80% or exceeds the allocated budget.

### 2. 💳 Transaction Management
- **Add Income & Expense:** Modal accessible from anywhere in the app with field validation (title, positive amount > 0, category, date, payment method, optional notes).
- **Edit & Delete Records:** Instant updates to dashboard totals, charts, and budget progress bars.
- **Confetti Celebration:** Festive animation triggered upon recording income or staying within budget targets.

### 3. 📜 Transaction History & Filtering
- **Multi-Filter Engine:** Filter records by transaction type (Income / Expense), category, or date range presets (*All Time*, *This Month*, *Last Month*, *Last 30 Days*, or *Custom Start/End Dates*).
- **Live Search:** Instant search across transaction titles and notes.
- **Flexible Sorting:** Sort by Date (newest/oldest), Amount (highest/lowest), or Title (A–Z).
- **Responsive Table & Mobile Cards:** Clean table on desktop and compact card layout on mobile screens with pagination controls.

### 4. 🎯 Budget Management & Insights
- **Overall Monthly Budget:** Set and adjust overall monthly expenditure targets.
- **Category-Wise Spending Limits:** Define quotas for Food & Dining, Rent, Utilities, Transport, Entertainment, Shopping, Healthcare, etc.
- **Visual Progress Gauges:** Color-coded progress bars:
  - 🟢 **Normal / Healthy:** Spending < 80% of budget.
  - 🟡 **Warning Threshold:** Spending between 80% and 99% (prompts user to slow down).
  - 🔴 **Exceeded Threshold:** Spending ≥ 100% (urgent alert with overbudget delta).

### 5. 📑 Reports, CSV Export & Printable Statements
- **Financial Trend Area Chart:** Cumulative cash flow and net savings trajectory.
- **Category Breakdown Table:** Detailed spending volume, transaction count, and percentage contribution.
- **CSV Data Export:** One-click download of all or filtered transactions formatted with standard headers.
- **Printable Monthly Summary:** Clean, printer-optimized statement (`window.print()`) featuring internship metadata, user details, key financial metrics, category breakdown, and signature section.

### 6. 🔐 Authentication & Multi-Tenant Security
- **Firebase Authentication:** Secure email/password registration, login, and Google Sign-in.
- **Multi-Tenant User Isolation:** Each user's financial records are stored under `users/{userId}/transactions` and protected by Firestore Security Rules.
- **1-Click Reviewer Demo Mode:** Allows internship evaluators to test all features immediately without entering Firebase credentials or configuring API keys.

### 7. ⚙️ Settings & Customization
- **Currency Selection:** Instant switching between **INR (₹)**, **USD ($)**, **EUR (€)**, **GBP (£)**, **CAD (CA$)**, **AUD (AU$)**, **JPY (¥)**, and **SGD (S$)**.
- **Dark / Light Theme Toggle:** Smooth visual transition with preference persisted in `localStorage`.
- **Display Profile Management:** Update user display name.
- **Demo Data Reset:** Easily restore the default realistic internship dataset or wipe records for clean testing.

---

## 🛠️ Technology Stack

| Layer | Technologies |
|---|---|
| **Frontend Framework** | React.js (v18) with Vite 6 |
| **Styling** | Tailwind CSS v3, PostCSS, Autoprefixer |
| **Routing** | React Router DOM v6 |
| **Icons** | Lucide React |
| **Data Visualization** | Recharts (Responsive Bar, Doughnut, and Area charts) |
| **Backend & Database** | Google Firebase Authentication & Cloud Firestore |
| **Local Storage** | Fallback service layer with automatic mock data seeding |
| **Animations & FX** | Canvas Confetti, Tailwind Transition Animations |

---

## 💻 Installation & Local Setup

### 1. Clone the Repository
```bash
git clone https://github.com/sunidhi-singhh/expense-tracker-budget-insights.git
cd expense-tracker-budget-insights
