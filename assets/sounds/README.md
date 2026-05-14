# Sound Effects

This directory contains audio files for game events.

## Available Sounds

| Event | Sound File | Description |
|------|-----------|-------------|
| Snake Eat | `eat.wav` | Satisfying "pop" when snake consumes food |
| Snake Move | `move.wav` | Subtle slide sound during movement |
| Game Over | `gameover.wav` | Dramatic ending theme |

## Sound Specifications

All sounds are in **WAV format** with 8-bit mono audio to match the retro Game Boy aesthetic:
- Sample rate: 22050 Hz (1/4th of CD quality)
- Bit depth: 8 bits
- Channels: Mono

## Implementation

Sounds are loaded using the Web Audio API and triggered by game events:

```javascript
// Snake eating food
if (snakeParts[0].x === food.x && snakeParts[0].y === food.y) {
    soundManager.play('eat');
}

// Game over
soundManager.play('gameover');
```

## Adding Custom Sounds

1. Convert your audio to 8-bit WAV format using tools like:
   - [Online-Converter](https://www.online-converter.com/)
   - FFmpeg: `ffmpeg -i input.mp3 -c:a pcm_s8le output.wav`

2. Place files in this directory
3. Update the sound names in `index.html`'s sound manager

---

*For more details, see [../README.md](../README.md)*
