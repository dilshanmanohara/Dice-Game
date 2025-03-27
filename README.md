# Dice Game 🎲

A modern Android dice game built with Jetpack Compose where players compete against a computer opponent in a strategic dice-rolling challenge.

## Game Overview 🎮

This dice game is an engaging turn-based game where players compete against an AI opponent. Each player rolls five dice and can strategically choose which dice to keep and which to reroll, aiming to reach the target score first.

## Features ✨

- **Interactive Gameplay**
  - Roll 5 dice simultaneously
  - Up to 2 optional rerolls per turn
  - Strategic dice selection for rerolls
  - Computer opponent with intelligent decision-making

- **Modern UI**
  - Built with Jetpack Compose
  - Material Design 3 theming
  - Animated dice representations
  - Intuitive user interface

- **Game Mechanics**
  - Customizable target score
  - Score tracking system
  - Tie-breaker mechanism
  - Win/loss statistics

## Game Rules 👋

1. **Basic Rules**
   - Each player rolls 5 dice
   - Score is the sum of all dice faces
   - First to reach target score wins

2. **Turn Structure**
   - Initial roll of all dice
   - Option for up to 2 rerolls
   - Can select specific dice to keep between rerolls

3. **Winning**
   - Game continues until target score is reached
   - If both players reach target score in same number of attempts:
     - Higher score wins
     - If tied, one final throw decides winner

## Technical Details 🫠

### Built With
- Kotlin
- Jetpack Compose
- Material Design 3
- Android Studio

### Requirements
- Minimum SDK: 24
- Target SDK: 34
- Compile SDK: 34

## Installation 📝

1. Clone the repository

```bash
git clone https://github.com/dilshanmanohara/DiceGame.git
```

2. Open project in Android Studio
3. Run on an emulator or physical device

## Development Setup 💻

### Prerequisites
- Android Studio Hedgehog or newer
- JDK 21
- Android SDK with API 34

### Building

```bash
./gradlew build
```

## Project Structure 💽

```
app/
├── src/
│   ├── main/
│   │   ├── java/com/example/dicegame/
│   │   │   ├── MainActivity.kt # Main game logic and UI
│   │   │   └── ui/theme/ # Theme configuration
│   │   └── res/
│   │       ├── drawable/ # Dice images and icons
│   │       └── values/ # App resources
└── build.gradle.kts # Project configuration
```

## Game Components 🎯

1. **Main Screen**
   - Game logo with animated dice
   - New Game button
   - About section with game information

2. **Setup Screen**
   - Target score configuration
   - Game rules display
   - Start game option

3. **Game Screen**
   - Player's dice section
   - Computer's dice section
   - Score display
   - Reroll and scoring controls

## Computer Strategy 🤖

The computer opponent uses a value-based strategy:
- Always keeps 6s
- Keeps 5s if three or more dice are ≥ 4
- Keeps 4s if four or more dice are ≥ 3
- Rerolls everything else

This creates a balanced opponent that makes strategic decisions while still being beatable.

## Author 👨‍💻

- Student ID: 20232125
- Name: Dilshan Manohara

## License 📝

MIT License

Copyright (c) 2024 Dilshan Manohara

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Acknowledgments 🙏

- Material Design for UI components
- Android Jetpack libraries
- Kotlin and Jetpack Compose documentation

---

For issues, feature requests, or contributions, please open an issue or pull request in this repository.

