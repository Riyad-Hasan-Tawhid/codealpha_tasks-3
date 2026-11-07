# Kindred Connect

Kindred Connect is a modern campus-focused dating and matchmaking web app designed to help people discover meaningful connections through profile-based matching, private messaging, and curated recommendations.

## Overview

This application includes:

- User authentication and onboarding
- Profile creation and personalization
- Discover page for browsing compatible profiles
- Like, skip, and love-request interactions
- Match tracking and conversation history
- Secure messaging between matched users
- Responsive UI built for desktop and mobile experiences

## Tech Stack

- React + TypeScript
- Vite
- Tailwind CSS
- shadcn/ui component system
- React Router
- Supabase for authentication and backend data
- Framer Motion for UI animation

## Project Structure

```bash
src/
  components/   # Reusable UI and page sections
  contexts/     # Application context providers
  hooks/        # Data-fetching and feature hooks
  integrations/
    supabase/   # Supabase client and types
  pages/        # Route-level pages
  lib/          # Utility helpers
```

## Prerequisites

Before running the app locally, make sure you have:

- Node.js 18+
- npm
- A Supabase project configured with your app credentials

## Local Setup

1. Clone the repository
2. Install dependencies:

```bash
npm install
```

3. Create a local environment file:

```bash
copy .env.example .env
```

If there is no `.env.example`, create a `.env` file in the project root with:

```bash
VITE_SUPABASE_URL=your_supabase_project_url
VITE_SUPABASE_PUBLISHABLE_KEY=your_supabase_anon_key
```

4. Start the development server:

```bash
npm run dev
```

5. Open the local URL provided by Vite in the terminal, usually:

```text
http://localhost:5173
```

## Production Build

```bash
npm run build
```

To preview the production build:

```bash
npm run preview
```

## Features in Detail

### Authentication
Users can sign up, sign in, and manage sessions with Supabase Auth.

### Profile Setup
Profiles collect personal information, preferences, and location to support better matching.

### Discovery
The discover experience surfaces nearby or compatible profiles and allows users to take actions like liking or sending a love request.

### Matches
The app tracks accepted connections and surfaces message-ready matches for continued engagement.

### Messaging
Matched users can send and view direct messages in a chat interface.

### Full feature set

Kindred Connect is designed as a full-stack social and relationship platform with the following core capabilities:

- User registration and login
- Secure profile creation and personalization
- Browse and discover potential matches
- Like, pass, and send love requests
- Match management and conversation tracking
- Direct messaging between connected users
- Profile validation and personalized user preferences
- Responsive, modern interface for mobile and desktop
- Data persistence through Supabase tables and auth services
- Future-ready extensions for notifications, recommendations, and premium experiences

### Social and engagement features

The product experience is built to support deeper social engagement beyond basic matching, including:

- Match recommendations based on shared interests and compatibility
- Profiles with lifestyle, education, and location-based details
- Ongoing communication flow after a successful match
- Premium or enhanced user interaction layers
- Clear user journeys for onboarding, exploring, and connecting

### Product roadmap ideas

Planned enhancements may include:

- Real-time push notifications for likes, matches, and messages
- Advanced filtering and recommendation scoring
- Admin moderation tools for reported profiles
- Premium subscription features and enhanced discovery options
- Activity feeds and social proof elements
- Event or community-based meetups for users

### Task-based feature coverage

This project also aligns with the feature themes seen in the task planning reference:

- User registration and login
- Database support for storing users, profiles, activity, and relationships
- Social platform experience with profiles, posts, and comments
- Like and follow interactions for engagement
- Collaboration tools for projects and task management
- Team workflows with group projects and assigned tasks
- Communication features with comments and updates inside task boards
- Full-stack architecture with authentication and database-backed data flows

## Environment Notes

This project depends on environment variables for Supabase connectivity. If data or auth is not working, verify that the values in your `.env` file match your active Supabase project configuration.

## Scripts

```bash
npm run dev      # start local dev server
npm run build    # create production build
npm run preview  # preview production build locally
npm run lint     # run ESLint checks
```

## License

This project is for internal or personal use unless a separate license is provided by the repository owner.
