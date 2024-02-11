# Eat Safe, Love: UK Food Hygiene Ratings Analysis

![Project Banner](https://github.githubassets.com/images/icons/emoji/unicode/1f343.png) <!-- Leaf icon for nature/health -->

Welcome to the "Eat Safe, Love" project repository, where we delve into the vast data of UK food establishments to bring transparency and awareness to food hygiene ratings across the country. Our mission is to empower food enthusiasts, critics, and the general public with data-driven insights into the cleanliness and safety of restaurants, cafes, canteens, and other food establishments.

## Project Overview

This project is divided into three main parts, each crucial for analyzing and understanding food hygiene ratings within the UK:

1. **Database and Jupyter Notebook Setup**
2. **Update the Database**
3. **Exploratory Analysis**

## Part 1: Database and Jupyter Notebook Setup

![Setup Icon](https://github.githubassets.com/images/icons/emoji/unicode/2699.png)

### Objectives:
- Import food establishments data into MongoDB.
- Set up a Jupyter Notebook environment for data analysis.

### Methodology:
- **Data Import**: Use MongoDB command-line tools to import `establishments.json` into a MongoDB database named `uk_food`.
- **Library Imports**: Utilize PyMongo for database interaction and Pretty Print for clearer output formatting in Jupyter Notebooks.
- **MongoDB Connection**: Establish a connection to MongoDB through PyMongo to interact with the `uk_food` database.
- **Data Verification**: Ensure the successful import of data by listing databases, collections, and displaying a sample document.

## Part 2: Update the Database

![Update Icon](https://github.githubassets.com/images/icons/emoji/unicode/1f504.png)

### Objectives:
- Incorporate new restaurant data.
- Clean and update existing records to maintain data integrity.

### Tasks:
- **New Establishment Addition**: Add "Penang Flavours" to the `establishments` collection.
- **BusinessTypeID Update**: Determine and update the `BusinessTypeID` for the new restaurant.
- **Removal of Unwanted Data**: Exclude establishments within the Dover Local Authority from the dataset.
- **Data Type Corrections**: Convert latitude, longitude, and `RatingValue` to appropriate numeric types.

## Part 3: Exploratory Analysis

![Analysis Icon](https://github.githubassets.com/images/icons/emoji/unicode/1f50e.png)

### Objectives:
- Analyze the dataset to extract meaningful insights.
- Identify high-performing establishments and areas for improvement.

### Analysis Questions:
1. **Hygiene Score Analysis**: Identify establishments with a hygiene score equal to 20.
2. **Rating Value Analysis**: Find establishments in London with a `RatingValue` of 4 or higher.
3. **Proximity Analysis**: Determine the top 5 establishments with a `RatingValue` of 5, closest to "Penang Flavours".
4. **Local Authority Analysis**: Analyze hygiene scores across Local Authorities, focusing on scores of 0.

### Approach:
- Utilize MongoDB's `count_documents` and `find` for targeted queries.
- Employ aggregation pipelines for complex data aggregation and sorting tasks.
- Convert query results into Pandas DataFrames for detailed analysis and visualization.

## Acknowledgments

- Thanks to the UK Food Standards Agency for providing the dataset.
- Appreciation to all contributors and supporters of the "Eat Safe, Love" project.

## References

UK Food Standards Agency (2022). UK food hygiene rating data API. https://ratings.food.gov.uk/open-data/en-GB. Contains public sector information licensed under the Open Government Licence v3.0
Accessed Sept 9, 2022 and Sept 12, 2022 with the establishment settings as follows: longitude=51.5072, latitude=-0.1276, maxdistancelimit=4567, pagesize=10000, sortoptionkey=distance, pagenumber=(1,2,3,4,5,6,7,8).

![Footer Image](https://github.githubassets.com/images/icons/emoji/unicode/1f37d.png) <!-- Fork and knife with plate icon for food -->
