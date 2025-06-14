# 🍋 Little Lemon Frontend Web Application

This is the frontend for **Little Lemon**, a fictional Mediterranean restaurant. Developed as part of the **Meta Front-End Developer Capstone Project**, this React-based application allows customers to make table reservations and explore the restaurant experience online.

---

## 🚀 Project Overview

The core of this application is a **table reservation form** with a smooth, responsive UI, built using modern React practices. It communicates with a Django REST API backend to submit and retrieve booking data.

---

## 🧰 Tech Stack

- **JavaScript**
- **React**
- **CSS**
- **HTML**

---

## 🧱 Project Structure

```
Little-Lemon-FrontWeb/
├── public/
│   ├── favicon.svg
│   ├── index.html
│   ├── Logo.svg
│   ├── manifest.json
│   └── robots.txt
│
├── src/
│   ├── assets/                # Static images and illustrations
│   │   └── [*.jpg, *.svg, *.png]
│   │
│   ├── components/            # UI components
│   │   ├── Footer/
│   │   ├── Header/
│   │   ├── Main/
│   │   ├── Navbar/
│   │   ├── OrderOnline/
│   │   └── Reservations/
│   │
│   ├── constants/             # Hardcoded data (e.g., images, text)
│   │   ├── headerData.js
│   │   ├── images.js
│   │   ├── orderOnline.js
│   │   └── reservationData.js
│   │
│   ├── utilities/             # API helpers
│   │   └── API.js
│   │
│   ├── wrapper/               # Reusable layout wrappers
│   │   ├── AppWrap.js
│   │   ├── AppWrapper.css
│   │   └── index.js
│   │
│   ├── App.js                 # Main app logic
│   ├── App.css                # Global styles
│   ├── App.test.js
│   ├── DataContext.js         # Context provider for app state
│   ├── index.js               # App entry point
│   ├── index.css              # App-wide base styles
│   ├── setupTests.js
│   └── reportWebVitals.js
│
├── package.json
├── package-lock.json
└── README.md
```

---

## 📬 Reservation Form Features

The table booking form (under `Reservations/`) includes:

- Input fields for name, date, number of guests, and comments
- Validation for required fields
- Submission via Axios to the `/restaurant/api/book/` backend endpoint
- Conditional UI messages for success/failure
- Uses shared state through `DataContext.js`

---

## 💪 Testing

React testing setup via `setupTests.js`. Unit and component tests can be written in `App.test.js` or extended to component-level files using:

```bash
npm test
```

---

## 📜 License

This project is licensed under the **MIT License**. See the [LICENSE](./LICENSE) file for details.
