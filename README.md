# Online Chess Game

## Overview
This is a real-time, multiplayer online chess game that allows players to engage in live matches by creating or joining game rooms. It offers seamless gameplay with synchronized moves across players.

## Features
- **Create Game Rooms:** Start a new game by generating a unique Room ID.
- **Join Game Rooms:** Enter a Room ID to join an existing game.
- **Live Multiplayer Chess:** Play live matches with real-time move synchronization.
- **Responsive Interface:** Intuitive chessboard layout for smooth user experience.

## Technologies Used

### Frontend
- **React:** User interface development.
- **React-Chessboard:** For rendering the interactive chessboard.
- **Socket.IO:** Real-time communication between players.

### Backend
- **Node.js:** Server environment.
- **Express.js:** Web application framework.
- **Socket.IO:** WebSocket connections for real-time updates.
- **Chess.js:** Chess game logic and validation.

## Installation

### Clone the Repository
If you haven't done so already, clone the repository:
```bash
git clone https://github.com/Ms-Ngari/Online-Chess-Game.git
```

### Navigate to the Project Directory
```bash
cd Online-Chess-Game
```

### Install Dependencies
For both frontend and backend:

#### Frontend
```bash
cd frontend
npm install
```

#### Backend
```bash
cd ../backend
npm install
```

## Running the Application
1. **Start the Backend Server:**
   ```bash
   cd backend
   npm start
   ```

2. **Start the Frontend:**
   ```bash
   cd ../frontend
   npm start
   ```

3. **Access the Game:**
   Open your browser and navigate to `http://localhost:3000`.


## License
This project is licensed under the [MIT License](LICENSE).