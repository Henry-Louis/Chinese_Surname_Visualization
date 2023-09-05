# Chinese Surname Visualization

## Table of Contents
1. Introduction
2. Prerequisites
3. File Structure
4. Code Overview
5. How to Run the Code
6. Acknowledgements

---

## 1. Introduction
This project consists of Python code designed to visualize embeddings of Chinese surnames using t-SNE (t-distributed Stochastic Neighbor Embedding). It is implemented in a Jupyter Notebook, with cells that import required packages, define functions, read and preprocess data, perform t-SNE transformations, and finally, plot the results.

## 2. Prerequisites

### Software and Packages
- Python 3.x
- Pandas
- OpenAI
- scikit-learn
- Matplotlib
- Plotly (optional)

### Data
- A text file named `baijiaxing.txt` containing Chinese surnames.
- OpenAI API key

## 3. File Structure
- `readme.md`: This readme file.
- `project_notebook.ipynb`: Jupyter notebook containing the code.

## 4. Code Overview

### Import Statements
Various Python packages are imported for data manipulation, plotting, and API requests.

```python
import pandas as pd
import openai
from sklearn.manifold import TSNE
import matplotlib.pyplot as plt
import matplotlib.font_manager as fm
```

### API Initialization
Initialize the OpenAI API with your key.

```python
openai.api_key = "YOUR_API_KEY_HERE"
```

### Functions
- `get_embedding()`: Calls the OpenAI API to get the embedding for a given surname.

### Data Preprocessing
- Reads a file `baijiaxing.txt` containing Chinese surnames and processes it into a DataFrame.

### t-SNE Transformation
- Performs a t-SNE transformation on the embeddings to create 2D and 3D representations.

### Visualization
- Utilizes Matplotlib for a 2D scatter plot.
- Utilizes Plotly for an optional 3D scatter plot.

## 5. How to Run the Code
1. Clone the repository.
2. Install the prerequisites mentioned above.
3. Replace `"YOUR_API_KEY_HERE"` with your OpenAI API key.
4. Place the `baijiaxing.txt` file in the same directory as the Jupyter notebook.
5. Run all the cells in the notebook to execute the code.

## 6. Acknowledgements
The code uses OpenAI’s API to fetch embeddings and scikit-learn's t-SNE algorithm for dimensionality reduction. 

---

Last Updated: September 5, 2023
