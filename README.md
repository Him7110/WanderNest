An awesome tour booking site built on top of NodeJS.
Demo • Key Features • Demonstration • How To Use • API Usage • Deployment • Build With • To-do • Installation • Known Bugs • Future Updates • Acknowledgement

Key Features 📝
Authentication and Authorization
Sign up, Log in, Logout, Update, and reset password.
User profile
Update username, photo, email, password, and other information
A user can be either a regular user or an admin or a lead guide or a guide.
When a user signs up, that user by default regular user.
Tour
Manage booking, check tour map, check users' reviews and rating
Tours can be created by an admin user or a lead-guide.
Tours can be seen by every user.
Tours can be updated by an admin user or a lead guide.
Tours can be deleted by an admin user or a lead-guide.
Bookings
Only regular users can book tours (make a payment).
Regular users can not book the same tour twice.
Regular users can see all the tours they have booked.
An admin user or a lead guide can see every booking on the app.
An admin user or a lead guide can delete any booking.
An admin user or a lead guide can create a booking (manually, without payment).
An admin user or a lead guide can not create a booking for the same user twice.
An admin user or a lead guide can edit any booking.
Reviews
Only regular users can write reviews for tours that they have booked.
All users can see the reviews of each tour.
Regular users can edit and delete their own reviews.
Regular users can not review the same tour twice.
An admin can delete any review.
Favorite Tours
A regular user can add any of their booked tours to their list of favorite tours.
A regular user can remove a tour from their list of favorite tours.
A regular user can not add a tour to their list of favorite tours when it is already a favorite.


How To Use 🤔
Book a tour
Login to the site
Search for tours that you want to book
Book a tour
Proceed to the payment checkout page
Enter the card details (Test Mood):
- Card No. : 4242 4242 4242 4242
- Expiry date: 02 / 22
- CVV: 222
Finished!
Manage your booking
Check the tour you have booked on the "Manage Booking" page in your user settings. You'll be automatically redirected to this page after you have completed the booking.
Update your profile
You can update your own username, profile photo, email, and password.
API Usage
Before using the API, you need to set the variables in Postman depending on your environment (development or production). Simply add:

- {{URL}} with your hostname as value (Eg. http://127.0.0.1:3000 or http://www.example.com)
- {{password}} with your user password as value.


Build With 🏗️
NodeJS - JS runtime environment
Express - The web framework used
Mongoose - Object Data Modelling (ODM) library
MongoDB Atlas - Cloud database service
Pug - High performance template engine
JSON Web Token - Security token
ParcelJS - Blazing fast, zero configuration web application bundler
Stripe - Online payment API and Making payments on the app.
Postman - API testing
Mailtrap & Sendgrid - Email delivery platform
Heroku - Cloud platform
Mapbox - Displaying the different locations of each tour.

Setting Up Your Local Environment ⚙️
If you wish to play around with the code base in your local environment, do the following

* Clone this repo to your local machine.
* Using the terminal, navigate to the cloned repo.
* Install all the necessary dependencies, as stipulated in the package.json file.
* If you don't already have one, set up accounts with: MONGODB, MAPBOX, STRIPE, SENDGRID, and MAILTRAP. Please ensure to have at least basic knowledge of how these services work.
* In your .env file, set environment variables for the following:
    * DATABASE=your Mongodb database URL
    * DATABASE_PASSWORD=your MongoDB password

    * SECRET=your JSON web token secret
    * JWT_EXPIRES_IN=90d
    * JWT_COOKIE_EXPIRES_IN=90

    * EMAIL_USERNAME=your mailtrap username
    * EMAIL_PASSWORD=your mailtrap password
    * EMAIL_HOST=smtp.mailtrap.io
    * EMAIL_PORT=2525
    * EMAIL_FROM=your real-life email address

    * SENDGRID_USERNAME=apikey
    * SENDGRID_PASSWORD=your sendgrid password

    * STRIPE_SECRET_KEY=your stripe secret key
    * STRIPE_WEBHOOK_SECRET=your stripe webhook secret

* Start the server.
* Your app should be running just fine.
Demo-.env file :
demo-env-file

Installation 🛠️
You can fork the app or you can git-clone the app into your local machine. Once done, please install all the dependencies by running

$ npm i
Set your env variables
$ npm run watch:js
$ npm run build:js
$ npm run dev (for development)
$ npm run start:prod (for production)
$ npm run debug (for debug)
$ npm start
Setting up ESLint and Prettier in VS Code 👇🏻
$ npm i eslint prettier eslint-config-prettier eslint-plugin-prettier eslint-config-airbnb eslint-plugin-node
eslint-plugin-import eslint-plugin-jsx-a11y  eslint-plugin-react --save-dev


Future Updates 🪴
Enable PWA
Improve overall UX/UI and fix bugs
Featured Tours
Recently Viewed Tours
And More! There's always room for improvement!

