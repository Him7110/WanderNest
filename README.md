WanderNest - Tour Booking Site
WanderNest is an amazing tour booking site built on top of NodeJS. It allows users to easily book tours, manage bookings, and interact with other users through reviews, favorites, and more. With user roles and multiple functionalities for both admins and regular users, WanderNest aims to provide a seamless tour booking experience.

Demo 🎬
You can view the live demo of the site at [demo link here].
Please replace this with the actual demo link once deployed.

Key Features 📝
Authentication and Authorization
Sign up, log in, log out, update, and reset passwords.

User Profile Management
Update username, profile photo, email, password, and other details.
Users can be categorized as regular users, admins, lead guides, or guides. By default, a new user is a regular user.

Tour Management

Admin and lead guides can create, update, and delete tours.
Regular users can view tours and see user reviews and ratings.
Tour maps are available to view for each tour.
Booking Management

Only regular users can book tours (make payments).
Regular users can view all their bookings and manage them.
Admins and lead guides can see all bookings, delete, edit, or manually create bookings (without payment).
Regular users can book a tour only once, and they cannot add the same tour twice.
Review Management

Only regular users who have booked a tour can write reviews.
All users can view the reviews for each tour.
Regular users can edit and delete their own reviews, but cannot review the same tour twice.
Admins can delete any review.
Favorites Management

Regular users can add, remove, and manage favorite tours from their bookings.
A user cannot add a tour to favorites if it is already on their list.
How To Use 🤔
Book a tour:
Log in to the site.
Search for the tour you want to book.
Proceed to the booking page and select your desired tour.
Complete the payment through the checkout page (Test card details are provided below).
Test Card Details:

Card No.: 4242 4242 4242 4242
Expiry date: 02 / 22
CVV: 222
Complete the booking.
Manage your booking:
Go to the "Manage Booking" page in your user settings to see the tours you've booked.
You will be automatically redirected here after making a booking.
Update your profile:
You can update your username, profile photo, email, and password through the profile settings page.
API Usage 🚀
Before using the API, configure Postman for your environment (either development or production).

Set the following variables in your Postman environment:

{{URL}} - Your hostname (e.g., http://127.0.0.1:3000 or http://www.example.com)
{{password}} - Your user password
Build With 🏗️
NodeJS - JavaScript runtime environment
Express - Web framework
Mongoose - ODM library for MongoDB
MongoDB Atlas - Cloud database service
Pug - High-performance template engine
JSON Web Token - Security token management
ParcelJS - Blazing-fast web application bundler
Stripe - Online payment API
Postman - API testing
Mailtrap & Sendgrid - Email delivery platforms
Heroku - Cloud platform for deployment
Mapbox - Displaying the locations of each tour on a map
Setting Up Your Local Environment ⚙️
To set up WanderNest on your local machine:

Clone the repo.

In your terminal, navigate to the cloned repo.

Install the necessary dependencies with:

bash
Copy code
$ npm i
Set up accounts for the following services:

MongoDB
Mapbox
Stripe
Sendgrid
Mailtrap
Create a .env file and set the environment variables for the following:

DATABASE=your Mongodb database URL
DATABASE_PASSWORD=your MongoDB password
SECRET=your JWT secret
JWT_EXPIRES_IN=90d
JWT_COOKIE_EXPIRES_IN=90
EMAIL_USERNAME=your Mailtrap username
EMAIL_PASSWORD=your Mailtrap password
EMAIL_HOST=smtp.mailtrap.io
EMAIL_PORT=2525
EMAIL_FROM=your email address
SENDGRID_USERNAME=apikey
SENDGRID_PASSWORD=your Sendgrid password
STRIPE_SECRET_KEY=your Stripe secret key
STRIPE_WEBHOOK_SECRET=your Stripe webhook secret
Start the server by running:

bash
Copy code
$ npm run dev (for development)
$ npm run start:prod (for production)
Your app should be up and running!

Demo .env file can be found in demo-env-file.

Installation 🛠️
Fork or clone the repository to your local machine.
Navigate to the project directory.
Install dependencies:
bash
Copy code
$ npm i
Set up your environment variables.
Run the app:
bash
Copy code
$ npm run watch:js
$ npm run build:js
$ npm run dev (for development)
$ npm run start:prod (for production)
$ npm run debug (for debugging)
$ npm start
Setting up ESLint and Prettier in VS Code 👇🏻
To set up ESLint and Prettier for consistent code formatting, run:

bash
Copy code
$ npm i eslint prettier eslint-config-prettier eslint-plugin-prettier eslint-config-airbnb eslint-plugin-node eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react --save-dev
Known Bugs 🐞
Currently, there are no known bugs, but if you encounter any, feel free to open an issue in the repository.
Future Updates 🪴
Enable Progressive Web App (PWA) functionality.
Improve overall UX/UI and fix any bugs.
Add features such as Featured Tours, Recently Viewed Tours, and more.
Acknowledgement 🙏
We would like to acknowledge the following services and tools used in this project:

NodeJS, Express, Mongoose, MongoDB Atlas - for the backend structure and database management.
Stripe - for handling secure payments.
Sendgrid & Mailtrap - for email delivery services.
Mapbox - for displaying maps.
Heroku - for deploying the app to the cloud.
ParcelJS - for bundling the app with zero configuration.
Thank you for using WanderNest! If you have any feedback or feature requests, feel free to reach out.
