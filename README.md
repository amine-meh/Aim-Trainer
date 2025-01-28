# Aim Trainer

Aim Trainer is a Python-based desktop application designed to help users improve their aiming skills. The game creates moving targets that the user must click on while keeping track of time, hits, misses, and overall performance.

## Features

- **Dynamic Target Growth:** Targets grow and shrink to challenge the user.
- **Performance Tracking:** Displays hits, misses, accuracy, and targets-per-second stats.
- **Customizable Settings:** Easily modify target growth rates, lives, and other gameplay mechanics.
- **End Screen Summary:** Shows detailed statistics at the end of the game.

## How It Works

The application is built using `pygame` and runs as a standalone game. Players click on dynamically generated targets within a set play area. The game ends when the player runs out of lives (misses too many targets).

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/aim-trainer.git
   cd aim-trainer
   ```
2. Install the required dependencies:
   ```bash
   pip install pygame
   ```

3. Run the game:
   ```bash
   python main.py
   ```

## Gameplay

- Targets appear randomly on the screen and grow until a maximum size before shrinking.
- Click on targets before they shrink to score points.
- Avoid missing too many targets, as this will cost lives.
- The game ends when you run out of lives.

## Controls

- **Mouse Click:** Hit targets.
- **Esc or Close Button:** Quit the game.

## Code Overview

### Main Components

- **Target Class:**
  - Manages target properties, growth/shrink mechanics, and collision detection.

- **Main Game Loop:**
  - Handles target generation, user input, and updating the game state.

- **UI Elements:**
  - Displays time, lives, hits, and performance stats on a top bar.

- **End Screen:**
  - Summarizes performance after the game ends.

### Key Variables

- `WIDTH` and `HEIGHT`: Screen dimensions.
- `TARGET_INCREMENT`: Time interval between new targets (in milliseconds).
- `LIVES`: Number of lives before the game ends.

## File Structure

```
├── main.py   # Main Python script
└── README.md        # Documentation
```

## Future Enhancements

- Add difficulty levels.
- Implement a leaderboard system.
- Add sound effects and animations.

## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
