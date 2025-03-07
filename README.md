# HomeRentals

## Overview
HomeRentals is a full-stack web application designed to help families and large groups find and book homes for trips. The platform allows property owners to list vacation homes, while travelers can browse, filter, and book accommodations based on their preferences. The system ensures a seamless booking experience with real-time availability updates and secure user authentication.

## Features
- **User Authentication**: Secure login/signup using JWT authentication.
- **Property Listings**: Hosts can add, edit, and manage home listings with images, descriptions, and pricing.
- **Search & Filter**: Users can search properties based on location, price, amenities, and availability.
- **Booking System**: Travelers can book homes, and real-time availability updates are maintained.
- **Image Uploads**: Cloudinary integration for uploading and managing property images.
- **Responsive UI**: Built with React.js for a smooth and interactive experience.

## Tech Stack
- **Frontend**: React.js, Tailwind CSS
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JWT (JSON Web Token)
- **Image Storage**: Cloudinary
- **State Management**: Redux (if applicable)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Shivang139/HomeRentals.git
   cd HomeRentals
   ```
2. Install dependencies for frontend and backend:
   ```bash
   cd client
   npm install
   cd ../server
   npm install
   ```
3. Set up environment variables (`.env` file in the server folder):
   ```env
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_secret_key
   CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   ```
4. Run the development servers:
   - **Frontend**:
     ```bash
     cd client
     npm start
     ```
   - **Backend**:
     ```bash
     cd server
     npm start
     ```
5. Open `http://localhost:3000` to view the app in the browser.

## API Endpoints
### Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login user

### Properties
- `GET /api/properties` - Get all property listings
- `POST /api/properties` - Add a new property (Host only)
- `PUT /api/properties/:id` - Edit a property (Host only)
- `DELETE /api/properties/:id` - Delete a property (Host only)

### Bookings
- `POST /api/bookings` - Create a new booking
- `GET /api/bookings/:userId` - Get all bookings for a user
- `DELETE /api/bookings/:id` - Cancel a booking

## Future Enhancements
- **Payment Integration**: Secure online payments for bookings.
- **Review System**: Allow users to leave reviews and ratings for properties.
- **Wishlist Feature**: Users can save properties for future bookings.
- **Admin Dashboard**: Manage users, properties, and bookings efficiently.

## Contributing
Contributions are welcome! Feel free to fork the repository and submit pull requests.

## Contact
For any queries or suggestions, feel free to reach out:
- **GitHub**: [Shivang139](https://github.com/Shivang139)
- **Email**: shivangagrawal139@gmail.com

