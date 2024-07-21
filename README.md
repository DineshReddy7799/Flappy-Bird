# Flappy-Bird
# Flappy Bird NEAT AI

This project is an implementation of the classic Flappy Bird game using NEAT (NeuroEvolution of Augmenting Topologies) to evolve neural networks to play the game autonomously. The game is developed using Python and Pygame, and the NEAT library is used for the evolutionary algorithm.

## Requirements

- Python 3.x
- Pygame
- NEAT-Python

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/flappy-bird-neat.git
   cd flappy-bird-neat
   ```

2. Install the required libraries:

   ```bash
   pip install pygame neat-python
   ```

3. Place the required images (`bird1.png`, `bird2.png`, `bird3.png`, `pipe.png`, `base.png`, `bg.png`) in an `imgs` directory inside the project folder.

## How to Run

1. Ensure that you have the NEAT configuration file (`config-feedforward.txt`) in the project directory.
2. Run the main script:

   ```bash
   python main.py
   ```

## Code Overview

### Constants

- `WIN_WIDTH` and `WIN_HEIGHT`: Dimensions of the game window.
- `GEN`: Global variable to keep track of the current generation.
- `BIRD_IMGS`, `PIPE_IMG`, `BASE_IMG`, `BG_IMG`: Images for the bird, pipe, base, and background respectively.
- `STAT_FONT`: Font used for displaying the score and generation.

### Classes

#### Bird
- Handles the bird's properties and behaviors such as jumping, moving, drawing, and collision detection.

#### Pipe
- Handles the pipe's properties and behaviors such as setting height, moving, drawing, and collision detection.

#### Base
- Handles the base's properties and behaviors such as moving and drawing.

### Functions

#### `draw_window(win, birds, pipes, base, score, gen)`
- Draws the game window including the background, pipes, base, birds, score, and generation number.

#### `main(genomes, config)`
- Main function that runs the game for each generation, evaluates the birds' performance, and evolves the population using the NEAT algorithm.

#### `run(config_path)`
- Loads the NEAT configuration and initializes the population. Runs the NEAT algorithm for a specified number of generations.

## NEAT Configuration

The NEAT configuration file (`config-feedforward.txt`) specifies the parameters for the neural network and the evolutionary algorithm. Ensure it is properly set up according to your needs.

## Usage

This project demonstrates how NEAT can be used to train neural networks to play Flappy Bird. You can modify the NEAT configuration file and the game parameters to experiment with different setups and observe how the AI evolves.

## Acknowledgements

- [NEAT-Python](https://neat-python.readthedocs.io/en/latest/) library
- Pygame library for game development

Feel free to contribute to this project by opening issues or submitting pull requests. Enjoy the game and happy coding!
