# **UPT - Junior Analyst**

## **Introduction**

An OpenAI based AI Tool for quick Data Analysis, Visualisation and model development but much more secure than Code Interpreter, as does not share the actual data, it processes the data locally and only shares the meta data such as column names, data types, etc. to generate the output.

## **Features**

The **"UPT - Junior Analyst"** is an application designed to assist Data Analysts in analyzing and working with datasets. It provides the following features:

1. **Data Analysis:** Users can perform data analysis similar to SQL queries on Excel datasets using natural language prompts.
2. **Data Visualization:** Users can generate various types of charts and plots using Python code, leveraging libraries like Matplotlib, Seaborn, and Plotly.
3. **Model Building:** Users can describe the model they want to build, including model type, hyperparameters, and columns for training and testing, and the script will generate the corresponding Python code.
4. **Senior Analyst:** Users can delegate the entire data analysis process to a "Senior Analyst persona" who will handle data cleaning, EDA, model selection, hyperparameter tuning, and visualization.

## **Requirements**

- **Python 3**
- **pip**
- **Environment Variable**
  - To run this project, you will need to add the following environment variable having the OpenAI API key stored. **`OPENAI_API_KEY`**

## **Usage**

1. Run the 'UPT-Junior Analyst.exe' and provide the path to the Excel file containing the dataset you want to analyze.

## **Output**

The output of the script will vary based on the user's selections:

- **Data Analysis**

  Will return SQL-like output and also an SQL query that you can run on the server to get the same output.
  ![screenshot.png](screenshot.png)

- **Data Visualization**

  The script will generate charts or plots based on the provided Python code.
  ![screenshot.png](screenshot.png)

- **Model Building**

  The script will generate Python code for building the specified machine learning model.
  ![screenshot.png](screenshot.png)

- **Senior Analyst (Beta Version)**
  Will provide insights and recommendations based on the data analysis, EDA, and model building process.
  ![screenshot.png](screenshot.png)

Since, we are sharing limited data with the model and the parameter are set such that it commands the model to be verbose, if you get some errors for a specific prompt retry typing it in a different way.

## **Limitations**

- The script relies on OpenAI's GPT-3.5 language model for natural language processing, which may not always produce accurate or desired results.
- Users should ensure that the dataset is clean and well-formatted to avoid errors during analysis and modeling.
- Complex queries or analysis may not be handled effectively by the language model.

## **Reporting Bugs or Issues**

If you encounter any bugs, issues, or have suggestions for improvements, please report them to me. You can contact me by sending an email to 'umairthakursocial@gmail.com'. Your feedback is valuable and will help enhance the tool's performance and user experience.

## **License**

This script is provided under the following license:

- You may use this application for personal, educational, or non-commercial purposes only.
- You may not use this application for any commercial purposes or distribute it for commercial gain.
- Attribution to the original author is required when sharing or modifying the application.

**Note:** The "UPT - Junior Analyst" script relies on external libraries, and their licenses and usage terms should be adhered to separately.
