# AGENTS.md

## Project Overview
Create a classic Space Invaders arcade game as a single HTML file. A retro arcade game where the player controls a spaceship defending Earth from alien invaders that move in formation and gradually descend towards the planet.

## Setup Commands
- No installation required
- Open the HTML file directly in any modern web browser
- No build process needed

## Code Style
- Single HTML file with embedded CSS and JavaScript
- Use HTML5 Canvas for game rendering
- Clean, readable JavaScript with meaningful variable names
- CSS classes for UI elements, inline styles for canvas elements
- Comments for complex game logic

## Technical Requirements
- HTML5 Canvas for smooth 60fps animations
- Vanilla JavaScript (no external libraries)
- CSS for styling UI elements
- Web Audio API for sound effects
- Responsive design that works on desktop browsers

## Game Specifications

### Core Gameplay
- Player spaceship moves horizontally at bottom of screen
- Grid of alien enemies (5 rows x 10 columns) at top
- Aliens move left-right in formation, dropping down at screen edges
- Player shoots lasers upward, aliens shoot downward occasionally
- Game ends when aliens reach bottom or player loses all lives
- Aliens speed up as fewer remain alive

### Controls
- A/D keys or Left/Right arrows - move spaceship
- Spacebar - shoot laser
- Enter - restart game after game over

### Visual Design
- Dark space background with animated stars
- Retro pixel-art aesthetic or clean geometric shapes
- Neon color scheme: green player ship, red aliens, yellow lasers
- Explosion particle effects when enemies destroyed
- Score display and lives counter

### Game Features
- Score system (points per alien destroyed)
- Player lives system (3 lives)
- High score tracking using localStorage
- Game over screen with restart functionality
- Sound effects for shooting, explosions, and background music

## File Structure
```
space-invaders.html 
├── <head> - Meta tags, title, embedded CSS 
├── <body> 
│ ├── <canvas> - Game rendering area 
│ ├── <div> - UI overlay (score, lives, game over) 
│ └── <script> - Game logic, controls, audio
```

## Development Instructions
- Use requestAnimationFrame for smooth animations
- Implement collision detection between bullets and sprites
- Create sprite classes for Player, Alien, Bullet
- Use arrays to manage multiple aliens and bullets
- Implement game states: playing, paused, game over
- Add particle systems for explosion effects

## Testing Guidelines
- Test on Chrome, Firefox, Safari
- Verify responsive behavior on different screen sizes
- Check that all controls work as expected
- Ensure smooth 60fps performance
- Test audio playback across browsers

## Security Considerations
- No external resources loaded
- localStorage usage only for high scores
- No user input validation needed (keyboard only)
