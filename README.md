# Coursera-recommender-system
This is the final project of Database labratoryat Shahid-Beheshti_University (SBU)

At this project we implemented a course-recommendation system for coursera web-site.

## Installation / Working

### Requirements

```bash
python 3.8+

pandas

tkinter

mysql

mysql.connector

pymysql

request

from sqlalchemy import create_engine

beautifulsoup4

packaging

```

Clone this repository or Download the files into your local system. 

- Extract the ZIP file (if you directly download from Github Web)
- Make sure all the files are in the same folder/directory
- Open main.ipynb and run all cells.

## Gathering Data
For doing this we request API of coursera witch give us some data of its courses and some information about them.

After gathering these information we create dataframe with them and save it on the database.

## Database
First of all we should connect to our DB and also define function for savinf data to DB.

For geting recommendation should get the datafarme from database and use it as .csv file 
by running query `SELECT * FROM DB_Name`

## Data Analysis
By doing some analysis and engineering on our dataset, make it ready for extract question that will be answered by user.

Also need some pre-processing like `str.replace()`, `copy()` and so on.

## Yes/No Questions
User throw a simple `UI/UX` should answer some questions and due to those answers get course(s) recommendation.

Thease questions are in **three** category witch each one of them has **three** sub-category as mentioned as bellow:

### Rating
- User see the "Should the rate of the course be less than 3.5? (yes/no): " question
- User will click on yes/no button at tkinter envierment
- We check that the user clicked the yes button or no button
- yes: Less than 3.5
- no: Greater or equal than 3.5

### Dificulty
1 . Beginer
- User see the "Should the Difficulty of the course be Beginer? (yes/no): " question
- User will click on yes/no button at tkinter envierment
- We check that the user clicked the yes button or no button
- yes: Beginer Difficulty
- no: return

2 . Intermediate
- User see the "Should the Difficulty of the course be Intermediate? (yes/no): " question
- User will click on yes/no button at tkinter envierment
- We check that the user clicked the yes button or no button
- yes: Beginer Difficulty
- no: return df

3 . Advanced
- User see the "Should the Difficulty of the course be Advanced? (yes/no): " question
- User will click on yes/no button at tkinter envierment
- We check that the user clicked the yes button or no button
- yes: Beginer Difficulty
- no: return df

### Skills
1 . Data Analysis
- User see the "Should the Skills of the course contain Data Analysis? (yes/no): " question
- User will click on yes/no button at tkinter envierment
- We check that the user clicked the yes button or no button
- yes: Beginer Difficulty
- no: return

2 . Programming
- User see the "Should the Skills of the course contain Programming? (yes/no): " question
- User will click on yes/no button at tkinter envierment
- We check that the user clicked the yes button or no button
- yes: Beginer Difficulty
- no: return

3 . Art
- User see the "Should the Skills of the course contain Art? (yes/no): " question
- User will click on yes/no button at tkinter envierment
- We check that the user clicked the yes button or no button
- yes: Beginer Difficulty
- no: return

## GUI Envierment
By using tkinter library in python create a `GUI` envierment for user to answer the questions.

Some iportant atribute for creating this envierment is mentioned in the following:
- `tk.Frame()`
- `tk.Label()`
- `tk.Button()`
- `pack()`
- `pack_forget()`

At the end this code give a dataframe of recommended course(s) to user.

## 🚀 Thanks

Thanks for looking into the project and being here. Feel free to share your reviews/suggestions/remarks! :)

**If you found it useful, leave a ⭐ here!**

## License

Ending Credits 
- Made using Python and tkinter
- @Author : [Farbod Fooladi](https://github.com/farbodfld)
- @Author : [Negin Mashayekhi](https://github.com/ngnma)
