# -DS-4002-Project-3-M3
This is the repository for analysis for Project 3 in DS 4002

## Section 1: Software and Platform

### Platform: Google Colab + Jupyter Notebook
### Language: Python 3
### Key Packages:
  - Pandas (data manipulation)
  - Numpy (numerical operation)
  - Tensor Flow (deep learning framework)
  - Matplotlib (accuracy and plotting)
  - Scikit-Learn (accuracy and classification

### This project was deveopled on MacOS and Windows

## Section 2: File Structure
```
├DS-4002-Project-3-M3/
│
├── DATA/ # Raw and processed data files
│ └── Where-to-Obtain.md # Relays how to obtain the data from MC Irvine Machine Learning Repository
│
├── OUTPUT/ # Generated charts and figures for reporting
│ ├── category_counts.png # From CategoryAmounts.ipynb, shows counts of images that belong to each waste type categories
│ ├── category_counts_aggregated.png # From CategoryAmounts.ipynb, shows counts of images that belong to three categories (recyclable, compostavle, and neither)
│ ├── cm_small_cnn.png # From Project3ItemClassModel.ipynb which shows a confusion matrix of how well the model was able to classify waste types
│ └── confusion_matrix_3class.png # From Project3WasteTypeModel.ipynb which shows a confusion matrix of the accuracy
│
├── SCRIPTS/ # Jupyter notebooks for analysis
│ ├── CategoryAmounts.ipynb # Our EDA code that demonstrates the numbers/ratios in waste type category and how many are recyclable, compostable, and neither.
│ ├── Project3ItemClassModel.ipynb # Creates a model that classifies based on waste type
│ └── Project3WasteTypeModel.ipynb # Creates a model that classifies based on if something is recyclable, compostable, or not
│
├── README.md # Project overview and instructions
└── LICENSE # License file
```


## Section 3: How To Reproduce

### 1. Set Up the Project Structure
Clone this repository and ensure your local folder structure matches the layout shown in **Section 2** of this README:

### 2.  Run the Data Analysis Code
Open and run the notebook: [Project3WasteTypeModel.ipynb](https://github.com/Bubcheeseburger/-DS-4002-Project-3-M3/blob/main/SCRIPTS/Project3WasteTypeModel.ipynb)
This notebook will:
- Load the **RealWaste** image folders and map the 9 original classes into 3 labels: **Recyclable**, **Compostable**, and **Trash**.  
- Split the images into **training, validation, and test** sets.  
- Build and train a **convolutional neural network (CNN)** on the training data to predict the 3 waste types.  
- Evaluate the model on the test set, reporting **accuracy, precision, recall, F1-score**, and a **confusion matrix**.  
- Save the trained model and result figures (plots and confusion matrix) into the `OUTPUT` folder.

### 3 (Optional).  Run Project3ItemClassModel.ipynb
Open and run the notebook: [Project3ItemClassModel.ipynb](https://github.com/Bubcheeseburger/-DS-4002-Project-3-M3/blob/main/SCRIPTS/Project3ItemClassModel.ipynb)
This notebook was the original data analysis, but due to low accuracy, the above was the chosen methodology. This will:
- Split the images into **training, validation, and test** sets.  
- Build and train a **convolutional neural network (CNN)** on the training data to predict the 3 waste types.  
- Evaluate the model on the test set, reporting **accuracy, precision, recall, F1-score**, and a **confusion matrix**.  
- Save the trained model and result figures (plots and confusion matrix) into the `OUTPUT` folder.
