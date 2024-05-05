# Collaborative Text Editor

This project is a collaborative text editor that allows multiple users to edit text in real time using Quill.js, Socket.IO, and Express. The server uses HTTPS to provide secure connections, and WebSocket (via Socket.IO) for real-time communication.

## Prerequisites

Before you begin, make sure you have the following software installed:

- [Node.js](https://nodejs.org/) (version 14.x or later)
- [npm](https://www.npmjs.com/) (usually bundled with Node.js)
- An HTTPS certificate and key in PEM format (for secure connections)

## Installation

1. Clone the repository:

    ```bash
    git clone <repository-url>
    cd <repository-folder>
    ```

2. Install dependencies:

    ```bash
    npm install
    ```

3. Set up your HTTPS certificate and key:

    - Place your certificate (`cert.pem`) and key (`key.pem`) files in a `cert` directory within the project folder.

## Running the Application

1. Start the server:

    ```bash
    node server.js
    ```

2. The server will listen on port `3000` by default. You can modify the port number in `server.js` if desired.

3. Once the server is running, open your web browser and navigate to `https://localhost:3000/`.

4. In the web interface, enter a room name and click the `enter` button. You will be directed to the text editor.

5. You can start typing in the text editor. When other users join the same room, your changes will be synced in real time.

## Notes

- For security reasons, make sure your certificate and key are stored securely.
- If you receive a security warning about the certificate, it may be due to using a self-signed certificate. You can proceed with the warning, or obtain a trusted certificate.

## License

This project is licensed under the MIT License. You can find the full text of the license [here](LICENSE).

## Contributing

Contributions are welcome! Feel free to submit pull requests or open issues on the [repository](<repository-url>).
