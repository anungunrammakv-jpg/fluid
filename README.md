# Fluid - WebGL Animation

Beautiful, interactive WebGL fluid simulation optimized for all devices, especially mobile.

## Features

✨ **Visual Effects**
- Real-time 2D incompressible fluid simulation
- Smooth particle advection
- Pressure projection with Jacobi iteration
- Beautiful gradient visualization with velocity-based coloring
- Glassmorphism UI design

📱 **Mobile Optimized**
- Responsive canvas rendering
- Touch input support (mouse and fingers)
- Adaptive quality based on device capabilities
- Safe area insets for notched devices
- Optimized WebGL settings for mobile GPUs

⚙️ **Interactive Controls**
- Real-time parameter adjustment
- Diffusion, viscosity, and decay controls
- Force and scale customization
- Reset button for fresh simulation

🚀 **Performance**
- WebGL2/WebGL rendering
- Framebuffer-based computation
- Efficient shader-based operations
- Optimized texture management

## Getting Started

### Prerequisites
- Node.js (v14+)
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/anungunrammakv-jpg/fluid.git
cd fluid

# Install dependencies
npm install

# Run development server
npm run dev
```

Open your browser and navigate to `http://localhost:5173`

### Building for Production

```bash
npm run build
```

The optimized build will be in the `dist/` directory.

## Usage

### Desktop
- **Mouse Movement**: Create fluid forces with mouse movement
- **Click & Drag**: Paint fluid density
- **Settings Button**: Adjust simulation parameters

### Mobile
- **Touch Interaction**: Swipe your finger to create fluid
- **Settings Button**: Bottom-right corner for parameters
- **Responsive Design**: Automatically adapts to screen size

## Project Structure

```
src/
├── main.js                 # Application entry point
├── fluid-simulator.js      # Core simulation engine
├── controls-manager.js     # UI controls manager
├── config.js              # Configuration and device detection
├── webgl-utils.js         # WebGL helper functions
├── shaders.js             # GLSL shader programs
└── styles.css             # Styles and mobile optimizations

public/
└── index.html             # HTML template

vite.config.js             # Vite configuration
package.json               # Dependencies and scripts
```

## Configuration

Edit `src/config.js` to customize:

- **Simulation parameters**: diffusion, viscosity, decay
- **Rendering**: scale factors and colors
- **Performance**: quality multipliers for different devices
- **Touch settings**: interaction radius and force

## Browser Support

- Chrome/Edge: ✅ Full support (WebGL2)
- Firefox: ✅ Full support (WebGL2)
- Safari: ✅ Good support (WebGL1 fallback)
- Mobile browsers: ✅ Optimized support

## Performance Tips

- On low-end devices, reduce simulation resolution in `config.js`
- Decrease `iterations` for faster but less accurate simulation
- Adjust `decayAmount` to control density persistence

## License

MIT

## Author

[@anungunrammakv-jpg](https://github.com/anungunrammakv-jpg)
