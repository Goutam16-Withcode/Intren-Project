# JoyfulJourney - MERN Stack Application

A beautiful happiness planning website built with the MERN stack (MongoDB, Express.js, React.js, Node.js).

## Features

- ✨ Beautiful, responsive UI with Framer Motion animations
- 🎨 Modern gradient design with happiness-themed colors
- 📝 Contact form with MongoDB storage
- 📧 Newsletter subscription functionality
- 🚀 Full-stack MERN architecture
- 💻 Mobile-first responsive design

## Tech Stack

### Frontend
- React.js 18
- Framer Motion for animations
- Tailwind CSS for styling
- Lucide React for icons
- Axios for API calls
- Vite for build tooling

### Backend
- Node.js
- Express.js
- MongoDB with Mongoose
- CORS enabled
- RESTful API design

## Quick Start

### Prerequisites
- Node.js (v16 or higher)
- MongoDB (local or MongoDB Atlas)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd mern-joyful-journey
```

2. Install server dependencies:
```bash
cd server
npm install
```

3. Install client dependencies:
```bash
cd ../client
npm install
```

4. Set up environment variables:
Create a `.env` file in the server directory:
```
PORT=5000
MONGODB_URI=mongodb://localhost:27017/joyful-journey
```

### Running the Application

1. Start the backend server:
```bash
cd server
npm run dev
```
The server will run on http://localhost:5000

2. Start the frontend development server:
```bash
cd client
npm run dev
```
The client will run on http://localhost:5173

### Building for Production

1. Build the client:
```bash
cd client
npm run build
```

2. The built files will be in the `client/dist` directory.

## API Endpoints

### Contact
- `POST /api/contact` - Submit contact form
- `GET /api/contacts` - Get all contacts (admin)

### Newsletter
- `POST /api/newsletter` - Subscribe to newsletter
- `GET /api/newsletter` - Get all subscribers (admin)

## Database Schema

### Contact
```javascript
{
  firstName: String (required),
  lastName: String (required),
  email: String (required),
  service: String,
  message: String (required),
  createdAt: Date (default: now)
}
```

### Newsletter
```javascript
{
  email: String (required, unique),
  createdAt: Date (default: now)
}
```

## Project Structure

```
mern-joyful-journey/
├── client/                 # React frontend
│   ├── src/
│   │   ├── components/    # React components
│   │   ├── App.jsx       # Main App component
│   │   └── main.jsx      # Entry point
│   ├── public/           # Static assets
│   └── package.json      # Client dependencies
├── server/               # Express backend
│   ├── server.js         # Server entry point
│   ├── package.json      # Server dependencies
│   └── .env             # Environment variables
└── README.md
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Design inspired by modern happiness and wellness websites
- Built with love using the MERN stack
- Special thanks to the open-source community