# Disaster-Response-Pipelines Project(NLP)
 This project was completed as part of the course requirements of Udacity's [Data Scientist Nanodegree](https://www.udacity.com/course/data-scientist-nanodegree--nd025) certification.
 
 ## Overview
The project used a data set from [Figure Eight](https://www.figure-eight.com/) that contained labeled disaster messages received by an aid organization. A multi-output Random Forrest classifier was trained using supervised learning with a natural language processing (NLP).
We will be working with a data set provided by [Figure Eight](https://www.figure-eight.com/) containing real messages that were sent during disaster events.


## Project Description
In this project, we will build a model to classify messages that are sent during disasters. There are 36 pre-defined categories, and examples of these categories include Aid Related, Medical Help, Search And Rescue, etc. By classifying these messages, we can allow these messages to be sent to the appropriate disaster relief agency.

Finally, this project contains a web app where you can input a message and get classification results.

![Screenshot of Web App](https://github.com/kumarAjeetsingh/Disaster-Response-Pipeline-Project/blob/master/web_app.png)

## File Description
~~~~~~~
        disaster_response_pipeline
          |-- app
                |-- templates
                        |-- go.html
                        |-- master.html
                |-- run.py
          |-- data
                |-- disaster_message.csv
                |-- disaster_categories.csv
                |-- DisasterResponse.db
                |-- process_data.py
          |-- models
                |-- classifier.pkl
                |-- train_classifier.py
          |-- Preparation
                |-- ETL Pipeline Preparation.ipynb
                |-- ML Pipeline Preparation.ipynb
                |-- README
          |-- README
~~~~~~~
## Installation
Must runing with Python 3 with libraries of numpy, pandas, sqlalchemy, re, NLTK, pickle, Sklearn, plotly and flask libraries.

## File Descriptions
1. App folder including the templates folder and "run.py" for the web application
2. Data folder containing "DisasterResponse.db", "disaster_categories.csv", "disaster_messages.csv" and "process_data.py" for data cleaning and transfering.
3. Models folder including "classifier.pkl" and "train_classifier.py" for the Machine Learning model.
4. README file
5. Preparation folder containing 6 different files, which were used for the project building. (Please note: this folder is not necessary for this project to run.)


### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/http://view6914b2f4.3001/( open another Terminal window. Type `env|grep WORK`. You'll see output contains SPACEID and SPACEDOMAIN. 
<br> In a new web browser window, type in the following: `https://SPACEID-3001.SPACEDOMAIN`. Subsitute the corresponding elements in the web address with the SPACEID and SPACEDOMAIN in the terminal window. Then, press Enter.)

# Licensing, Authors, Acknowledgements
Many thanks to Figure-8 for making this available to Udacity for training purposes. Special thanks to udacity for the training. Feel free to utilize the contents of this while citing me, udacity, and/or figure-8 accordingly.
