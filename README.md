# Nanolet Social App

A simple social media web application built using the [Nanolet](https://github.com/7AkhilV/nanolet) framework. This app supports basic user authentication, posting, and session management. It's a lightweight application designed to demonstrate the usage of the Nanolet HTTP framework for building RESTful APIs and serving static files.

## Features

- **Authentication**: Log in, log out, and manage user sessions with tokens stored in cookies.
- **User Management**: Update user details like username, name, and password.
- **Posts**: Create and fetch posts with user details associated.
- **Static Files**: Serve HTML, CSS, and JavaScript files for the frontend.

## Tech Stack

- **Backend**: Nanolet (Custom lightweight HTTP framework)
- **Frontend**: Basic HTML, CSS, and JavaScript (can be extended for a real frontend)
- **Session Management**: In-memory sessions stored in an array
- **Routing**: RESTful API routes for user authentication and post management

## Getting Started

To run this project locally, follow these steps:

### Prerequisites

- Node.js (v20 or higher)

### Clone the Repository

```bash
git clone https://github.com/7AkhilV/nanolet-social-app.git
cd nanolet-social-app
```

### Install Dependencies

```bash
npm install
```

### Run the App

```bash
node index.js
```

By default, the app will run on port `8000`. You can access it in your browser at `http://localhost:8000`.

## API Endpoints

### Authentication

- **POST** `/api/login`: Log in a user and receive a session token.
- **DELETE** `/api/logout`: Log out the current user by invalidating the session.

### User Management

- **GET** `/api/user`: Get user information (requires authentication).
- **PUT** `/api/user`: Update user details (requires authentication).

### Posts

- **GET** `/api/posts`: Get all posts.
- **POST** `/api/posts`: Create a new post (requires authentication).

## Preview

![image](https://github.com/user-attachments/assets/65202419-a9ec-4a74-bbc6-941c7054ee5e)

![image](https://github.com/user-attachments/assets/8bfae0a2-0775-433c-9473-58b3dacdbc6f)

![image](https://github.com/user-attachments/assets/9ee06b5d-a707-4692-aeae-2d632f20dbd8)

## Contributing

Feel free to fork the repository and submit pull requests. If you find any bugs or have suggestions for improvement, open an issue.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Note**: The app is currently a basic prototype. Feel free to enhance it with additional features such as a frontend UI, persistent database, and more.
