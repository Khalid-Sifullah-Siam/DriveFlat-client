<div align="center">

# DriveFleet

### Find the right car for every journey.

A modern car rental platform for discovering vehicles, making bookings, and sharing cars with other travelers.

[![Live Website](https://img.shields.io/badge/Live%20Website-DriveFleet-16a34a?style=for-the-badge)](https://drive-fleet-car-rental.vercel.app/)
[![Client](https://img.shields.io/badge/Client-Next.js-black?style=for-the-badge&logo=next.js)](https://github.com/Khalid-Sifullah-Siam/DriveFlat-client)
[![Server](https://img.shields.io/badge/Server-Express.js-43853d?style=for-the-badge&logo=express)](https://github.com/Khalid-Sifullah-Siam/DriveFlat-server)

</div>

## About the Project

DriveFleet makes car rental simple for both renters and car owners. Users can browse available cars, search and filter the fleet, view detailed vehicle information, choose rental dates, and manage bookings from one place.

Authenticated users can also add their own vehicles, update listings, change availability, and remove cars from the marketplace. The Next.js client works with a separate Express server for car and booking data.

## Contents

- [Main Features](#main-features)
- [Built With](#built-with)
- [User Journey](#user-journey)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Screenshots](#screenshots)
- [Deployment](#deployment)

## Main Features

### For Renters

- Browse available cars by type, location, price, and availability
- Search the fleet by car name
- View detailed car specifications and rental information
- Select pickup and return dates for a booking
- Choose whether a driver is needed and add special notes
- View and cancel personal bookings

### For Car Owners

- Add a personal car to the rental marketplace
- Update car details, pricing, location, and availability
- View all cars added by the logged-in user
- Delete an existing car listing

### Platform Features

- Email/password and Google authentication with Better Auth
- Protected booking, listing, and account routes
- Responsive interface for desktop, tablet, and mobile
- Loading, error, empty, and custom not-found states
- Toast notifications for clear user feedback

## Built With

| Frontend | Backend and Services |
| --- | --- |
| Next.js 16 App Router | Node.js and Express.js |
| React 19 | MongoDB |
| Tailwind CSS 4 | Better Auth |
| HeroUI | Vercel |
| Motion | REST API |
| Lucide React and React Icons | React Toastify |

## User Journey

| User | What they can do |
| --- | --- |
| Guest | Explore the fleet, search cars, and view car details |
| Renter | Book cars, manage bookings, and cancel reservations |
| Car Owner | Add, update, manage, and delete car listings |

## Getting Started

### Prerequisites

- Node.js 20 or newer
- npm
- A MongoDB database
- The [DriveFleet server](https://github.com/Khalid-Sifullah-Siam/DriveFlat-server)

### Installation

```bash
git clone https://github.com/Khalid-Sifullah-Siam/DriveFlat-client.git
cd DriveFlat-client
npm install
```

Create a `.env.local` file in the project root:

```env
MONGO_URI=your_mongodb_connection_string
BETTER_AUTH_SECRET=your_better_auth_secret
BETTER_AUTH_URL=http://localhost:3000
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
NEXT_PUBLIC_SERVER_URL=http://localhost:5000
```

Start the development server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser. Keep the DriveFleet server running for car and booking features.

### Available Commands

| Command | Description |
| --- | --- |
| `npm run dev` | Start the development server |
| `npm run build` | Create a production build |
| `npm start` | Start the production server |
| `npm run lint` | Check the project with ESLint |

## Project Structure

```text
src/
├── app/                  # Next.js App Router pages and auth API route
├── components/           # Shared sections, cards, modals, and UI
├── lib/
│   ├── auth.js           # Better Auth configuration
│   ├── auth-client.js    # Client-side auth helper
│   └── data.js           # Car and booking API functions
└── proxy.js              # Protected route handling

public/
└── images/               # Website and README screenshots
```

## Screenshots

### Home and Explore

<div align="center">
  <img src="public/images/Screenshot%20(569).png" alt="DriveFleet home page" width="90%" />
  <br /><br />
  <img src="public/images/Screenshot%20(568).png" alt="DriveFleet explore cars page" width="90%" />
</div>

### Car Details and Booking

<div align="center">
  <img src="public/images/Screenshot%20(567).png" alt="Car details page" width="90%" />
  <br /><br />
  <img src="public/images/Screenshot%20(566).png" alt="Car booking interface" width="90%" />
</div>

### Authentication and Dashboard

<div align="center">
  <img src="public/images/Screenshot%20(565).png" alt="DriveFleet login page" width="90%" />
  <br /><br />
  <img src="public/images/Screenshot%20(563).png" alt="DriveFleet registration page" width="90%" />
  <br /><br />
  <img src="public/images/Screenshot%20(562).png" alt="My bookings page" width="90%" />
  <br /><br />
  <img src="public/images/Screenshot%20(561).png" alt="My added cars page" width="90%" />
</div>

### Responsive Views

<div align="center">
  <img src="public/images/Screenshot%20(560).png" alt="DriveFleet responsive view" width="90%" />
  <br /><br />
  <img src="public/images/Screenshot%20(559).png" alt="DriveFleet mobile interface" width="90%" />
  <br /><br />
  <img src="public/images/Screenshot%20(558).png" alt="DriveFleet car listing view" width="90%" />
  <br /><br />
  <img src="public/images/Screenshot%20(557).png" alt="DriveFleet booking view" width="90%" />
</div>

## Deployment

The client is deployed on Vercel. To deploy your own copy:

1. Import the client repository into Vercel.
2. Add the production environment variables.
3. Set `NEXT_PUBLIC_SERVER_URL` to the deployed server URL.
4. Deploy the project.

The server must be deployed separately and configured with the required database and authentication values.

## Links

- [Live Application](https://drive-fleet-car-rental.vercel.app/)
- [Client Repository](https://github.com/Khalid-Sifullah-Siam/DriveFlat-client)
- [Server Repository](https://github.com/Khalid-Sifullah-Siam/DriveFlat-server)

<div align="center">

Built for smoother rentals, better journeys, and smarter fleet sharing.

</div>
