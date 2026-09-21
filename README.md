# Freight Rate Prediction Challenge

This repository contains a machine learning model built to predict freight rates based on geography, equipment type, and market conditions. The model uses a Random Forest Regressor trained on an 80/20 chronological time-series split.

## Setup Instructions

Follow these steps to set up the project on your local machine.

1. Open your terminal or command prompt.
2. Create a virtual environment to keep packages isolated:
   `python -m venv env`
3. Activate the virtual environment:
   `env\Scripts\activate`
4. Install the required packages and tools:
   `pip install -r requirements.txt`

## How to Run the Code

1. Start the Jupyter Notebook server:
   `jupyter notebook`
2. Open the `freight_rate_model.ipynb` file in your browser.
3. Run every cell in the notebook from top to bottom. This will execute the data pipeline, train the model, and generate the final CSV prediction files.

## How to Validate the Predictions

To verify the model outputs and generate the December price chart, run the provided scoring script in your terminal:

`python score.py --predictions validation_predictions.csv --december-predictions december-chart-inputs.csv`