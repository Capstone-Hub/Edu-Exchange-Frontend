# Edu Exchange – Frontend

Edu Exchange is a peer-to-peer learning platform where students can connect with mentors or peers to learn new skills, book sessions, and collaborate. The platform is built using modern web technologies, ensuring speed, scalability, and a seamless user experience.

---

## Tech Stack
- **Framework:** [React](https://react.dev/)  
- **Bundler:** [Vite](https://vitejs.dev/)  
- **Language:** TypeScript  
- **Component Library:** [Chakra UI](https://chakra-ui.com/)  
- **Routing:** [React Router](https://reactrouter.com/)  
- **Icons:** [React Icons (Fi)](https://react-icons.github.io/react-icons/)  
- **Linting & Formatting:** ESLint + Prettier  
- **Themes:** Dark & Light mode support  

---

## Frontend Pages & Workflow
The frontend covers the following user journey:

1. **Landing Page** – Introduction, sign-up/login CTAs, success stories.  
2. **Registration Page** – User details (name, email, password, mentee/mentor selection).  
3. **Educational KYC Page** – Academic background and skills.  
4. **Dashboard (First Login)** – Welcome message, quick links, notifications.  
5. **Find Mentors Page** – Browse/filter mentors with mentor cards.  
6. **Mentor Profile Page** – Mentor details, reviews, booking option.  
7. **Find a Peer Page** – Search peers by skills, availability, and interests.  
8. **Book Session Page** – Choose skill, date/time, and confirm booking.  
9. **Booking Confirmation Page** – Success message with session details.  
10. **My Sessions Page** – Upcoming and past sessions with feedback options.

---

## Project Setup
Follow these steps to set up and run the frontend locally:

### 1. Clone the Repository
```bash
git clone https://github.com/<your-org>/edu-exchange-frontend.git
cd edu-exchange-frontend

```

### 2. Install Dependencies


**Ensure you have Node.js (>=16) and npm or yarn installed.**

```

npm install
 OR
yarn install

```

### 3. Configure TypeScript and ESLint
M**ake sure tsconfig.json and .eslintrc are properly set up.
(Preconfigured in this project; adjust rules if necessary.)**

### 4. Install Chakra UI with Vite
Run the following commands:
```
npm install @chakra-ui/react @emotion/react @emotion/styled framer-motion
```

Wrap your app with Chakra’s ChakraProvider in main.tsx:

```
import { ChakraProvider } from '@chakra-ui/react';
import React from 'react';
import ReactDOM from 'react-dom/client';
import App from './App';

ReactDOM.createRoot(document.getElementById('root')!).render(
  <React.StrictMode>
    <ChakraProvider>
      <App />
    </ChakraProvider>
  </React.StrictMode>,
);
```
**Refer to Chakra’s Vite guide for additional setup.**

### 5. Run the Development Server
```
npm run dev

```
Your app will run at http://localhost:5173 by default.


## Folder Structure

```
edu-exchange-frontend/
│
├── public/              # Static assets
├── src/
│   ├── components/      # Reusable UI components
│   ├── pages/           # Page components (Landing, Dashboard, etc.)
│   ├── routes/          # React Router configuration
│   ├── theme/           # Chakra theme customizations (dark/light mode)
│   ├── assets/          # Images, icons
│   ├── App.tsx
│   └── main.tsx
├── package.json
├── tsconfig.json
└── vite.config.ts

```

## UI & Design

- Theme: Light & Dark modes with Chakra UI.

- Icons: react-icons/fi for consistent iconography.

- Images: Stock images from Freepik.

## Team Assignments
- **Ben:** Landing Page, Dashboard, Book Session Page.

- **Chidiebere:** Registration Page, Educational KYC Page, Find a Peer Page, My Sessions Page.

- **Jindu:** Mentor Profile Page, Educational KYC Page.

- **Daniel:** Find Mentors Page.

- **Ijeoma:** Booking Confirmation Page.

## Next Steps

- Integrate the frontend with MERN backend (Express + Node.js).

- Connect to MongoDB database for users, mentors, and bookings.

- Implement authentication and session booking API endpoints.
