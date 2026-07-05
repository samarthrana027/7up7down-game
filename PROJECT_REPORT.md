# 7 Up 7 Down — Project Report

Author: samarthrana027
Repository: 7up7down-game

## Project Summary

7 Up 7 Down is a lightweight Streamlit web app that simulates rolling two six-sided dice and lets the user guess whether the sum will be "up" (greater than 7), "down" (less than 7), or "exact" (exactly 7). The app provides immediate feedback indicating whether the guess is correct.

## Files

- `streamlit_pro_7up7down.py` — Main Streamlit application implementing the dice roll and game logic.

## How it works

- The app uses Python's `random` module to generate two integers in the range [1, 6].
- The sum is computed and compared against the player's guess selected via a Streamlit radio input (`up`, `down`, `exact`).
- When the user clicks "Roll Dice", the app shows the two dice values, their total, and whether the guess was correct.

Key function:
- `roll_dice()` — returns `(dice1, dice2, total)` where dice1 and dice2 are random integers 1..6.

## Installation

1. Install Python 3.8+.
2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # Mac/Linux
   .venv\Scripts\activate     # Windows
   ```
3. Install dependencies:
   ```bash
   pip install streamlit
   ```
4. Run the app:
   ```bash
   streamlit run streamlit_pro_7up7down.py
   ```

## Usage

- Open the local Streamlit URL displayed after running the app.
- Choose one of the three options (up / down / exact) and click "Roll Dice".
- The app will display the two dice values, their sum, and a success or error message.

## Example scenarios

- Dice roll 4 and 5: total = 9 -> correct guess is `up`.
- Dice roll 2 and 3: total = 5 -> correct guess is `down`.
- Dice roll 1 and 6: total = 7 -> correct guess is `exact`.

## Limitations & Notes

- The UI accepts exactly three choices and uses a simple `st.radio` control.
- The app currently has no persistent state across runs and no logging of previous results.
- No automated tests are provided in the repo.

## Possible Improvements

- Add a scoreboard to track wins/losses across rounds and sessions.
- Add unit tests for the core logic (e.g., `roll_dice`, result-evaluation).
- Add CI (GitHub Actions) to run linting and tests.
- Improve UX: animations, dice images, and history of recent rolls.

## License

Include a LICENSE file if you want to specify licensing. Currently none is provided.

## Contact

Repository owner: @samarthrana027

