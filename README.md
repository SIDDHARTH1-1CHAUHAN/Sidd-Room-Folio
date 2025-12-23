# Sidd's Room Folio

A 3D interactive portfolio website showcasing a modeled room, built with Blender and modern web technologies.

![Page screenshot](public/media/og-image.webp?raw=true "Page screenshot")

## Features

- Interactive 3D room model with day/night texture sets
- Ambient audio with background music and sound effects
- Custom GLSL shaders for smoke and theme effects
- Responsive web design with SCSS styling
- Optimized 3D models using Draco compression
- Piano sound effects and UI interactions

## Tech Stack

- **Build Tool**: Vite
- **3D Graphics**: Three.js with custom GLSL shaders
- **Animation**: GSAP (GreenSock Animation Platform)
- **Audio**: Howler.js
- **Styling**: SCSS with include-media for responsiveness
- **Modeling**: Blender
- **Compression**: Draco for GLTF models

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Sidd-Room-Folio.git
   cd Sidd-Room-Folio
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run the development server:
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to the provided localhost URL.

## Usage

- **Navigation**: Use mouse drag to orbit around the room
- **Interaction**: Click on interactive elements to trigger animations and sounds
- **Themes**: Switch between day and night modes to see different textures
- **Audio**: Background music plays automatically; sound effects on interactions

## Project Structure

- `blender files/`: Source Blender project files, textures, and images
- `public/`: Static assets including 3D models (GLB), textures, audio files, fonts, and favicons
- `src/`: Source code
  - `main.js`: Main application logic
  - `style.scss`: Global styles
  - `shaders/`: GLSL shader files for visual effects
  - `styles/`: Modular SCSS files
  - `utils/`: Utility scripts like OrbitControls

## Known Issues & Notes

- Audio compatibility: .ogg files may not play on iOS devices. Consider adding .mp3 fallbacks for better cross-platform support.
- Raycasting hitboxes: Some interactive elements may experience "vibrating" effects at certain camera angles due to mesh animations. This can be mitigated by using static hitboxes or adjusting raycaster logic.
- Code structure: Everything is in a single `main.js` file for simplicity, but consider modularizing for larger projects.
- SCSS organization: Styles are functional but could be better structured for maintainability.

## Contributing

Feel free to fork this repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## Credits

- Inspired by 3D portfolio projects like Bruno Simon's Room and Rachel Wei's Room
- Blender tutorials and materials from various online resources
- Audio assets from Uppbeat, Pixabay, and YouTube
- Fonts from Fontspace
- Icons and SVGs from SVG Repo

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
