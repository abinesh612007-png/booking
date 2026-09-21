# ✈️ TravelHub

> **Your Plans. One Place.**

TravelHub is a modern, responsive travel platform landing page that brings **travel planning, hotel stays, and movie ticket discovery** together in one unified experience.

The project is designed with a clean, modern UI and includes interactive booking forms, destination cards, hotel listings, movie cards, an FAQ section, and an early-access/contact form.

---

## 🌐 Overview

TravelHub aims to provide users with a single place to:

* ✈️ Search for travel options
* 🏨 Find and explore hotels
* 🎬 Search for movies
* 📍 Explore popular destinations
* 📋 Manage booking-related actions
* 📩 Register for early access
* ❓ Get answers through an FAQ section

The homepage uses the tagline:

**"Travel, stay, and movie tickets — all in one place."**

---

## ✨ Features

### ✈️ Travel Search

Users can enter:

* Departure city
* Destination city
* Travel date
* Number of travellers

The interface also includes a **From ↔ To swap button** for quickly switching the departure and destination fields.

### 🏨 Hotel Search

The hotel booking interface allows users to enter:

* Destination
* Check-in date
* Check-out date
* Number of guests and rooms

The checkout date is automatically restricted based on the selected check-in date.

### 🎬 Movie Search

Users can search for movies by:

* City
* Movie name
* Date

Supported example cities include Mumbai, Delhi, Bangalore, Chennai, Hyderabad, Pune, Kolkata, Ahmedabad, Jaipur, and Goa.

### 📍 Popular Destinations

The landing page showcases popular Indian destinations including:

* Goa
* Manali
* Kerala
* Rajasthan
* Mumbai
* Delhi

### 📱 Responsive Design

The website is designed to work across:

* Desktop
* Tablet
* Mobile

The layout automatically adapts grids, navigation, booking forms, cards, and footer content for smaller screens.

### 📋 Interactive Booking Tabs

The booking component contains three tabs:

```text
Travel | Hotels | Movies
```

Switching between tabs dynamically displays the corresponding search form.

### ❓ FAQ Accordion

The FAQ section uses an interactive accordion where users can expand one question at a time.

It also supports keyboard interaction using:

* `Enter`
* `Space`

### 📩 Early Access Form

The early-access form collects:

* Name
* Email
* Phone number

Client-side validation is included for all three fields.

The form is configured to submit the data to a **Google Apps Script endpoint**.

---

## 🛠️ Tech Stack

This project is built using lightweight frontend technologies:

* **HTML5**
* **CSS3**
* **Vanilla JavaScript**
* **Google Apps Script** for the early-access form
* **Google Fonts – Inter**
* **Unsplash** for placeholder imagery

No frontend framework is required.

---

## 🎨 Design System

TravelHub uses a centralized CSS design-token system.

### Primary Colors

| Token         | Value     |
| ------------- | --------- |
| Primary       | `#2563EB` |
| Primary Hover | `#1D4ED8` |
| Accent        | `#F59E0B` |
| Success       | `#10B981` |
| Error         | `#EF4444` |
| Dark          | `#0B1426` |
| Background    | `#FFFFFF` |

The project also uses reusable values for:

* Border radius
* Shadows
* Typography
* Spacing
* Transitions
* Maximum content width

---

## 📂 Project Structure

A simple deployment can use a single HTML file:

```text
TravelHub/
│
├── index.html
└── README.md
```

The current implementation contains the HTML, CSS, and JavaScript inside the main HTML document.

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

### 2. Navigate to the project

```bash
cd YOUR_REPOSITORY
```

### 3. Open the website

You can simply open:

```text
index.html
```

in your browser.

For development, you can also use a local server such as VS Code Live Server.

---

## ⚙️ Configuration

The booking integrations are currently represented by configurable JavaScript variables:

```javascript
const TRAVEL_BOOKING_URL = "";
const HOTEL_BOOKING_URL  = "";
const MOVIE_BOOKING_URL  = "";
```

Replace these values with your actual booking URLs when your backend or booking providers are ready.

For example:

```javascript
const TRAVEL_BOOKING_URL = "https://example.com/travel";
const HOTEL_BOOKING_URL  = "https://example.com/hotels";
const MOVIE_BOOKING_URL  = "https://example.com/movies";
```

If a booking URL is not configured, the interface displays a temporary searching state instead of redirecting the user.

---

## 📩 Early Access Form

The early-access form is connected to a Google Apps Script endpoint.

The frontend sends:

```text
name
email
phone
```

using a GET request.

Before submission, the form validates:

* Name length
* Email format
* Indian phone number format

After a successful submission, the form displays a success message and resets the form.

---

## 🔒 Important Security Note

If you fork this repository, review the Google Apps Script endpoint and any external integrations before deploying the project publicly.

For a production application, sensitive credentials, API keys, and private backend configuration should **not** be stored directly in client-side JavaScript.

---

## 🖼️ Images

The current design uses external Unsplash images as placeholder/visual assets for destinations and the hero section.

For production use, consider replacing them with:

* Optimized local images
* CDN-hosted assets
* Properly licensed photography
* WebP/AVIF images for better performance

---

## 📱 Responsive Breakpoints

The stylesheet includes responsive layouts for:

```text
Desktop
   ↓
1024px
   ↓
768px
   ↓
480px
```

At smaller widths, navigation changes to a hamburger menu and multi-column layouts collapse into single-column layouts.

---

## 🧩 Interactive Components

The project currently includes:

* Fixed navigation header
* Mobile hamburger menu
* Smooth scrolling
* Booking tabs
* Travel form validation
* Hotel form validation
* Movie form validation
* Travel location swap
* Date restrictions
* Search loading states
* FAQ accordion
* Early-access form validation
* Google Apps Script submission
* Responsive cards and grids

---

## 🚧 Current Limitations

This project is currently primarily a **frontend landing page/prototype**.

The following integrations are placeholders and should be connected to production services:

* Real travel booking API
* Real hotel booking API
* Real movie booking API
* User authentication
* My Bookings functionality
* Payment processing
* Dynamic destination data
* Dynamic hotel data
* Dynamic movie data
* Production backend

---

## 🔮 Future Improvements

Possible future development includes:

* [ ] User authentication
* [ ] Real-time flight/train/bus search
* [ ] Hotel API integration
* [ ] Movie/showtime API integration
* [ ] Payment gateway
* [ ] Booking history
* [ ] User profiles
* [ ] Wishlist functionality
* [ ] Search filters
* [ ] Location-based recommendations
* [ ] Real-time pricing
* [ ] Backend API
* [ ] Database integration
* [ ] Admin dashboard
* [ ] PWA/mobile application

---

## 🚀 Deployment

Because the project is a static frontend, it can be deployed using services such as:

* GitHub Pages
* Vercel
* Netlify
* Cloudflare Pages

For GitHub Pages, push the project to your repository and enable **Pages** from the repository settings.

---

## 📄 License

This project is currently provided for personal/project use.

Add an appropriate open-source license such as **MIT** if you want others to freely use, modify, and distribute the project.

---

## 👨‍💻 Author

**Your Name**

GitHub: `https://github.com/YOUR_USERNAME`

---

## ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub.

---

### Built with ❤️ in India

**TravelHub — Your Plans. One Place.**

URL WEB SITE
https://booking-xi-gules.vercel.app/
