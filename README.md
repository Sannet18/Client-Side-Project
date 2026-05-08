# 💬 Messaging App

A full-featured messaging application built with Vue.js on the frontend and a custom Node.js REST API backed by MongoDB. Supports user accounts, friends, group chats, invitations, and more.

---

## Features

### Account & Authentication
- Create an account with real-time input validation 
- Sign in and sign out securely
- Delete account

### Friends
- Send, accept, and decline friend requests
- View incoming friend requests
- Remove friends

### Group Chats
- Create group chat sessions
- Invite friends and non-friends to a group
- Accept or decline group chat invitations
- View group name and members
- View, and send messages in a group chat
- Leave a group chat


---

## Tech Stack

| Layer      | Technology       |
|------------|------------------|
| Frontend   | Vue.js           |
| Backend    | Node.js          |
| Database   | MongoDB          |
| API Style  | REST             |


## Views

### Create Account View
- Link to Sign-in view
- Real-time input validation with user-facing feedback (e.g. *"Username must be at least 5 characters"*)
- Create button disabled until all validation requirements are met
- On success: redirects to Sign-in view with a confirmation message
- On failure: displays an appropriate error message

### Sign-in View
- Link to Create Account view
- On success: redirects to Home view
- On failure: displays an appropriate error message

### Home View
The main application view. From here the user can:
- View their friends list
- Invite a user to be a friend
- View and respond to incoming friend requests (accept or reject)
- Create a group chat session
- Invite users (friends and non-friends) to a group chat
- View group chat invitations and accept or decline them
- View the name and members of a group chat
- View messages in a group chat
- Post a message to a group chat
- Leave a group chat

---

## Project Structure

```
├── client/               # Vue.js frontend
│   ├── src/
│   │   ├── views/        # Page-level views (Home, SignIn, CreateAccount)
│   │   ├── components/   # Reusable UI components
│   │   └── api/          # API request helpers
├── server/               # Node.js REST API
│   ├── routes/           # Express route handlers
│   ├── models/           # MongoDB/Mongoose models
│   └── middleware/       # Auth and validation middleware
├── .env.example
├── package.json
└── README.md
```

---


## License

[MIT](LICENSE) © [Sannet]
