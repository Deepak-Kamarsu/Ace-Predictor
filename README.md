# Predicting Tennis Serve: Ace or Not
This project presents the process and results of building a classification model to predict whether a tennis serve is an ace based on various features. The project involves data exploration, preprocessing, and modeling using the XGBoost algorithm.

## Methodology
The notebook, `ace_predictor_v2.ipynb` is the main file to run the model script.

The following steps were undertaken in the project:

**Data Exploration**: Analyzed the dataset's structure, including distributions of categorical and numerical features.

**Data Visualization**: Basic, univariat and bivariate analysis is performed using visualizations.

**Data Preprocessing**: Handled missing values, encoded categorical features, and analyzed feature correlations.

**Modeling**: Used the XGBoost algorithm, performed parameter tuning, and evaluated model performance.

**Key Visualizations** Few samples are shown in this ReadMe. The notebook explains this in detail.

  ***Player and Ball Coordinates:***
  
  <img width="691" alt="image" src="https://github.com/user-attachments/assets/672ef268-02df-4b49-ba92-d59fbdc20a3f" />
  
  This plot shows the distribution of player and ball positions during serves. This motivates in investing in data quality where huge improvement can be made.
  

  ***Model Feature Importance:***
  <img width="1053" alt="image" src="https://github.com/user-attachments/assets/fa69aaa8-d68d-4ed5-bced-fea23d3bba0f" />
  
  An example plot is shown here. This plot shows the importance of the feature(ball_bounce) that has an impact on deciding  ace/not.

**Evaluation**

 <img width="994" alt="image" src="https://github.com/user-attachments/assets/1c16810c-b36c-4f7d-824b-5111010e72c6" />

 The confusion matrix is plotted on a test data and Macro-Precision/Recall/F1 score are of primary interests.
 

## Prerequisites
This project includes a Jupyter Notebook named `ace_predictor_v2.ipynb`, which requires specific Python dependencies to run. Follow the steps below to set up the environment and execute the notebook.

- **Python**: Ensure `pyenv` is installed on your system for managing Python versions.
- **Taskfile**: Install the `task` CLI for managing tasks.
  - macOS/Linux:
    ```bash
    sudo apt install task
    ```
  - Windows: Download the binary from [Taskfile.dev](https://taskfile.dev).

## Setup Instructions

1. Clone the repository or download the project files.
   ```bash
   git clone <repository-url>
   cd <repository-folder>

2. Create a `./data` folder and place the data file(`task_set.csv`) in the folder

3. Set up Python and install dependencies:
    ```bash
    task setup

4.  If the dependencies are already locked in poetry.lock, you can install them directly:
    ```bash
    task install

5.  Run the below command for jupyter notebook to open in a browser
    ```bash
    task run
