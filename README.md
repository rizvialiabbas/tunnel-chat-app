# Tunnel Chat App

> A small chat application built using the **MEAN** stack  
> Note: this is a deployed project hence the code cannot be made public

# Features

- Register and authenticate users using JSON web tokens

- Join a common room where you can chat with all the registered users

- Open 1on1 private conversations with a user of your choice

- Special departmenal room where all users of the same department can communicate

- Allows the sharing of media files

- Find contacts easily through the search option

- Notifications for messages on background conversations

- Have a pleasant UI/UX built to look awesome from mobile to desktop

# Technologies

- [NodeJS](https://nodejs.org/) - JavaScript backend/server-side solution of choice

- [Express](https://expressjs.com/) - Node framework that makes handling http requests with ease

  - [JsonWebToken](https://www.npmjs.com/package/jsonwebtoken) - package that helps with generating JWTs for secure authentication

  - [PassportJS](http://passportjs.org/) - authentication middleware used to guard certain parts of the app for non-authenticated requests

- [MongoDB](https://www.mongodb.com/) - data storage solution that just speaks JSON and pairs very well with Node

  - [Mongoose](http://mongoosejs.com/) - package that helps with object modeling and manages connection between server and database

  - [Bcryptjs](https://www.npmjs.com/package/bcryptjs) - for salting and hashing the user password to be stored in the database

- [Socket.io](https://socket.io/) - web sockets implementation, fast and reliable real-time communication engine

- [Angular](https://angular.io/) - rich frontend web framework, helps creating fast, reliable web applications

  - [Angular-CLI](https://cli.angular.io/) - command line interface for streamlined angular development

  - [TypeScript](https://www.typescriptlang.org/) - superset of JavaScript that can be compiler-checked, also has types!!

  - [MomentJS](https://momentjs.com/) - JavaScript date/time parser

  - [Bootstrap](http://getbootstrap.com/) - CSS/JS framework, makes it easy to develop responsive, well polished web apps

# How it works

On the client-side users can create accounts that will be stored in the database. Then users can authenticate with the given credentials, if those are correct the server sends a unique token to the client. The client stores it for use on restricted backend route requests.

Once authenticated, the server creates a socket bidirectional connection with the client to facilitate the chat functionality.

Every time a user sends a message, this goes to the server which redirects it to the desired respondent. Also every time a user enters or leaves chat, the server announces all the connected clients.

Also, a user can share media through this platform.

# Motivation

This is a company internship project that provides a work-oriented chatting environment for all employees. The main intention was to explore and learn a lot about [Socket.io](https://socket.io/) and [Angular](https://angular.io/).

# ScreenShots

- ![Working View](https://ibb.co/VQPVVS3)
- [Home Page](https://ibb.co/cD2hV2c)
- [Chat Room](https://ibb.co/YNvyK4w)
