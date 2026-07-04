# 7 Up 7 Down Game 🎲

A fun and interactive dice rolling game built with **Streamlit**. Guess whether the sum of two dice will be greater than 7, less than 7, or exactly 7!

## Features

- 🎮 **Interactive Gameplay**: Simple and intuitive user interface
- 🎲 **Dice Simulation**: Realistic random dice rolls (1-6 for each die)
- 🎯 **Three Betting Options**: 
  - **Up** - Guess the sum will be greater than 7
  - **Down** - Guess the sum will be less than 7
  - **Exact** - Guess the sum will be exactly 7
- ✅ **Instant Feedback**: Immediate win/loss notification

## Game Rules

1. Choose your guess: **'up'** (sum > 7), **'down'** (sum < 7), or **'exact'** (sum = 7)
2. Click the **"Roll Dice"** button
3. Two dice will be rolled (each showing 1-6)
4. Compare the total sum with your guess
5. Get instant feedback on whether you guessed correctly!

## Installation

### Prerequisites
- Python 3.7 or higher
- pip (Python package manager)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/samarthrana027/7up7down-game.git
   cd 7up7down-game
   ```

2. **Install Streamlit**
   ```bash
   pip install streamlit
   ```

3. **Run the application**
   ```bash
   streamlit run streamlit_pro_7up7down.py
   ```

4. **Open your browser**
   - The app will automatically open at `http://localhost:8501`
   - If it doesn't, manually navigate to the URL shown in your terminal

## How to Play

1. Open the game in your browser
2. Read the rules displayed on the screen
3. Select your prediction using the radio buttons:
   - Choose **"up"** if you think the dice sum will be greater than 7
   - Choose **"down"** if you think the dice sum will be less than 7
   - Choose **"exact"** if you think the dice sum will be exactly 7
4. Click the **"Roll Dice"** button
5. View the results and see if you guessed correctly!
6. Play as many times as you want

## Probability of Outcomes

| Outcome | Dice Combinations | Probability |
|---------|-------------------|-------------|
| **Down** (<7) | 2-3, 2-4, 2-5, ..., 6-6 | 15/36 ≈ 41.67% |
| **Exact** (=7) | 1-6, 2-5, 3-4, 4-3, 5-2, 6-1 | 6/36 ≈ 16.67% |
| **Up** (>7) | 2-6, 3-5, 3-6, ..., 6-6 | 15/36 ≈ 41.67% |

## Technologies Used

- **Streamlit** - Web application framework for creating interactive Python apps
- **Python** - Programming language
- **Random** - Python's built-in module for random number generation

## File Structure

```
7up7down-game/
├── README.md                      # Project documentation
└── streamlit_pro_7up7down.py     # Main game application
```

## Code Overview

### Main Components

- **`roll_dice()`** - Simulates rolling two dice and returns their individual values and sum
- **`play_7_up_7_down()`** - Main game logic that handles user input and determines win/loss

## Future Enhancements

- [ ] Score tracking and leaderboard
- [ ] Betting system with virtual currency
- [ ] Difficulty levels
- [ ] Sound effects
- [ ] Game statistics and history
- [ ] Multiplayer support

## Contributing

Contributions are welcome! Feel free to:
1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some improvement'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Open a Pull Request

## License

This project is open-source and available under the MIT License.

## Author

**Samarth Rana** - [@samarthrana027](https://github.com/samarthrana027)

## Acknowledgments

- Built with [Streamlit](https://streamlit.io/)
- Inspired by classic dice games

---

**Enjoy the game and good luck! 🎲**
