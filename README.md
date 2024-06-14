# Team_65

This repository contains code and outputs for two tasks along with their respective preprocessing steps.

## Folders:

### task1
Contains files related to Task 1.

- `task1_preprocessing.ipynb`: Jupyter notebook for preprocessing data related to Task 1.
- `task1.ipynb`: Main Jupyter notebook for Task 1.
- `final.pth`: Model for Task 1.

### task2
Contains files related to Task 2.

- `task2_preprocessing.ipynb`: Jupyter notebook for preprocessing data related to Task 2.
- `task2.ipynb`: Main Jupyter notebook for Task 2.

### team_65_results
Contains output files generated from the tasks.

- `behaviour_simulation_test_company.xlsx`: Prediction of likes ( **predicted_likes** column) for tweets of unseen brands.
- `behaviour_simulation_test_time.xlsx`: Prediction of likes ( **predicted_likes** column) for tweets of unseen time period.
- `content_simulation_test_company.xlsx`: Prediction of content ( **output** column) for tweets of unseen brands.
- `content_simulation_test_time.xlsx`: Prediction of content ( **output** column) for tweets of unseen time period.

## Usage:

### task1
- Upload any dataset for task 1 in the correct directory and run the preprocessing notebook for task 1 (`task1_preprocessing.ipynb`).
- This preprocessing notebook generates an excel file which is the original dataset along with a new column **followers**.
- We manually added the followers for the usernames which had empty entries in the followers column. 
- Upload this excel file (the file with the original dataset + followers column) in the correct directory.
- Upload the model `final.pth` in the same directory and run the main notebook for task 1 (`task1.ipynb`).
- The predicted likes are saved as a column **predicted_likes** in a new excel file along with the dataset.
- All dependencies and libraries required for running the notebooks are installed when the first cell of `task1.ipynb` is executed.

### task2
- **Note :** The main notebook for task 2 has to run on a GPU (due to mistralai/Mistral-7B-Instruct-v0.1 contraints).
- Upload any dataset for task 2 in the correct directory and run the preprocessing notebook for task 2 (`task2_preprocessing.ipynb`).
- This preprocessing notebook generates an excel file which is a mapping between companies and their respective sectors.
- We manually added the sectors using wikidata for the companies which had empty entries in the sector column. 
- Upload this excel file (company-sector mapping) in the correct directory.
- Upload the dataset for task 2 in the same directory and run the main notebook for task 2 (`task2.ipynb`).
- The generated content is saved as a column **output** in a new excel file along with the dataset.
- All dependencies and libraries required for running the notebooks are installed when the first cell of `task2.ipynb` is executed.
