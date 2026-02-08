# National Lottery Portal Website

A simple and responsive **Lottery Portal Website** built using **HTML, CSS, and JavaScript**.  
This project simulates an official lottery system where users can generate lottery tickets, make a fake payment, and verify their ticket result.

The website contains animations, mobile responsiveness, validation rules, and a ticket verification lock system.

---

## Features

### Login System (index.html)
- User enters **Full Name**
- User enters **Login ID**
- Login ID is validated to be exactly 6 digits
- Redirects user to ticket verification page

### Ticket Generation System (generate.html)
- User enters:
  - Full Name
  - Age
  - Aadhaar Number (12 digits validation)
- Ticket price fixed: **₹500**
- Payment options:
  - UPI (Paytm, PhonePe, Google Pay, Other UPI)
  - Credit / Debit Card
- Displays fake QR code
- Starts 60 seconds payment timer
- After payment completion:
  - Generates a random 6-digit lottery ticket number
  - Generates Login ID as last 6 digits of Aadhaar number
  - Generates a random claim deadline date within 15 days
- Provides buttons to:
  - Go to Login Page
  - Go to Ticket Verification Page

### Ticket Verification System (lottery.html)
- User enters lottery ticket number
- Winning ticket number is taken from generated ticket
- Verifies ticket and displays result
- **One verification attempt only per User ID**
- If user wins:
  - Displays prize: $1,000,000
  - Converts to INR (₹83,000,000 approx)
  - Shows withdrawal instructions

---

## Project Structure

National-Lottery-Portal/
│
├── index.html # Login page
├── generate.html # Ticket generation + payment page
├── lottery.html # Ticket verification page
└── README.md # Project documentation

---

## Technologies Used
- HTML5
- CSS3
- JavaScript (Vanilla JS)

---

---

## How the System Works

### Step 1: Generate Lottery Ticket
- Open `index.html`
- Click **Generate your lottery ticket**
- Fill details and complete fake payment
- After 60 seconds, a ticket number is generated

### Step 2: Login
- Go back to login page
- Enter your name and login ID
- Login ID = last 6 digits of Aadhaar number

### Step 3: Verify Ticket
- Enter lottery ticket number
- The system checks if it matches winning ticket number
- If matched, user wins

---

## Important Notes
- This project is only a **simulation**.
- The payment QR code is fake and for UI demonstration.
- Ticket verification is stored in browser using `localStorage`.
- Clearing browser storage resets the system.

---

## Future Improvements (Optional)
- Database integration (MySQL / Firebase)
- Real authentication system
- Admin panel to control winning ticket number
- Transaction receipt generation
- Backend support using Node.js / Java / Python

---

## Author
Developed by **Darshan Gowda**

---
acess the website:https://darshan-code11.github.io/National-Lottery-Portal-Website/lottery.html

## License
This project is for educational purposes only.


