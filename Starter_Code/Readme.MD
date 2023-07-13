<h1>NoSQL Challenge: UK Food Ratings Analysis</h1>

<h2>Introduction</h2>
<p>The UK Food Standards Agency evaluates various establishments across the United Kingdom and assigns them food hygiene ratings. In this project, we analyze the ratings data to help the food magazine, Eat Safe, Love, make informed decisions about future articles and restaurant recommendations.</p>

<h2>Project Overview</h2>
<p>This project utilizes MongoDB, PyMongo, and Jupyter Notebook to perform the analysis. The dataset used is establishments.json, which contains information about different establishments and their food hygiene ratings.</p>

<h2>Part 1: Database and Jupyter Notebook Set Up</h2>
<ul>
  <li>The dataset is imported into the MongoDB database named 'uk_food' with the collection name 'establishments'.</li>
  <li>The data is verified by listing the databases, checking the presence of the 'uk_food' database, listing the collections, and displaying a document from the 'establishments' collection.</li>
</ul>

<h2>Part 2: Data Manipulation and Cleaning</h2>
<ul>
  <li>A new restaurant, "Penang Flavours," is added to the database using the provided dictionary of restaurant data.</li>
  <li>The BusinessTypeID of the new restaurant is updated based on the BusinessType.</li>
  <li>Duplicate documents are removed by ensuring uniqueness based on the BusinessName field.</li>
  <li>The data types of longitude, latitude, and RatingValue are converted from strings to numbers.</li>
  <li>RatingValues that are not in the range of 1-5 are set to null.</li>
  <li>Documents with LocalAuthorityName as "Dover" are deleted from the database.</li>
</ul>

<h2>Part 3: Exploratory Analysis</h2>
<p>Several questions are answered using MongoDB queries:</p>
<ol>
  <li>Number of establishments with a hygiene score of 20.</li>
  <li>Number of establishments in London with a RatingValue greater than or equal to 4.</li>
  <li>Top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant, "Penang Flavours".</li>
  <li>Number of establishments in each Local Authority area with a hygiene score of 0, sorted from highest to lowest.</li>
</ol>

<h2>Conclusion</h2>
<p>This project demonstrates how to perform data analysis on the UK food hygiene ratings dataset using MongoDB and PyMongo. The analysis provides insights into hygiene scores, ratings, and local authority areas, helping the food magazine make informed decisions about future articles and restaurant recommendations.</p>

<p>Please feel free to customize and enhance this summary based on your project's specific details and findings.</p>