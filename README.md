# Real-Time Tracker 🌍

A real-time location tracking application built using **JavaScript**, **Socket.IO**, and **Leaflet.js**. This project showcases the use of Socket.IO to facilitate real-time communication between clients and servers for tracking live locations.

## Features 🚀

- **Real-Time Location Updates**: Continuously tracks and updates user locations in real-time.
- **Interactive Map**: Powered by [Leaflet.js](https://leafletjs.com/), displaying dynamic markers for users on an OpenStreetMap base map.
- **Geolocation Support**: Utilizes the browser's Geolocation API for precise latitude and longitude coordinates.
- **Dynamic Marker Management**:
  - Adds new markers for connected users.
  - Updates existing markers for users as their location changes.
  - Removes markers when users disconnect.

## How It Works 🛠️

1. **Geolocation Tracking**:

   - Checks if the browser supports geolocation.
   - Configures high-accuracy settings with a 5-second timeout and no caching.
   - Uses `watchPosition` to continuously monitor user location.

2. **Socket.IO Communication**:

   - Emits the user's latitude and longitude to the server via a `send-location` event.
   - Receives real-time location updates from the server.

3. **Map Integration**:

   - Initializes a map centered at `(0, 0)` with a zoom level of 15 using Leaflet.js.
   - Adds OpenStreetMap tiles to the map for visualization.

4. **Marker Management**:
   - Dynamically updates marker positions for existing users.
   - Creates new markers for new users.
   - Removes markers when a user disconnects.

## Setup Instructions ⚙️

### Prerequisites

- Node.js and npm installed.
- A modern web browser that supports the Geolocation API.

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/realtime-tracker.git
   ```

## Technologies Used 🧑‍💻

- **Frontend**: JavaScript, Leaflet.js, OpenStreetMap
- **Backend**: Node.js, Socket.IO

## Challenges Faced & Lessons Learned 🌟

- Implementing real-time communication and handling dynamic user connections were challenging but rewarding.
- Learned the intricacies of the Geolocation API and WebSocket communication.


You can save this in a file named `README.md` and include it in your GitHub repository. Let me know if you need further customization!
