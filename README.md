# AR Office Experience

An interactive Augmented Reality (AR) web application that brings office objects to life through marker-based AR technology. This project allows users to view and interact with 3D models of office items like laptops, coffee makers, books, and office chairs.

## Features

- **Interactive 3D Models**: View and interact with detailed 3D models of office objects
- **Marker-Based AR**: Uses AR markers to place and track 3D objects in real space
- **Sound Effects**: Interactive sound effects for each object
- **Responsive Design**: Works on both desktop and mobile devices
- **User-Friendly Interface**:
  - Permission handling for camera and motion sensors
  - Loading screen with progress indicator
  - Toast notifications for user feedback
  - Marker detection indicator
  - Sound controls
  - Student details panel

## Prerequisites

- Modern web browser with WebGL support
- Camera access
- AR markers (provided in the `markers` directory)
- HTTPS connection (required for camera access in most browsers)

## Project Structure

```
ar-application/
├── index.html          # Main application file
├── markers/           # AR marker pattern files
│   ├── laptop-marker.patt
│   ├── coffee-marker.patt
│   ├── books-marker.patt
│   └── chair-marker.patt
├── models/            # 3D model files
│   ├── laptop.glb
│   ├── coffee_maker.glb
│   ├── books.glb
│   └── office_chair.glb
└── sounds/           # Sound effect files
    ├── office_ambience.mp3
    ├── keyboard_typing.mp3
    ├── coffee_brewing.mp3
    ├── flipping_through_pages.mp3
    └── chair_adjustment.mp3
```

## Setup and Installation

1. Clone the repository:

   ```bash
   git clone [repository-url]
   cd ar-application
   ```

2. Set up a local server (required for AR.js to work):

   - Using Python:
     ```bash
     # Python 3
     python -m http.server 8000
     # Python 2
     python -m SimpleHTTPServer 8000
     ```
   - Using Node.js:
     ```bash
     npx serve
     ```

3. Open the application:
   - Navigate to `http://localhost:8000` in your web browser
   - Allow camera access when prompted

## Usage

1. **Starting the Application**:

   - Open the application in a web browser
   - Grant necessary permissions (camera and motion sensors)
   - Wait for the loading screen to complete

2. **Using AR Markers**:

   - Print the marker patterns from the `markers` directory
   - Point your camera at the markers to see the 3D objects
   - The marker indicator will show when a marker is detected

3. **Interacting with Objects**:
   - Click on 3D objects to trigger animations and sounds
   - Use the sound button to toggle audio effects
   - View student details using the "Show Details" button

## Technologies Used

- [A-Frame](https://aframe.io/) - Web framework for building VR experiences
- [AR.js](https://ar-js-org.github.io/AR.js-Docs/) - JavaScript library for adding augmented reality experiences to web apps
- [A-Frame Animation Component](https://github.com/ngokevin/aframe-animation-component) - Animation system for A-Frame
- [A-Frame Particle System](https://github.com/IdeaSpaceVR/aframe-particle-system-component) - Particle effects for A-Frame

## Student Contributors

- **Laptop**: Thuduwage I.M.H.G
- **Coffee Maker**: Arandara.S.D
- **Books**: Karunarathne R.Y.D.
- **Office Chair**: Kodithuwakku C.K.

## Browser Support

- Chrome (recommended)
- Firefox
- Safari
- Edge

## Troubleshooting

1. **Camera Not Working**:

   - Ensure you're using HTTPS or localhost
   - Check browser permissions
   - Try a different browser

2. **Markers Not Detected**:

   - Ensure good lighting
   - Keep the marker steady
   - Check if the marker is printed clearly
   - Try adjusting the distance between camera and marker

3. **3D Models Not Loading**:
   - Check internet connection
   - Clear browser cache
   - Try refreshing the page

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- A-Frame team for the amazing VR/AR framework
- AR.js team for the marker-based AR implementation
- All student contributors for their work on the project
