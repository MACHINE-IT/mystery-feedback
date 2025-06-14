# FeedbackFullstack

A full-stack feedback application built with Next.js, designed to collect, manage, and display user feedback efficiently.

## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [API Endpoints](#api-endpoints)
- [Environment Variables](#environment-variables)
- [Contributing](#contributing)
- [License](#license)

---

## Features

- User authentication and authorization
- Submit, edit, and delete feedback
- Admin dashboard for managing feedback
- Responsive UI with modern design
- API endpoints for feedback operations
- Error handling and validation

## Tech Stack

- **Frontend:** Next.js, React, Tailwind CSS
- **Backend:** Next.js API Routes (Node.js)
- **Database:** MongoDB (Mongoose)
- **Authentication:** NextAuth.js
- **Deployment:** Vercel

## Getting Started

### Prerequisites

- Node.js >= 16.x
- npm or yarn
- MongoDB database

### Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/FeedbackFullstack.git
    cd FeedbackFullstack
    ```

2. **Install dependencies:**
    ```bash
    npm install
    # or
    yarn install
    ```

3. **Configure environment variables:**
    - Copy `.env.example` to `.env.local` and fill in the required values.

4. **Run the development server:**
    ```bash
    npm run dev
    # or
    yarn dev
    ```

5. **Open [http://localhost:3000](http://localhost:3000) in your browser.**

## Project Structure

```
/mstrymessage
├── components/        # Reusable React components
├── pages/             # Next.js pages (API & UI)
│   ├── api/           # API routes
│   └── ...            # UI pages
├── models/            # Mongoose models
├── utils/             # Utility functions
├── styles/            # Global styles
├── public/            # Static assets
├── README.md
└── ...
```

## API Endpoints

### Feedback

- `GET /api/feedback` - Get all feedback
- `POST /api/feedback` - Submit new feedback
- `PUT /api/feedback/:id` - Update feedback (admin)
- `DELETE /api/feedback/:id` - Delete feedback (admin)

### Auth

- `POST /api/auth/signin` - Sign in
- `POST /api/auth/signout` - Sign out

## Environment Variables

Create a `.env.local` file in the root directory and add:

```
MONGODB_URI=your_mongodb_connection_string
NEXTAUTH_URL=http://localhost:3000
NEXTAUTH_SECRET=your_nextauth_secret
```

## Contributing

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

## License

This project is licensed under the [MIT License](LICENSE).

---

**Made with ❤️ using Next.js**
