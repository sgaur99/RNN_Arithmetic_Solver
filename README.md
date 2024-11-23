# RNN-Based Arithmetic Operation Solver

This project is an implementation of a Recurrent Neural Network (RNN) for performing basic arithmetic operations—addition, subtraction, and multiplication—on sequences of numerical inputs. The purpose is to explore how neural networks, specifically RNNs, can be trained to solve arithmetic problems that involve sequential data.

## Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Model Description](#model-description)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project aims to showcase the capability of RNNs in performing basic arithmetic operations. The implemented model takes two numbers as inputs, represented as sequences, and returns their arithmetic result. This type of problem is a great way to understand how RNNs can handle sequences of numerical data and learn complex transformations.

## Project Structure

The repository includes the following files and directories:

- `add_sub_mul_RNN.ipynb`: Jupyter notebook containing the code for data preprocessing, model building, training, and evaluation.
- `README.md`: Provides an overview of the project, setup instructions, and other useful information.
- `requirements.txt`: List of required Python packages.
- `LICENSE`: License for the project.

## Requirements

- Python 3.8 or higher
- TensorFlow 2.x
- NumPy
- Pandas
- Matplotlib

All dependencies can be installed using the `requirements.txt` file.

## Installation

1. **Clone the repository**

   ```sh
   git clone https://github.com/sgaur99/rnn-arithmetic-solve.git
   cd RNN_Arithmetic_Solver
   ```

2. **Create a virtual environment** (optional but recommended)

   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install dependencies**

   ```sh
   pip install -r requirements.txt
   ```

## Usage

### Running the Notebook

To explore the project interactively, open the Jupyter notebook:

```sh
jupyter notebook add_sub_mul_RNN.ipynb
```

### Training the Model

You can also train the model using the script:

```sh
python train_model.py
```

This script reads the dataset, preprocesses it, and trains the RNN model. Hyperparameters can be adjusted in the script.

### Making Predictions

To use the trained model for making predictions, use:

```sh
python predict.py --input "5 + 3"
```

Replace `"5 + 3"` with any arithmetic expression you want to solve.

## Model Description

The model is a Recurrent Neural Network (RNN) designed to solve basic arithmetic operations on sequences. It includes the following components:

- **Input Layer**: Takes in numerical sequences representing the numbers and the operation.
- **RNN Layers**: Consist of LSTM cells that learn sequential dependencies between input digits.
- **Output Layer**: Outputs the result of the arithmetic operation as a sequence.

## Results

- The model was trained on a dataset of generated arithmetic expressions and achieved good accuracy on addition, subtraction, and multiplication tasks.
- **Training Loss** and **Validation Loss** were plotted to visualize model convergence.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an issue if you have suggestions for improvements.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

