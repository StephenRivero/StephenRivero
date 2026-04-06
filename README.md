# Stephen Manasseh R. Pastor

## Front-End Developer

[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-007ACC?style=for-the-badge&logo=vercel&logoColor=white)](https://stephenrivero.vercel.app)

---

## About Me

Passionate Front-End Developer with expertise in building responsive, user-friendly web applications. Based in Taguig City, Metro Manila.

**Contact:**
- Email: stephen.m.rivero@gmail.com
- Phone: (+63)991-531-1151

---

## Work Experience

### Front-End Engineer | BETRNK Tours Inc. (BGC, Taguig)
**August 2025 – Present**

- Build front-end UI/UX of B-ticket website and its admin/merchant dashboard B-merchant
- Utilize AI agents such as Claude Code and Augment Code to accelerate feature development
- Integrate data from RESTful APIs with the help of Postman
- Convert UI/UX designs from Figma into front-end code with Responsive Design
- **Tech Stack:** Next.js, React.js, Redux, TypeScript, JavaScript (ES6), Shadcn, Tailwind CSS, Zod

### Front-End Web Developer | TRYCAN SOFT CO. (BGC, Taguig)
**Jan. 2024 – July 2025 (1.5 years)**

- Build front-end UI/UX of E-commerce with admin dashboard websites
- Integrate data from RESTful APIs with the help of Postman
- Convert UI/UX designs from Adobe and Figma into front-end code with Responsive Design
- **Tech Stack:** Next.js, React.js, TypeScript, JavaScript (ES6), SCSS, Tailwind CSS

### Front-End Web Developer | REALHOLMES PROPERTY INC.
**Jan. 2022 – Jan. 2024 (2 years)**

- Build front-end UI/UX of the Realholmes Property Inc. website
- Convert UI/UX designs from Figma into front-end code with Responsive Design
- **Tech Stack:** Tailwind CSS, Alpine.js, Laravel, Livewire (TALLSTACK)

---

## Skills

| Category | Technologies |
|----------|--------------|
| **Languages** | HTML5, CSS3, JavaScript ES6, TypeScript |
| **Frameworks** | React.js, Next.js, Laravel |
| **Styling** | Tailwind CSS, SCSS, Material UI, Framer Motion |
| **State Management** | Redux, Context API |
| **Validation** | Zod |
| **API** | REST API integration, Postman |
| **Version Control** | Git, Bitbucket, GitHub, GitLab |
| **Deployment** | Vercel |
| **Project Management** | Jira (Scrum/Agile) |
| **IDE** | Visual Studio Code, WebStorm, IntelliJ |

---

## Education

| Institution | Course | Duration |
|-------------|--------|----------|
| Udemy | The Ultimate React Course 2025: React, Next.js, Redux & More | Feb 2025 – Present |
| The Odin Project | Free Online Web Development Course | Oct 2021 – Present |
| De La Salle University – Dasmariñas | B.S. in Environmental & Sanitary Engineering | 2009 – 2014 |

---

## Featured Project

# The Wild Oasis - Luxury Cabin Booking Website

A Next.js 14 application for a luxury cabin resort located in the Italian Dolomites. The app allows guests to browse cabins, make reservations, and manage their bookings.

## Features

### 🏠 Homepage
- Full-screen hero background image
- Welcome message: "Welcome to paradise"
- Call-to-action button linking to cabins page

### 🏡 Cabins Listing (`/cabins`)
- Display all available luxury cabins
- **Filtering by capacity:** All cabins, Small (1-3 guests), Medium (4-7 guests), Large (8-12 guests)
- Cabin cards showing: Image, Name, Capacity, Price (with discount applied)
- Reservation reminder for logged-in users

### 🛏️ Cabin Details (`/cabins/[cabinid]`)
- Full cabin information: Image gallery, Name and description, Maximum capacity, Regular price and discount
- Interactive reservation form: Date selector (blocks booked dates), Guest count selector, Observations field, Real-time price calculation

### 👤 User Authentication
- **Google OAuth** via NextAuth.js
- Automatic guest creation on first sign-in
- Session management with guest ID
- Protected routes for account area

### 👤 Guest Account (`/account`)
- Welcome message with user's first name
- Access to profile and reservations

### 📋 Profile Management (`/account/profile`)
- Update guest profile information: Nationality (country selector with flag), National ID (validated: 6-12 alphanumeric characters)
- Server-side form validation
- Profile update via Supabase

### 📅 My Reservations (`/account/reservations`)
- List all user's reservations with cabin name, image, dates, number of nights, guests, total price, booking status
- **Edit reservations:** Modify number of guests, add/modify observations
- **Delete reservations:** Remove bookings with authorization check

### ✅ Booking Confirmation (`/cabins/thankyou`)
- Thank you page after successful booking

### ℹ️ About Page (`/about`)
- Property description, Family history (since 1962), Images, Dynamic cabin count display

## Technology Stack

| Category | Technology |
|----------|------------|
| **Framework** | Next.js 14 (App Router) |
| **Language** | JavaScript |
| **Authentication** | NextAuth.js (Google Provider) |
| **Database** | Supabase (PostgreSQL) |
| **Styling** | Tailwind CSS |
| **Date Handling** | date-fns, react-day-picker |
| **Icons** | Heroicons React |
| **Fonts** | Geist (Variable) |

## Project Structure

```
the-wild-oasis-website/
├── app/
│   ├── _components/          # Reusable UI components
│   ├── _lib/                 # Core utilities (actions.js, auth.js, data-service.js, supabase.js)
│   ├── _styles/
│   ├── account/              # Protected account routes
│   ├── cabins/               # Cabins listing & details
│   ├── login/                # Login page
│   ├── about/                # About page
│   ├── layout.js
│   └── page.js
├── public/                   # Static assets
├── tailwind.config.js
└── package.json
```

## Database Schema (Supabase)

- **cabins**: id, name, maxCapacity, regularPrice, discount, description, image
- **guests**: id, email, fullName, nationality, countryFlag, nationalID
- **bookings**: id, created_at, startDate, endDate, numNights, numGuests, cabinPrice, extrasPrice, totalPrice, status, hasBreakfast, isPaid, guestId, cabinId
- **settings**: id, minBookingLength, maxBookingLength, breakfastPrice

## Environment Variables

```env
# NextAuth
AUTH_SECRET=your-nextauth-secret
AUTH_GOOGLE_ID=your-google-client-id
AUTH_GOOGLE_SECRET=your-google-client-secret

# Supabase
NEXT_PUBLIC_SUPABASE_URL=your-supabase-url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your-supabase-anon-key
```

## Getting Started

```bash
# Install dependencies
npm install

# Set up environment variables
# Create .env.local with your Supabase and Google OAuth credentials

# Run development server
npm run dev

# Open in browser
Visit http://localhost:3000
```

## Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm run start` | Start production server |
| `npm run prod` | Build and start production |
| `npm run lint` | Run ESLint |

---

## Portfolio

🌐 **Live Portfolio:** [stephenrivero.vercel.app](https://stephenrivero.vercel.app)

---

## Let's Connect

I'm open to collaboration and new opportunities. Feel free to reach out!

- Email: stephen.m.rivero@gmail.com
- Location: Taguig City, Metro Manila
