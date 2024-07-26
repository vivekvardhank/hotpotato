# Hot Potato


This project is a web-based multiplayer game where players pass a virtual hot potato to avoid being the one holding it when the timer runs out. The game utilizes WebSockets for real-time communication between players and the server.

## Features

- **Multiplayer Setup**: The game requires exactly four players to start. Players are assigned avatars, with one player holding the potato at the beginning.
- **Game Logic**: The player holding the potato when the timer hits zero loses. Players can pass the potato by clicking on another player's avatar.
- **Real-Time Interaction**: The game uses WebSockets to facilitate real-time interactions between players and the server, ensuring smooth gameplay.

## Installation and Setup

To run this project locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/vivekvardhank/hotpotato.git
   ```

2. **Navigate to the Project Directory and Install Dependencies**:
   ```bash
   cd hotpotato
   npm install
   ```

3. **Start the Server**:
   ```bash
   node server.js
   ```
   If the server starts successfully, you will see the message `Listening on: http://localhost:8080` in your terminal.

4. **Play the Game**:
   Open your web browser and go to `http://localhost:8080` to access the game. Click on "Start" to begin.

## File Structure

- **public/index.html**: Contains the front-end code for the game, including the user interface and client-side logic.
- **server.js**: Handles the server-side logic and WebSocket connections, managing game state and player interactions.
- **utils/constants.js**: Defines constants used for message types exchanged between the server and clients.

## How to Play

- Join the game and wait for four players to connect.
- When the game starts, one player is randomly assigned the hot potato.
- The player holding the potato must click on another player's avatar to pass it.
- The game ends when the timer reaches zero, and the player holding the potato loses.

## Future Enhancements

Potential enhancements include:
- Adding a leaderboard to track player wins and losses.
- Implementing different game modes or difficulty levels.
- Allowing more players or different game mechanics.

## License

This project is open-source and available under the [MIT License](LICENSE).

