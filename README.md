# InstaPlaces

### Live Demo

https://wesmern.web.app/

** **Note that currently this web app is deployed with Heroku, which does not have persistent storage. The static resources such as the avatar images and the photos will be deleted every new 24-hour cycle. It is a Heroku feature which I cannot disable. The fix is to use a third party persistent storage, such as AWS S3, which I am planning to integrate in the near future. For now, you will see most user/places records not rendering images, as they were created before of the 24-hour cycle that you are currently in. However, if you sign up for a new user and upload images, you will see them rendering correclty (until the next 24-hour cycle).** **


### Introduction

This is a Instagram-like photo-sharing web app, designed for users to share their travelling photos. The difference is users ought to share photos of specific places. They will be specifically asked to enter a address/coordinates when they want to post a photo, and afterwards others will be able to view this place with the integrated Google Map.

### Technology Used

This web app is developed with the MERN stack - MongoDB, Express.js, React.js, Node.js. I have previously developed full-stack web apps based on Spring Boot and Vue, and wanted to try different tech stacks so that I have a better understanding of full stack development process.

### How to use

- Clone the repository to local, which has npm installed
- At line 52 of the file `backend/app.js`, add your mongodb url
- In the file `frontend/.env`, add your backend service url. In my case, is the url of my server deployed on Heroku. It could be `localhost` if you run locally.
- run `npm install` in both `frontend` and `backend` directory.
- run `npm start` in both `frontend` and `backend` directory.
