# Assets Directory

This directory contains optional assets that can enhance the game:
- **sounds/** - Audio files for game events (eating, collision, etc.)
- **sprites/** - Custom sprite graphics for snake and food
- **fonts/** - Pixel-art fonts for score display

## Current Status

| Asset | Status | Notes |
|------|-------|------|
| Sound Effects | ✅ Built-in | Web Audio API integration |
| Snake Sprites | ✅ Built-in | 8×8 pixel graphics |
| Food Sprites | ✅ Built-in | Classic dot design |
| Custom Fonts | ❌ Not needed | System fonts work fine |

## Adding Your Own Assets

### Sound Effects

You can replace the built-in sound effects with your own WAV/MP3 files:

1. Place audio files in `assets/sounds/`
2. Update `index.html` to reference your paths
3. Modify the sound loading code in the script

Example:
```javascript
// Load custom sound
const mySound = new Audio('sounds/eat.wav');
```

### Custom Sprites

If you want different snake or food sprites:

1. Place sprite images in `assets/sprites/` (PNG format recommended)
2. Use the SpriteLoader class to load them
3. Replace the built-in pixel graphics

Example:
```javascript
// Load custom snake sprite
const snakeSprite = await SpriteLoader.load('sprites/snake.png');
```

## Asset Guidelines

- **Sound Files**: WAV (preferred) or MP3, max 10 seconds each
- **Sprites**: PNG format, maximum 16×16 pixels for grid compatibility
- **Fonts**: System fonts are fine; custom fonts need proper licensing

---

*For detailed implementation examples, see the main [README.md](../README.md)*
