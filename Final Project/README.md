<!-- PROJECT TITLE -->
<br />
<div align="center">
  <h3 align="center">Rock-Paper-Scissors Agent</h3>

  <p align="center">
The goal of this project is to build an intelligent agent that learns to play the Rock-Paper-Scissors game.
  </p>
</div>



<!-- ABOUT THE PROJECT -->

## About The Project

The agent will bet €1 against a "Random Agent" for a total of N rounds. If our agent wins, it receives €2, in a tie it gets back €1, otherwise, it loses €1. The Random Agent always plays first, choosing a random image from the 2188 images available (Rock, Scissors, or Paper). The Random Agent is tricky and may apply vertical flip with a probability 𝑝1 = 0.5, followed by horizontal flip with a probability 𝑝2 = 0.5. Additionally, it introduces random noise to each pixel of the image. The Random Agent's function can be described as:

1. Map moves (Paper, Rock, Scissors) to (0, 1, 2, respectively).
2. Split the dataset into train-test: You can choose a percentage as a test set for each class.
3. Select Image: Choose a random image from the 2188 images.
4. Preprocess Image:
   - Apply Vertical Flip with probability 𝑝.
   - Apply Horizontal Flip with probability 𝑝.
   - Add noise with mean = 0, standard deviation = 255 * 0.05.
   - Optionally apply other image processing methods.
5. Send the preprocessed image to our agent.
6. The agent reads the image and selects the optimal action.
7. The goal is to maximize profit. Plot the agent's profit for each round.
8. Evaluate the accuracy of our agent on images outside the dataset.



<!-- Dataset -->

## Dataset

For training the agent, we utilized the following dataset, available [here](https://www.kaggle.com/datasets/drgfreeman/rockpaperscissors), which comprises of 700+ images for each move.



<!-- Built With -->

## Built With

* Python 3.10.12
* tensorflow: 2.15.0
* keras: 2.15.0
* gymnasium: 0.29.1
* matplotlib: 3.7.1
* seaborn: 0.13.1
* numpy: 1.23.5
* scikit-learn: 1.2.2



<!-- GETTING STARTED -->

## Usage
1. Clone the repository.
2. Open the provided Google Colab notebook.
3. Ensure the required libraries are installed.
4. Run the notebook cells to train and test the Rock-Paper-Scissors agent.
5. Evaluate the agent's accuracy on external images.



<!-- Results -->

## Results
Check the provided Google Colab notebook for the overall performance of the agent and the plotted profit per round.



<!-- LICENSE -->

## License

Distributed under the MIT License. See `LICENSE.txt` for more information.