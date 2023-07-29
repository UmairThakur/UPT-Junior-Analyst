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
- **OPENAI_API_KEY**

## **Environment Variable**
- To run this project, you will need to add the following environment variable having the OpenAI API key stored. **`OPENAI_API_KEY`**

To set your OpenAI API key as an environment variable, you can follow these general steps:

1. **Locate your API Key**: If you already have an OpenAI API key, make sure you have it ready. If you don't have one, you'll need to sign up for an API key from the OpenAI website.

2. **Set the Environment Variable**: The specific method for setting environment variables varies depending on your operating system.

   - **For Windows**:
     - Open the Start menu and search for "Environment Variables."
     - Click on "Edit the system environment variables."
     - In the System Properties window, click the "Environment Variables" button.
     - In the Environment Variables window, under "System Variables," click "New."
     - Enter `OPENAI_API_KEY` as the variable name and paste your API key as the variable value.
     - Click "OK" to save the changes.

   - **For macOS and Linux**:
     - Open a terminal window.
     - Edit your shell profile file (`.bashrc`, `.bash_profile`, `.zshrc`, etc.) using a text editor such as `nano` or `vim`.
     - Add the following line at the end of the file:
       ```
       export OPENAI_API_KEY=your_api_key_here
       ```
     - Save the file and exit the text editor.
     - Run `source ~/.bashrc` (or `source ~/.bash_profile`, `source ~/.zshrc`, etc.) to apply the changes in your current terminal session. Alternatively, you can close and reopen the terminal.

3. **Verify the Environment Variable**:
   To verify that the environment variable is set correctly, you can open a new terminal or command prompt and type the following command (depending on your OS):

   - **For Windows**:
     ```
     echo %OPENAI_API_KEY%
     ```

   - **For macOS and Linux**:
     ```
     echo $OPENAI_API_KEY
     ```

   If everything is set up correctly, the command should output your API key.

Please note that you should treat your API key as sensitive information and avoid sharing it publicly or committing it to version control systems. If you're working on a shared system, it's better to use a more secure method for storing your API key, such as using a secrets manager or configuration file with restricted permissions.

## **Usage**
1. Run the 'UPT-Junior Analyst.exe'. It might take some time to load for the first time, as it will be installing the necessary dependencies.

   <img width="426" alt="00 - Run  exe" src="https://github.com/UmairThakur/UPT/assets/81063457/9d3f9c2c-753d-48b9-a85a-d0ff80c0d516">


2. Provide the path to the Excel file containing the dataset you want to analyze. If have a .csv file or want to use multiple .csv files, just paste every in a single Excel Workbook into different sheet(sheet name as the table name that you want, and **Save As 'Excel Workbook'**). Once the Data is Loaded you will see something like this.

   <img width="674" alt="03- data_loaded" src="https://github.com/UmairThakur/UPT/assets/81063457/6afdc9bf-0909-4818-9416-dcad48cbcc73">


The output will vary based on the user's selections:
- **1. Analyse the Data** 
    
    Will return SQL-like output and also an SQL query that you can run on the server to get the same output.
    
    <img width="769" alt="01 - Analyse" src="https://github.com/UmairThakur/UPT/assets/81063457/f6ac8981-80f9-4e9a-9550-5b8834facf53">


- **Data Visualization** 

    The script will generate charts or plots based on the provided Python code.

    <img width="770" alt="02 - Visualise" src="https://github.com/UmairThakur/UPT/assets/81063457/bfe2f54a-7a1b-43fe-931e-80cfeaeccd1b">

    Output:

    <img width="960" alt="02 - Visual Output" src="https://github.com/UmairThakur/UPT/assets/81063457/a3eb0fe0-773a-40fb-ae11-61e9fe16e7f9">

    If you requested for multiple charts, you will get each chart in a new Window.

- **Model Building** 
    
    The script will generate Python code for building the specified machine learning model.
    
    <img width="675" alt="03 - Model Building" src="https://github.com/UmairThakur/UPT/assets/81063457/c181f3a2-d6a5-4b32-812d-bf727993105c">

    Output:
    It not only will give you the Python code like Code Interpreter but it **goes one step further by also providing you with the errors that you may face while you run this code on your system.**

    <img width="675" alt="03 - output1" src="https://github.com/UmairThakur/UPT/assets/81063457/61b6cb0b-a03b-46a6-a3f1-c87e6349ff97">

    Example: Highlighting the Error here, as GPT didn't install sklearn as it cannot access your system, therefore UPT is showing the you may get this error while running the code.
    
    <img width="674" alt="03 - output2" src="https://github.com/UmairThakur/UPT/assets/81063457/b211c1bb-35a9-45c8-b822-f442ab9a7785">

  
    
    
- **Senior Analyst (Beta Version)** 
    
    Will provide insights and recommendations based on the data analysis, EDA, and model building process.
    ![screenshot.png](screenshot.png)

**Note:** Since, we are sharing limited data with the model and the parameter are set such that it commands the model to be verbose, if you get some errors for a specific prompt retry typing it in a different way.

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

