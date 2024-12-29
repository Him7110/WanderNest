# WanderNest - Tour Booking Site

WanderNest is an amazing tour booking platform built with NodeJS. It offers users an easy and seamless experience for booking tours, managing bookings, and interacting with others through reviews, favorites, and more.

## Demo 🎬
You can view a live demo of the site at [demo link here].  
*Make sure to replace this placeholder with the actual demo URL once it's live.*

## Key Features 📝

### Authentication and Authorization
- Users can sign up, log in, log out, and reset passwords.  
- Each user can update their information, including username, profile photo, email, and password.

### User Roles
- Users can have different roles such as regular users, admins, lead guides, and guides. By default, a new user is a regular user.

### Tour Management
- Admins and lead guides can create, update, and delete tours.  
- Regular users can view the tours, read reviews, and check tour maps.

### Booking Management
- Regular users can book tours and make payments.  
- Admins and lead guides can view, edit, or delete bookings.  
- Regular users cannot book the same tour twice.

### Review Management
- Only users who have booked a tour can write reviews.  
- Admins can delete any review, while regular users can edit or delete their own reviews.

### Favorites Management
- Regular users can add their booked tours to the list of favorites.  
- They cannot add the same tour to favorites more than once.

## How To Use 🤔

### Booking a Tour:
1. Log in to the site.
2. Search for the tour you want to book.
3. Click on the tour and proceed to the payment page.
4. Complete the payment using the provided test card details:

   **Test Card Details**:
   - Card No.: 4242 4242 4242 4242
   - Expiry Date: 02 / 22
   - CVV: 222

5. Your booking will be confirmed.

### Managing Your Booking:
- Visit the "Manage Booking" page in your user settings to check your booked tours.
- You will be automatically redirected here after completing a booking.

### Updating Your Profile:
- You can update your username, profile photo, email, and password in the profile settings section.

## API Usage 🚀

Before using the API, you must set up the environment variables in Postman (depending on your environment).

Set the following variables:
- `{{URL}}` - Your server hostname (e.g., `http://127.0.0.1:3000` or `http://www.example.com`)
- `{{password}}` - Your user password

## Build With 🏗️
- **NodeJS** - JavaScript runtime
- **Express** - Web framework
- **Mongoose** - ODM library for MongoDB
- **MongoDB Atlas** - Cloud database
- **Pug** - High-performance template engine
- **JSON Web Token (JWT)** - For secure authentication
- **ParcelJS** - Web app bundler
- **Stripe** - Payment gateway integration
- **Postman** - API testing
- **Mailtrap & Sendgrid** - Email delivery services
- **Heroku** - Deployment platform
- **Mapbox** - For displaying tour locations on a map

## Setting Up Your Local Environment ⚙️

To run WanderNest locally:

1. Clone the repository:
   git clone <repo_url>
2. Navigate to the project directory:
  cd WanderNest
3. Install dependencies:
   npm install
4. Set up accounts with the following services:
    MongoDB Atlas
    Mapbox
    Stripe
    Sendgrid
    Mailtrap
5. DATABASE=your_mongodb_url
   DATABASE=your_mongodb_url
   DATABASE_PASSWORD=your_mongodb_password
   SECRET=your_jwt_secret
   JWT_EXPIRES_IN=90d
   JWT_COOKIE_EXPIRES_IN=90
   EMAIL_USERNAME=your_mailtrap_username
   EMAIL_PASSWORD=your_mailtrap_password
   EMAIL_HOST=smtp.mailtrap.io
   EMAIL_PORT=2525
   EMAIL_FROM=your_email
   SENDGRID_USERNAME=apikey
   SENDGRID_PASSWORD=your_sendgrid_password
   STRIPE_SECRET_KEY=your_stripe_secret_key
   STRIPE_WEBHOOK_SECRET=your_stripe_webhook_secret
6. Start the application:
   npm run dev
7. The app should now be running on your local environment.

## Setting up ESLint and Prettier in VS Code 👇🏻
To ensure consistent code formatting, you can set up ESLint and Prettier:
npm install eslint prettier eslint-config-prettier eslint-plugin-prettier eslint-config-airbnb eslint-plugin-node eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react --save-dev

