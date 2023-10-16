# nosql-challenge

This README file provides an overview of the tasks completed during the Data Analytics Bootcamp challenge related to the evaluation of food hygiene ratings data for the "Eat Safe, Love" magazine. The challenge is divided into three parts, each focusing on different aspects of data setup, database updates, and exploratory analysis.

## Part 1: Database and Jupyter Notebook Set Up

In this section, we set up the database and Jupyter Notebook environment to work with the provided data.

**Database Setup:**

- Imported the data from the `establishments.json` file into a MongoDB database named `uk_food` and a collection named `establishments`.
- The following commands were used to import the data from the Terminal:
  
  ```bash
  mongoimport --db uk_food --collection establishments --file establishments.json
  ```

**Jupyter Notebook Environment Setup:**

- Imported the necessary libraries, including PyMongo and Pretty Print (pprint).
- Created an instance of the Mongo Client to connect to the MongoDB database.
- Confirmed the successful setup by listing the databases and collections and displaying a sample document using `find_one`.

## Part 2: Update the Database

In this section, we made modifications to the database.

**Database Updates:**

- Added a new restaurant, "Penang Flavours," to the database with the provided information. 
- Found the `BusinessTypeID` for "Restaurant/Cafe/Canteen" and updated the new restaurant's entry with the correct `BusinessTypeID`.
- Checked for establishments within the "Dover" Local Authority, and subsequently removed them from the database.
- Converted certain number values stored as strings to actual numbers using `update_many`.

## Part 3: Exploratory Analysis

In this section, we conducted exploratory analysis on the database to answer specific questions.

**Exploratory Analysis:**

- Identified establishments with a hygiene score equal to 20.
- Found establishments in London with a `RatingValue` greater than or equal to 4, considering variations in the Local Authority name.
- Determined the top 5 establishments with a `RatingValue` of 5, sorted by lowest hygiene score, nearest to the new restaurant, "Penang Flavours."
- Calculated the number of establishments in each Local Authority area with a hygiene score of 0, sorted from highest to lowest.

## Conclusion

This README provides an overview of the tasks completed during the Data Analytics Bootcamp challenge.

For more detailed information and code implementation, refer to the provided Jupyter Notebook files: `NoSQL_setup_starter.ipynb` and `NoSQL_analysis_starter.ipynb`.

Please note that additional documentation and code comments are available within the Jupyter Notebook files to provide a comprehensive understanding of the analysis process.

## Disclosure

README file formatted by GPT4
