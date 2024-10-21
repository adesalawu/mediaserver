# mediaserver

---

# Media Server with Jellyfin, Home Assistant, and MotionEye

This project sets up a Media Server that hosts **Jellyfin**, **Home Assistant**, and **MotionEye**. It provides a unified platform for media streaming, smart home control, and video surveillance.

## Features
- **Jellyfin**: Open-source media server for streaming movies, TV shows, and music.
- **Home Assistant**: Open-source platform for home automation, enabling control and monitoring of smart devices.
- **MotionEye**: Video surveillance system that provides live feeds and motion detection from connected cameras.

## Prerequisites

Make sure you have the following software installed before proceeding:
- Docker (or Docker Compose)
- Git

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/your-username/media-server.git
   cd media-server
   ```

2. **Set Up Environment Variables:**

   Create a `.env` file with required configurations for Jellyfin, Home Assistant, and MotionEye, such as port numbers and data directories.

3. **Run the Services:**

   Use Docker Compose to set up the media server with all services:

   ```bash
   docker-compose up -d
   ```

4. **Access the Services:**
   - **Jellyfin**: [http://localhost:8096](http://localhost:8096)
   - **Home Assistant**: [http://localhost:8123](http://localhost:8123)
   - **MotionEye**: [http://localhost:8765](http://localhost:8765)

## Configuration

### Jellyfin
1. Open the Jellyfin URL to access the media server and follow the initial setup instructions.
2. Add your media library (movies, TV shows, music, etc.) to start streaming.

### Home Assistant
1. Access the Home Assistant dashboard and follow the setup instructions.
2. Integrate your smart home devices through the available integrations.

### MotionEye
1. Open MotionEye and configure your connected cameras.
2. Set up motion detection, video recording, or live video feeds as per your preferences.

## Troubleshooting

- If any container fails to start, check the logs using:
  
  ```bash
  docker-compose logs <service-name>
  ```

- Ensure that ports used by each service are not blocked or used by other applications.

## Contributing

Feel free to submit pull requests, open issues, or suggest features to improve this media server.

## License

This project is licensed under the MIT License.
