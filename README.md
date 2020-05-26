<h1 align="center">
  <img alt="Fastfeet" title="Fastfeet" src="https://github.com/Rocketseat/bootcamp-gostack-desafio-02/raw/master/.github/logo.png" width="300px" />
</h1>

<h3 align="center">
  GoStack Challenge 10: FastFeet - Mobile App
</h3>

### Challenge

Create a mobile app for a fake logistics company called FastFeet.

### Instructions ###

Setup back-end

- Change directory to the backend folder cd backend and run yarn install.

All of the following commands that has [] wrapped around it are related to the .env file. Just duplicate from .env.example and update the values.

PostgreSQL
- docker run --name database -e POSTGRES_PASSWORD=[DB_PASS] -p 5432:5432 -d [DB_USER]

Redis
$ docker run --name redisfastfeet -p 6379:[REDIS_PORT] -d -t redis:alpine

Seed database with admin user
$ yarn sequelize db:seed:all

This command generates the admin user with the following credentials:

Email: fastfeet@admin.com
Password: 123456

Run migrations
$ yarn sequelize db:migrate

Update the .env variables for Mailtrap and Sentry
At this point you shoud have the back-end all set up and good to go.

Start server

$ yarn dev

Start queue (open a new terminal)

$ yarn queue

Setup frontend

Change directory to the frontend folder cd frontend and run yarn install. Open src/services/api.js and update the API_URL variable with the APP_URL you specified in the config backend.

Start server
$ yarn start
$ Setup mobile

Change directory to the mobile folder cd mobile and run yarn install. Open src/services/api.js and update the API_URL variable with the APP_URL you specified in the config backend. The mobile app was tested on the iOS Simulator (iPhone X and iPhone 8), Genymotion (Google Pixel 3) and on an actual Android device (Moto X4).

Build app for Android

$ npx react-native run-android

Build app for iOS

$ npx react-native run-ios

Start Metro server

$ yarn start

### Description ###
Mobile app of a fake logistics company called FastFeet.

Tools and technologies used on this project:

- Javascript ES6
- React Native
- React Native Camera
- React Native Navigation
- Redux
- Redux Saga
- Immer
- Styled Components


