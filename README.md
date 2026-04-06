# Stephen Manasseh R. Pastor

## Front-End Developer

[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-007ACC?style=for-the-badge&logo=vercel&logoColor=white)](https://stephenrivero.vercel.app)

---

## About Me

Passionate Front-End Developer with expertise in building modern, responsive, and user-friendly web applications. Currently working at BETRNK Tours Inc. as a Front-End Engineer, specializing in Next.js, React.js, and TypeScript.

- **Email:** stephen.m.rivero@gmail.com
- **Phone:** (+63)991-531-1151
- **Location:** Taguig City, Metro Manila
- **Portfolio:** [stephenrivero.vercel.app](https://stephenrivero.vercel.app)

---

## Work Experience

### Front-End Engineer | BETRNK Tours Inc. (BGC, Taguig)
**August 2025 – Present**

- Build front-end UI/UX of B-ticket website and its admin/merchant dashboard B-merchant
- Utilize AI agents such as Claude Code and Augment Code to accelerate feature development
- Integrate data from RESTful APIs with Postman
- Convert UI/UX designs from Figma into front-end code with Responsive Design
- **Tech Stack:** Next.js, React.js, Redux, TypeScript, JavaScript (ES6), Shadcn, Tailwind CSS, Zod

### Front-End Web Developer | TRYCAN SOFT CO. (BGC, Taguig)
**Jan. 2024 – July 2025 (1.5 years)**

- Build front-end UI/UX of E-commerce with admin dashboard websites
- Integrate data from RESTful APIs with Postman
- Convert UI/UX designs from Adobe and Figma into front-end code with Responsive Design
- **Tech Stack:** Next.js, React.js, TypeScript, JavaScript (ES6), SCSS, Tailwind CSS

### Front-End Web Developer | REALHOLMES PROPERTY INC.
**Jan. 2022 – Jan. 2024 (2 years)**

- Build front-end UI/UX of the Realholmes Property Inc. website
- Convert UI/UX designs from Figma into front-end code with Responsive Design
- **Tech Stack:** Tailwind CSS, Alpine.js, Laravel, Livewire (TALLSTACK)

---

## Skills

### Languages & Frameworks
- HTML5, CSS3, SASS/SCSS
- JavaScript ES6, TypeScript
- React.js, Next.js
- Redux, Redux Toolkit
- Laravel, Livewire

### Styling & UI
- Tailwind CSS
- Material UI
- Shadcn
- Framer Motion
- Alpine.js

### Tools & Technologies
- REST API integration (Postman)
- Version Control: Git, Bitbucket, GitHub, Gitlab
- Deployment: Vercel
- Project Management: Jira (Scrum/Agile)
- IDE: Visual Studio Code, WebStorm, IntelliJ

### Soft Skills
- Problem Solving
- High Attention to Details
- Sustained Attention/Focus
- Team Work & Independent Work

---

## Education

| Institution | Course | Duration |
|-------------|--------|----------|
| Udemy | The Ultimate React Course 2025: React, Next.js, Redux & More | Feb 2025 – Present |
| The Odin Project | Free Online Web Development Course | Oct 2021 – Present |
| De La Salle University – Dasmariñas | B.S. in Environmental & Sanitary Engineering | 2009 – 2014 |

---

## Projects

### 1. The Wild Oasis - Luxury Cabin Booking Website

🔗 **Live Demo:** [stephens-wild-oasis.vercel.app/](https://stephens-wild-oasis.vercel.app/)

A Next.js 14 application for a luxury cabin resort located in the Italian Dolomites. The app allows guests to browse cabins, make reservations, and manage their bookings.

#### Features

- **Homepage:** Full-screen hero background, welcome message "Welcome to paradise", call-to-action button
- **Cabins Listing:** Display all available luxury cabins with filtering by capacity (Small 1-3, Medium 4-7, Large 8-12 guests), cabin cards showing image, name, capacity, and price with discount
- **Cabin Details:** Full cabin information including image gallery, name, description, maximum capacity, regular price and discount, interactive reservation form with date selector (blocks booked dates), guest count selector, observations field, real-time price calculation
- **User Authentication:** Google OAuth via NextAuth.js, automatic guest creation on first sign-in, session management with guest ID, protected routes for account area
- **Guest Account:** Welcome message with user's first name, access to profile and reservations
- **Profile Management:** Update guest profile with nationality (country selector with flag), national ID (validated: 6-12 alphanumeric characters), server-side form validation
- **My Reservations:** List all user's reservations with cabin name and image, dates, number of nights, number of guests, total price, booking status; edit reservations (modify guests, observations); delete reservations with authorization check
- **Booking Confirmation:** Thank you page after successful booking
- **About Page:** Property description, family history (since 1962), images of property and family, dynamic cabin count display

#### Technology Stack

| Category | Technology |
|----------|------------|
| Framework | Next.js 14 (App Router) |
| Language | JavaScript |
| Authentication | NextAuth.js (Google Provider) |
| Database | Supabase (PostgreSQL) |
| Styling | Tailwind CSS |
| Date Handling | date-fns, react-day-picker |
| Icons | Heroicons React |
| Fonts | Geist (Variable) |

#### Project Structure

```
the-wild-oasis-website/
├── app/
│   ├── _components/          # Reusable UI components
│   ├── _lib/                 # Core utilities (actions, auth, data-service, supabase)
│   ├── account/             # Protected account routes
│   │   ├── profile/
│   │   └── reservations/
│   ├── cabins/               # Cabins listing & details
│   ├── login/                # Login page
│   ├── about/                # About page
│   ├── layout.js
│   └── page.js               # Homepage
├── public/                   # Static assets
├── tailwind.config.js
└── package.json
```

#### Database Schema (Supabase)

- **cabins:** id, name, maxCapacity, regularPrice, discount, description, image
- **guests:** id, email, fullName, nationality, countryFlag, nationalID
- **bookings:** id, created_at, startDate, endDate, numNights, numGuests, cabinPrice, extrasPrice, totalPrice, status, hasBreakfast, isPaid, guestId, cabinId
- **settings:** id, minBookingLength, maxBookingLength, breakfastPrice

#### Environment Variables

```env
# NextAuth
AUTH_SECRET=your-nextauth-secret
AUTH_GOOGLE_ID=your-google-client-id
AUTH_GOOGLE_SECRET=your-google-client-secret

# Supabase
NEXT_PUBLIC_SUPABASE_URL=your-supabase-url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your-supabase-anon-key
```

#### Getting Started

```bash
# Install dependencies
npm install

# Set up environment variables
Create .env.local with Supabase and Google OAuth credentials

# Run development server
npm run dev
```

#### Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm run start` | Start production server |
| `npm run prod` | Build and start production |
| `npm run lint` | Run ESLint |

---

### 2. YouTube Clone 2

🔗 **Live Demo:** [youtubeclone-2.vercel.app](https://youtubeclone-2.vercel.app)

A YouTube clone built with React, Redux Toolkit, Tailwind CSS, and React Router.

#### Features

- Video browsing and playback
- Category-based navigation
- Infinite scroll
- Search functionality
- Responsive design

#### Technology Stack

| Category | Technology |
|----------|------------|
| Frontend | React 18, TypeScript |
| State Management | Redux Toolkit, React Redux |
| Routing | React Router DOM v7 |
| Styling | Tailwind CSS |
| HTTP Client | Axios |

#### Available Scripts

| Command | Description |
|---------|-------------|
| `npm start` | Run app in development mode |
| `npm test` | Launch test runner |
| `npm run build` | Build for production |

---

## Let's Connect

I'm open to collaboration and new opportunities. Feel free to reach out!

- Email: stephen.m.rivero@gmail.com
- Location: Taguig City, Metro Manila

---

*Last updated: April 2026*
