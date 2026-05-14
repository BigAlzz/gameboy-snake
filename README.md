# 🎮 Game Boy Snake

A retro-styled Snake game inspired by the classic Nintendo Game Boy with authentic 8-bit aesthetics!

![Game Boy Snake Preview](https://raw.githubusercontent.com/BigAlzz/gameboy-snake/main/assets/screenshot.png)

## Features

- **Authentic Game Boy Design** - Pixel-perfect recreation of the iconic Game Boy hardware
- **LCD Screen Effects** - Realistic dot-matrix display with scanlines and pixelation
- **Classic Snake Gameplay** - Navigate a growing snake to eat food and grow longer
- **Retro Sound Effects** - 8-bit audio synthesized in real-time
- **On-Screen Controls** - Physical Game Boy-style buttons for immersive gameplay
- **Score Tracking** - Classic score display showing your progress

## Screenshots

### Main Screen
![Main View](https://raw.githubusercontent.com/BigAlzz/gameboy-snake/main/assets/main-view.png)

### In-Game Action
![In-Game](https://raw.githubusercontent.com/BigAlzz/gameboy-snake/main/assets/in-game.png)

## Controls

| Button | Action |
|-------|--------|
| ⬆️ ↑ (Up) | Move snake up |
| ⬇️ ↓ (Down) | Move snake down |
| ⬅️ ← (Left) | Move snake left |
| ➡️ → (Right) | Move snake right |
| 🔘 A / Select | Start/Restart game |
| ▶️ B / Start | Pause/Resume game |

## Keyboard Controls

You can also play using your keyboard:
- **Arrow Keys** - Control snake movement
- **Spacebar** - Start or restart game

## How to Play

1. Open `index.html` in a web browser
2. Press **SPACE** or click **START** to begin
3. Use arrow keys to guide the snake around the grid
4. Eat food (shown as brighter pixels) to grow and increase your score
5. Avoid hitting walls or your own tail!

## Game Mechanics

- **Grid Size**: 16×16 tiles
- **Snake Speed**: Adjustable (currently set for balanced gameplay)
- **Score**: +10 points per food eaten
- **Game Over**: Hitting walls or your own tail ends the game

## Customization

You can modify these constants in `index.html`:

```javascript
// Grid size (default: 16×16)
const GRID_SIZE = 16;

// Snake movement speed in milliseconds
let moveInterval = 150; 

// Color palette adjustments
// Change .pixel.on background color for different LCD tones
```

## Browser Compatibility

✅ Fully compatible with:
- Chrome / Chromium
- Firefox
- Safari (desktop)
- Edge
- Opera

⚠️ Mobile browsers require a modern browser that supports the Web Audio API.

## Project Structure

```
gameboy-snake/
├── index.html      # Main game file
├── README.md       # This documentation
└── assets/        # (Optional) Additional assets
    ├── sounds/    # Pre-recorded audio files
    └── sprites/   # Custom sprite graphics
```

## Future Enhancements

- [ ] Mobile touch controls
- [ ] Multiple difficulty levels
- [ ] Power-ups and special items
- [ ] Boss battles
- [ ] Level progression system
- [ ] Save/load functionality
- [ ] Multiplayer mode (local hotseat)

## License

MIT License - Feel free to use, modify, and distribute!

---

**Enjoy the retro vibes!** 🎮✨
