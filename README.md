# Social-Network-Api

## Table Of Content
- [General Info](#general-info)
- [Demo](#Demo)
- [Technologies](#technologies)
- [Installation](#installation)
- [Tests](#Tests)
- [License](#license)
- [Github](#Github)

## General Info
This is an API for a social network web application where users can share their thoughts, react to friends' thoughts, and create a friend list. It uses Express.js for routing, a MongoDB database, the Mongoose ODM, and Moment.js to format timestamps. The seed data is created using Insomnia.

## Demo
[![Demo Video](./video/Screenshot%202024-07-16%20022530.png)](./video/2024-07-16%2002-20-31.mp4)

## Technologies
- [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [Express.js](https://expressjs.com/)
- [Node.js](https://nodejs.org/en/)
- [MongoDB](https://www.mongodb.com/)
- [Mongoose](https://mongoosejs.com/)
- [Insomnia](https://insomnia.rest/)
- [Moment.js](https://www.npmjs.com/package/moment)

## Installation
- Download or clone repository to use this application on local machine.
- `Node.js` and `MongoDB` is required to run the application
- To install necessary dependencies, navigate to the root directory and run the following command:
  `npm i`

  ## Tests

Insomnia is used to test REST API calls. Please see the walk-through demonstration videos: https://drive.google.com/file/d/1MQ2WUP7RbTJPUuadVkVzzmjbWWJe8IWU/view as well as the sections on Description and Usage to see how data is added and tested using Insomnia.

On Insomnia, the following API routes have been created and used to add, update, or remove users, friends, thoughts, and reactions in the user's database.

📁 **USER**

- Create a new user: `POST /api/users`
- Get all users: `GET /api/users`
- Get a single user by its `id`: `GET /api/users/:userId`

- Update a user by its `id`: `PUT /api/users/:userId`

- Delete a user by its `id`: `DELETE /api/user/:userId`

📁 **FRIEND**

- Add a new friend to a user's friend list: `POST /api/users/:userid/friends/:friendId`
- Delete a friend from a user's friend list: `DELETE /api/users/:userid/friends/:friendId`

📁 **THOUGHT**

- Create a new thought: `POST /api/thoughts/`
- Get all thoughts: `GET /api/thoughts/`
- Get a single thought by its `id`: `GET /api/thoughts/:thoughtId`
- Update a thought by its `id`: `PUT /api/thoughts/:thoughtId`
- Delete a thought by its `id`: `DELETE /api/thoughts/:thoughtId`

📁 **REACTION**

- Create a reaction: `POST /api/thoughts/:thoughtId/reactions`
- Delete a reaction by the `reactionId`: `DEL /api/thoughts/:thoughtId/reactions/:reactionId`

## License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
<br>
This repository is licensed under the MIT license.

## Github
[<img src="./video/25231.png" alt="Github Logo" width="75" height="75">](https://github.com/AliyusUnderwood/Social-Network-Api)