# Hand Tracking Web App
A real-time system that uses your camera to detect and identify the position of your hand with hand tracking.

## Features

- **Real-time hand tracking** using MediaPipe Hands
- **Visual feedback** with hand landmarks and connections overlay
- **Camera switching** between multiple input devices
- **Responsive design** that works on desktop and mobile
- **Error handling** with clear user feedback

## Setup & Usage

### Quick Start
1. Open `index.html` in a web browser
2. Allow camera permissions when prompted
3. Position your hand in front of the camera
4. Watch as signs are recognized in real-time

### Local Server (Recommended)
For better camera compatibility, run with a local server:

```bash
python server.py
```

This opens the app at `http://localhost:8000`

## Technical Details

### Technologies Used
- **HTML5** - Structure and video element
- **CSS3** - Responsive styling and layout
- **JavaScript** - Camera handling and sign recognition logic
- **MediaPipe Hands** - Hand landmark detection
- **WebRTC** - Camera access via getUserMedia API

### Browser Requirements
- Modern browser with WebRTC support (Chrome, Firefox, Safari, Edge)
- Camera access permissions
- HTTPS connection (or localhost for development)

## File Structure

```
Camera Display Site/
├── index.html          # Main application file
├── server.py          # Local development server
└── README.md          # This file
```

## Troubleshooting

### Camera Access Issues
- **Permission Denied**: Check browser camera permissions
- **Camera in Use**: Close other applications using the camera
- **No Camera Found**: Verify camera is connected and enabled
- **HTTPS Required**: Use local server or deploy to HTTPS site

### Performance Tips
- Use good lighting for better hand detection
- Keep hands within camera frame
- Avoid cluttered backgrounds
- Ensure stable internet connection for MediaPipe libraries
