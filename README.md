
#  NoSQL-CHALLENGE

## 📊UK Food Hygiene Ratings Evaluation
This project analyzes UK Food Standards Agency data to assist *Eat Safe, Love* magazine in crafting insightful articles  about food hygiene across the United Kingdom. Using MongoDB, Python libraries, and Jupyter Notebook, the analysis cleanses the dataset and provides  actionable insights for journalists and food critics.

---

## ✅Exploratory Analysis
**Key findings from the dataset include:**
-  **41 establishments** have a hygiene score of 20
-  **33 London establishments** have ratings ≥ 4
-  **Top 5 establishments near Penang Flavours** (rating value 5, hygiene score  0) :
   - Volunteer
   - Plumstead Manor Nursery
   - Atlantic Fish Bar
   - Howe and Co Fish and Chips - Van 17m
   - Iceland
-  **Thanet** tops the list of local authorities, with **1,130 establishments** having a hygiene score of 0.

---

## Setup/Usage Instructions
### Clone the repository:
    ``` bash 
    git clone <https://github.com/geraldine1456/nosql-challenge.git>

### Import the data set which contains food hygiene ratings and details about establishments across the UK
    ```bash
    mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json

-   Note:**`establishments.json`** file in the **`Resources`** folder

### Install dependencies:
-   **MongoDB**
-   **Python libraries:**
        **`PyMongo`**
        **`Pandas`**
        **`Pretty Print`** (`pprint`)
-   **Jupyter Notebook**

### Execution
-   **NoSQL_setup.ipynb:** Sets up the MongoDB database and refines records.
-   **NoSQL_analysis.ipynb** Runs queries to generate insights and summaries.

----

##  References
-   [UK Food Standards Agency](https://www.food.gov.uk/) (2022). UK food hygiene rating data API. [https://ratings.food.gov.uk/open-data/en-GB](https://ratings.food.gov.uk/open-data/en-GB) Contains public sector information licensed under the [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/)
Accessed Sept 9, 2022 and Sept 12, 2022 with the establishment settings as follows: longitude=51.5072, latitude=-0.1276, maxdistancelimit=4567, pagesize=10000, sortoptionkey=distance, pagenumber=(1,2,3,4,5,6,7,8).
-   [MongoDB Installer](https://www.mongodb.com/docs/mongodb-shell/)
-   [Pandas Documentation](https://pandas.pydata.org/docs/)
-   [W3Schools](https://www.w3schools.com/)
-   [Microsoft Copilot](https://copilot.microsoft.com/)  


