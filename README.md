# Social-Networking-API

## Description
This is an API for a socail networking application where users can create thoughts and react to others.
It uses Express.js, MongoDB, Mongoose, and Moment.js.
Insomnia was used for seed data.

## Video Link
https://drive.google.com/file/d/1U5wj9b_exKG1dJLrFIiYNqZbMWA5tkPP/view?usp=sharing

## Preview
![image](https://github.com/JBowen96/Social-Networking-API/assets/139276635/aae04a59-d34e-4e55-a7e7-c7e82ac19001)
![image](https://github.com/JBowen96/Social-Networking-API/assets/139276635/564100c3-83d8-4d3f-941c-95e31f937373)
![image](https://github.com/JBowen96/Social-Networking-API/assets/139276635/fdfba1e4-7c7f-473a-aca8-bb67a362c557)

## Installation
- Download/ clone the repo.
- Assure that MongoDB and Node.js are installed.
- Use `npm i` to install all necessary dependencies.
- Open MongoDB with `MongoDB Compass` and create a database named `socialDB`.
- Add `thoughts` and `users` as collections in the database.
- Use `npm start` to run server.js.
- Access the API with Insomnia via `localhost:3001`.
- Set seeds in the API with `POST`, `GET`, `DELETE`, and `PUT`.

## Insomnia Calls

In Insomnia, the following API routes have been created.

**USER**

- Create a new user: `POST /api/users`
- Get all users: `GET /api/users`
- Get a single user by its `id`: `GET /api/users/:userId`

- Update a user by its `id`: `PUT /api/users/:userId`

- Delete a user by its `id`: `DELETE /api/user/:userId`

**FRIEND**

- Add a new friend to a user's friend list: `POST /api/users/:userid/friends/:friendId`
- Delete a friend from a user's friend list: `DELETE /api/users/:userid/friends/:friendId`

**THOUGHT**

- Create a new thought: `POST /api/thoughts/`
- Get all thoughts: `GET /api/thoughts/`
- Get a single thought by its `id`: `GET /api/thoughts/:thoughtId`
- Update a thought by its `id`: `PUT /api/thoughts/:thoughtId`
- Delete a thought by its `id`: `DELETE /api/thoughts/:thoughtId`

**REACTION**

- Create a reaction: `POST /api/thoughts/:thoughtId/reactions`
- Delete a reaction by the `reactionId`: `DEL /api/thoughts/:thoughtId/reactions/:reactionId`

## Contact
Josh Bowen
github.com/JBowen96
