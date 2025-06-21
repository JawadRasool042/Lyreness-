# 🎵 Lyreness - Music Streaming Platform

A modern, responsive music streaming application built with React and Node.js, featuring a beautiful Spotify-inspired interface with full CRUD operations for music management.

## ✨ Features

### 🎵 Music Management

- **Upload & Manage Songs**: Add, edit, and delete your personal music collection
- **Audio File Support**: Upload audio files with metadata (title, artist, album, genre, duration)
- **Real-time Updates**: Instant UI updates with proper error handling
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices

### 🔐 User Authentication

- **Secure Registration**: User signup with email validation and password requirements
- **JWT Authentication**: Secure login with token-based authentication
- **Profile Management**: Update user profiles and display names
- **Session Management**: Persistent login state with automatic logout

### 🎨 Modern UI/UX

- **Lyreness Theme**: Custom purple gradient design with modern aesthetics
- **Responsive Layout**: Adaptive sidebar and content areas for all screen sizes
- **Interactive Elements**: Hover effects, smooth transitions, and intuitive navigation
- **Preview Mode**: Guest users can browse content with signup prompts

### 📱 Pages & Navigation

- **Home**: Personalized music feed or preview content for guests
- **Search**: Browse categories and discover new music
- **Library**: Manage playlists and personal collections
- **Browse Podcasts**: Explore podcast categories and episodes
- **Premium**: Subscription plans and features showcase
- **Support**: Help center with contact options
- **Download**: Multi-platform app downloads

## 🛠️ Tech Stack

### Frontend

- **React 19.1.0** - Modern React with hooks and context
- **React Router DOM 7.6.2** - Client-side routing
- **Axios 1.10.0** - HTTP client for API calls
- **CSS3** - Custom styling with responsive design
- **Font Awesome** - Icon library

### Backend

- **Node.js** - Server runtime
- **Express.js 4.18.3** - Web framework
- **MongoDB** - NoSQL database
- **Mongoose 8.2.1** - MongoDB ODM
- **JWT 9.0.2** - Authentication tokens
- **bcryptjs 3.0.2** - Password hashing
- **Multer** - File upload handling
- **CORS** - Cross-origin resource sharing

## 🚀 Installation & Setup

### Prerequisites

- Node.js (v14 or higher)
- MongoDB (running on localhost:27017)
- npm or yarn

### Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file in the backend directory:

```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/lyreness
JWT_SECRET=your_secure_jwt_secret_here
```

Start the backend server:

```bash
npm run dev
```

### Frontend Setup

```bash
cd frontend
npm install
npm start
```

The application will be available at `http://localhost:3000`

## 📁 Project Structure

```
lyreness/
├── backend/
│   ├── models/
│   │   ├── User.js          # User schema and methods
│   │   └── Song.js          # Song schema
│   ├── routes/
│   │   ├── auth.js          # Authentication routes
│   │   └── songs.js         # Song management routes
│   ├── middleware/
│   │   └── auth.js          # JWT authentication middleware
│   ├── uploads/             # Audio file storage
│   ├── server.js            # Express server setup
│   └── package.json
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Sidebar.js   # Navigation sidebar
│   │   │   └── TopBar.js    # Top navigation bar
│   │   ├── pages/
│   │   │   ├── Home.js      # Main dashboard
│   │   │   ├── Songs.js     # Song management
│   │   │   ├── Login.js     # User authentication
│   │   │   ├── Signup.js    # User registration
│   │   │   └── ...          # Other pages
│   │   ├── App.js           # Main app component
│   │   └── style.css        # Global styles
│   ├── public/
│   │   └── logo/            # Custom favicon
│   └── package.json
└── README.md
```

## 🔧 Key Features Implementation

### Authentication System

- JWT-based authentication with secure token storage
- Password hashing with bcryptjs
- Protected routes with middleware
- Automatic token validation and logout

### File Upload System

- Multer middleware for handling audio file uploads
- File validation and storage in uploads directory
- Metadata extraction and database storage

### Responsive Design

- Mobile-first approach with CSS Grid and Flexbox
- Breakpoint-based media queries for different screen sizes
- Adaptive sidebar that hides on mobile devices
- Touch-friendly interface elements

### State Management

- React Context for global authentication state
- Local state management for forms and UI interactions
- Optimistic UI updates with proper error handling

## 🎨 Design System

### Color Palette

- **Primary**: Purple gradient (#7B2CBF to #9D4EDD)
- **Background**: Dark theme (#1f1f1f to #000000)
- **Surface**: Card backgrounds (#1a1a1a)
- **Text**: White (#ffffff) and secondary gray (#b3b3b3)

### Typography

- **Logo**: Dangrek font for brand identity
- **Body**: System fonts for optimal readability
- **Headings**: Bold weights with gradient text effects

### Components

- **Buttons**: Rounded corners with hover effects
- **Cards**: Subtle shadows with hover animations
- **Forms**: Gradient inputs with focus states
- **Navigation**: Sticky positioning with backdrop blur

## 🔒 Security Features

- **Password Requirements**: Minimum 8 characters
- **JWT Tokens**: 24-hour expiration
- **CORS Protection**: Configured for frontend domain
- **Input Validation**: Server-side validation for all inputs
- **File Upload Security**: Restricted file types and size limits

## 📱 Responsive Breakpoints

- **Desktop**: 1100px+ (Full sidebar, large grids)
- **Tablet**: 900px-1100px (Compact sidebar, medium grids)
- **Mobile**: 700px-900px (Hidden sidebar, small grids)
- **Small Mobile**: 500px-700px (2-column grids, compact layout)

## 🚀 Deployment

### Backend Deployment

1. Set up MongoDB Atlas or local MongoDB instance
2. Configure environment variables
3. Deploy to Heroku, Vercel, or similar platform

### Frontend Deployment

1. Build the React app: `npm run build`
2. Deploy to Netlify, Vercel, or similar platform
3. Configure environment variables for API endpoints

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This project is licensed under the ISC License.

## 🙏 Acknowledgments

- Inspired by Spotify's design and functionality
- Built with modern web technologies
- Responsive design principles
- User experience best practices

---

**Lyreness** - Where music meets modern design! 🎵✨
