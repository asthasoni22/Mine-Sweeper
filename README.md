# Minesweeper AI

This is a knowledge-based AI implementation of the classic Minesweeper game. The AI uses logical inference to deduce safe moves and mine locations based on revealed board information.

## Features
- **Automated Play**: The AI can make safe moves and infer mine positions.
- **Knowledge-Based Reasoning**: Uses logical sentences to deduce information.
- **Random Moves**: Makes a random move when no safe move is available.
- **Pygame Visualization**: A `runner.py` script is provided for visualizing the game.

## Installation
To install required dependencies, run:
```sh
pip install -r requirements.txt
```

## Usage
Run the visualization with:
```sh
python runner.py
```

## Files
- `minesweeper.py`: Core logic of the Minesweeper game and AI.
- `runner.py`: Pygame-based visualization for playing the game.
- `requirements.txt`: List of dependencies needed to run the game.

## How the AI Works
The AI maintains a knowledge base of logical sentences representing constraints on mine locations. It:

- **Marks Safe Moves**: If a cell is determined to be safe, it is added to the safe set.
- **Marks Mines**: If a cell is determined to be a mine, it is flagged.
- **Updates Knowledge**: It refines its knowledge base by deriving new sentences from existing ones.
- **Makes Moves**: If a safe move exists, it is chosen; otherwise, a random move is made.


