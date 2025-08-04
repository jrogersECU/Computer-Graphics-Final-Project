# Computer-Graphics-Final-Project
# Virtual Ball Pit Party 🎈

A fun, interactive 3D ball pit simulation with realistic physics, collision detection, and sound effects. Perfect for birthdays, celebrations, or just playing around!

## Features

- 🔴 **Spawn Colorful Balls**: Create red, blue, yellow, and green party balls
- 🖱️ **Mouse Interaction**: Push and repel balls with your mouse cursor
- ⚡ **Realistic Physics**: Watch balls collide with physics simulation
- 🔊 **Sound Effects**: Hear ball pit collision sounds
- ✨ **WebGL Rendering**: Real-time 3D graphics with dynamic shadows and lighting
- 🧹 **Easy Cleanup**: "Erase All" button to clear the pit instantly

## Technologies Used

- **HTML5**: Structure and markup
- **CSS3**: Styling and animations
- **JavaScript (ES6+)**: Core application logic and physics
- **Three.js (r128)**: 3D graphics library for WebGL rendering
- **WebGL**: Hardware-accelerated 3D graphics
- **Web Audio API**: Synthetic sound generation for collision effects

## Physics Implementation

- **Collision Detection**: Sphere-to-sphere and sphere-to-ground collision detection
- **Physics Simulation**: Gravity, friction, velocity damping, and elastic collisions
- **Mouse Interaction**: Ray casting for 3D mouse position calculation and repulsion forces
- **Real-time Rendering**: 60 FPS animation loop with dynamic lighting

## How to Run

### Option 1: Local Development Server (Recommended)

1. **Download the project** from GitHub:
   ```bash
   git clone https://github.com/yourusername/Computer-Graphics_Final_Project.git
   cd Computer-Graphics_Final_Project
   ```

2. **Start a local server** (required for proper Three.js loading):
   
   **Using Python:**
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Python 2
   python -m SimpleHTTPServer 8000
   ```
   
   **Using Node.js:**
   ```bash
   npx serve .
   ```

3. **Open your browser** and navigate to:
   ```
   http://localhost:8000
   ```

### Option 2: Direct File Opening

1. **Download the project** files
2. **Open `index.html`** directly in a modern web browser
3. **Note**: Some browsers may block Three.js CDN loading when opening files directly

## Browser Requirements

- **Modern Web Browser** with WebGL support (Chrome, Firefox, Safari, Edge)
- **Audio Support** for Web Audio API
- **JavaScript Enabled**

## Usage Instructions

1. **Start**: Open `home.html` and click "Jump Into the Ball Pit!"
2. **Enable Sound**: Click anywhere on the ball pit page to enable audio
3. **Spawn Balls**: Use the colored buttons to create balls
4. **Interact**: Move your mouse to push balls around
5. **Clear**: Use the "Erase All" button to remove all balls
6. **Return**: Click "Back to Landing" to return to the home page

## Performance Notes

- Optimized for **smooth 60 FPS** performance
- **Dynamic shadow mapping** with 2048x2048 resolution
- **Sound pooling** prevents audio overlap during rapid collisions
- **Efficient collision detection** using spatial optimization

## Browser Compatibility

| Browser | Status |
|---------|--------|
| Chrome 80+ | ✅ Fully Supported |
| Firefox 75+ | ✅ Fully Supported |
| Safari 13+ | ✅ Fully Supported |
| Edge 80+ | ✅ Fully Supported |

## Technical Details

- **Rendering Engine**: Three.js WebGL renderer with soft shadow mapping
- **Physics**: Custom Verlet integration with elastic collision response
- **Audio**: Procedurally generated collision sounds using Web Audio API
- **Lighting**: Multi-light setup with ambient, directional, and point lights
- **Materials**: Physically-based rendering (PBR) with metallic and emissive properties

**Enjoy your virtual ball pit party!** 🎊🎈🎉
