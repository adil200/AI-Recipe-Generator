
# AI Recipe Generator Web App

Welcome to the AI Recipe Generator web app project! This repository contains the code for a Flask-based web application designed to generate recipes based on just a few starting words. Below is an in-depth overview of the project, including details about the code, algorithms used, and the model-saving process.
### INPUT
![Screenshot 2024-01-30 at 2 50 16 PM](https://github.com/adil200/AI-Recipe-Generator/assets/75264739/e0042ff6-093c-488a-80b6-ec3977ecafba)
### OUTPUT
![Screenshot 2024-01-30 at 3 59 15 PM](https://github.com/adil200/AI-Recipe-Generator/assets/75264739/f935906b-557d-4c4f-84be-ecec641d2277)

## Overview

The main file, `app.py`, is the heart of the web application, integrating Flask, the underlying natural language processing model, and the recipe database. The application leverages state-of-the-art algorithms in natural language processing to understand user preferences and generate creative and personalized recipes. What makes this project unique is its ability to generate whole recipes with just 2-3 starting words provided by the user. Users can input specific constraints or preferences, and the application provides tailored recipe suggestions. The project includes HTML templates for the main and result pages, along with a CSS file for styling.

## Code Details

### Algorithms Used

The AI Recipe Generator utilizes advanced natural language processing algorithms, including recurrent neural networks (RNNs) and sequence-to-sequence models. These algorithms enable the system to grasp the nuances of recipe structures, ingredients, and cooking instructions. Additionally, the model incorporates attention mechanisms for better contextual understanding and creative text generation.

### Model Saving Process

The trained natural language processing model is a crucial component of the AI Recipe Generator. After training the model on a diverse dataset of recipes, it is saved using the `torch.save` function in PyTorch. This serializes the trained model and associated parameters to a file (e.g., `recipe_model.h5`). During the web application's runtime, Flask loads the saved model to generate recipes based on minimal starting words.

## Usage

1.  Clone this repository:

```bash
git clone https://github.com/adil200/AI-Recipe-Generator.git
cd AI-Recipe-Generator
```

2.  To run the web app, ensure you have the required dependencies installed. You can install them using the following command:

```bash
pip install -r requirements.txt
```

3.  Run the Flask application:

```bash
python app.py
```

4.  Open your web browser and go to [http://localhost:5000/](http://localhost:5000/) to access the AI Recipe Generator web app.
    
5.  Provide 2-3 starting words for your recipe, submit the form, and explore the detailed and creative recipe suggestions.
    

## Acknowledgments

This web app leverages Flask for web development and utilizes cutting-edge natural language processing techniques for recipe generation. Feel free to explore and customize the code to suit your specific culinary preferences.

Please note that the web app is currently set to run in debug mode. Ensure that it meets your security and deployment standards before deploying it in a production environment.
