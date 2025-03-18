# YelpCamp

YelpCamp is a web application that allows users to discover, review, and share campgrounds. Built with Node.js, Express, and MongoDB, this platform provides a comprehensive solution for camping enthusiasts to find their next adventure.

## Features

- **User Authentication**: Secure account creation and login system using Passport.js
- **Campground Management**: Create, view, edit, and delete campgrounds
- **Review System**: Leave and manage reviews for campgrounds
- **Interactive Maps**: Location-based features using Mapbox
- **Responsive Design**: Works on desktop and mobile devices
- **Flash Messages**: Intuitive user feedback system
- **Security Features**: Implementation of Helmet.js, MongoDB sanitization, and more

## Tech Stack

- **Backend**: Node.js, Express.js
- **Database**: MongoDB with Mongoose ODM
- **Frontend**: EJS templating, Bootstrap
- **Authentication**: Passport.js
- **Cloud Storage**: Cloudinary (for image uploads)
- **Maps**: Mapbox API

## Installation

### Prerequisites

- Node.js (v12 or higher)
- MongoDB (local installation or Atlas)
- npm or yarn

### Setup

1. Clone the repository:
`
  git clone https://github.com/your-username/yelp-camp.git
cd yelp-camp
`
2. Install dependencies:
 `npm install`

3. Create a `.env` file in the root directory with the following variables:
`DB_URL=your_mongodb_connection_string
SECRET=your_session_secret
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_KEY=your_cloudinary_key
CLOUDINARY_SECRET=your_cloudinary_secret
MAPBOX_TOKEN=your_mapbox_token`

4. Start the application:
`npm start`

For development:
`npm run dev`

5. Access the application at `http://localhost:3000`

## Project Structure
`yelp-camp/
├── models/             # Database models
├── public/             # Static assets (CSS, JS, images)
├── routes/             # Route handlers
│   ├── campgrounds.js  # Campground routes
│   ├── reviews.js      # Review routes
│   └── users.js        # User authentication routes
├── utils/              # Utility functions
├── views/              # EJS templates
├── app.js              # Main application file
└── .env                # Environment variables (not in version control)  `

## Usage

- **Home Page**: Browse featured campgrounds
- **Campgrounds**: View all available campgrounds
- **User Authentication**: Register or login to create campgrounds and leave reviews
- **Campground Details**: View location, description, and reviews for each campground
- **User Dashboard**: Manage your campgrounds and reviews

## Security Features

YelpCamp implements various security measures:

- **Helmet.js**: Sets various HTTP headers for app security
- **Content Security Policy**: Restricts which resources can be loaded
- **MongoDB Sanitization**: Prevents MongoDB operator injection
- **Express Session Management**: Secures user sessions
- **HTTP-Only Cookies**: Prevents client-side access to cookies

## Deployment

This application is configured for deployment on platforms like Heroku with the following considerations:

- MongoDB connection string is configured via environment variables
- Port is set dynamically based on the hosting environment
- Static files are served efficiently

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- [Colt Steele's Web Developer Bootcamp](https://www.udemy.com/course/the-web-developer-bootcamp/) - Original project concept
- [Express.js](https://expressjs.com/) - Web framework
- [MongoDB](https://www.mongodb.com/) - Database
- [Bootstrap](https://getbootstrap.com/) - Frontend framework
- [Mapbox](https://www.mapbox.com/) - Maps API
- [Cloudinary](https://cloudinary.com/) - Image hosting


      
