# Node.js WebSocket Mock Service

A Node.js project demonstrating how to integrate **WebSockets** into a mock service and frontend application to enable real-time, two-way communication between the client and server.

## 📖 Overview

This project builds on a previously created mock service by adding WebSocket support. Instead of relying on repeated HTTP requests (polling), the application establishes a persistent connection between the browser and the server, allowing data to be pushed instantly whenever changes occur.

The application displays **live product order counts**, updating connected clients in real time as new orders are processed.

## 🚀 Features

* REST API for mock product data
* WebSocket server for real-time communication
* Live order count updates
* Persistent client-server connection
* Mock service for testing frontend applications
* Simple and lightweight Node.js implementation

## 🛠️ Technologies Used

* Node.js
* Express.js
* WebSocket (`ws`)
* JavaScript
* HTML & CSS

## 📂 Project Structure

```text
node-mocking/
├── mock-srv/
├── static/
└── README.md
```

## ⚙️ Installation

1. Clone the repository.

```bash
git clone <repository-url>
```

2. Navigate into the project folder.

```bash
cd project-folder
```

3. Install dependencies.

```bash
npm install
```

## ▶️ Running the Project

Start the server:

```bash
npm start
```

or

```bash
node server.js
```

Open your browser and navigate to:

```text
http://localhost:3000
```

## 🔄 How It Works

1. The browser loads the frontend using HTTP.
2. A WebSocket connection is established with the server.
3. The server upgrades the HTTP connection to a WebSocket connection.
4. Whenever a product order changes, the server broadcasts the updated order count to all connected clients.
5. Every connected browser receives the update instantly without refreshing the page.

## 📡 Why WebSockets?

Traditional HTTP requires the client to repeatedly ask the server for updates. WebSockets create a persistent connection that allows both the client and server to send messages at any time, making them ideal for:

* Live dashboards
* Chat applications
* Notifications
* Multiplayer games
* Stock price updates
* Real-time analytics

## 📚 Learning Objectives

This project demonstrates how to:

* Create a WebSocket server using Node.js.
* Connect a browser to a WebSocket server.
* Broadcast messages to multiple clients.
* Update the UI in real time.
* Combine REST APIs with WebSockets in a single application.

## 📄 License

This project was created for educational purposes as part of a Node.js learning course.
