# 🎓 Conflict-Free Student Timetable & Schedule Checker

A lightweight, responsive, client-side web application designed to help students manage their weekly academic schedules while **automatically preventing time conflicts**. 

No backend server, database, or complex build process is required—just open it in a browser and start scheduling!

---

## ✨ Features

* **Automated Conflict Detection:** Real-time validation checks ensure you never accidentally double-book yourself during the same time slot on any day of the week.
* **Interactive Weekly Grid:** A clean, color-coded timetable layout covering Monday through Friday from 9:00 AM to 5:00 PM.
* **Course Management:** 
  * Add custom courses with names, codes, rooms/halls, days, and exact hourly time blocks.
  * Easily remove unwanted or changed classes with a single click.
* **Pre-populated Sample Schedule:** Comes loaded with a sample schedule out-of-the-box so you can see how it works instantly.
* **Fully Responsive:** Adapts seamlessly to desktop monitors, tablets, and mobile devices.

---

## 🛠️ Tech Stack

* **HTML5** – Semantic document structure
* **CSS3** – Modern styling with CSS Grid, Flexbox, and CSS Custom Properties (Variables)
* **JavaScript (ES6+)** – Core state management, dynamic DOM rendering, and interval overlap algorithms

---

## 🚀 Getting Started

### Prerequisites
All you need is a modern web browser (Google Chrome, Mozilla Firefox, Microsoft Edge, Safari, etc.).

### Installation & Usage
1. **Clone or Download** the project files to your local machine.
2. Save the main code file as `index.html`.
3. **Double-click** `index.html` (or open it via your favorite browser) to launch the app instantly.

---

## 🧠 How the Conflict Detection Works

When you submit a new course, the application converts all time strings into minutes from midnight. It then evaluates your proposed time block against existing classes on the same day using the classic **interval overlap condition**:

$$\max(\text{Start}_1, \text{Start}_2) < \min(\text{End}_1, \text{End}_2)$$

If an overlap is detected, the submission is blocked and an informative alert notification displays the conflicting course details.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).