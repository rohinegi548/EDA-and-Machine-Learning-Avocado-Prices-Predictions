# EDA-and-Machine-Learning-Avocado-Prices-Predictions
Exploratory Data Analysis and Price Predictions for Avocado Dataset based on Machine Learning

<h1>Avocado Dataset Analysis and ML Prediction</h1>
<ul>
  <h2>Table of Contents</h2>
  <li>Problem Statement</li>
  <li>Data Loading and Description</li>
  <li>Data Profiling
    <ul>
      <li>Understanding the Dataset</li>
      <li>Profiling</li>
      <li>Preprocessing</li>
    </ul>
<li>Data Visualisation and Questions answered
  <ul>
    <li>Q.1 Which type of Avocados are more in demand (Conventional or Organic)?</li>
    <li>Q.2 In which range Average price lies, what is distribution look like?</li>
    <li>Q.3 How Average price is distributed over the months for Conventional and Organic Types?</li>
    <li>Q.4 What are TOP 5 regions where Average price are very high?</li>
    <li>Q.5 What are TOP 5 regions where Average consumption is very high?</li>
    <li>Q.6 In which year and for which region was the Average price the highest?</li>
    <li>Q.7 How price is distributed over the date column?</li>
    <li>Q.8 How dataset features are correlated with each other?</li>
  </ul>
<li>Feature Engineering for Model building</li>
<li>Model selection/predictions
  <ul>
    <li>P.1 Are we good with Linear Regression? Lets find out.</li>
    <li>P.2 Are we good with Decision Tree Regression? Lets find out.</li>
    <li>P.3 Are we good with Random Forest Regressor? Lets find out.</li>
  </ul>
<li>Lets see final Actual Vs Predicted sample.</li>
<li>Conclusions</li>
</ul>

<h2>Problem Statement</h2>
<ul>
<li>The notebooks explores the basic use of Pandas and will cover the basic commands of (EDA) for analysis purpose.</li>

<li>In this study, we will try to see if we can predict the Avocado’s Average Price based on different features. The features are different (Total Bags,Date,Type,Year,Region…).</li>

The variables of the dataset are the following:
<li>Categorical: ‘region’,’type’</li>
<li>Date: ‘Date’</li>
<li>Numerical:’Total Volume’, ‘4046’, ‘4225’, ‘4770’, ‘Total Bags’, ‘Small Bags’,’Large Bags’,’XLarge Bags’,’Year’</li>
<li>Target:‘AveragePrice’</li>
</ul>

<h2>Data Loading and Description</h2>

<p>
This data was downloaded and provided by INSAID, from the Hass Avocado Board website in May of 2018 & compiled into a single CSV.
Represents weekly 2018 retail scan data for National retail volume (units) and price.
The dataset comprises of 18249 observations of 14 columns. Below is a table showing names of all the columns and their description.
</p>

The unclear numerical variables terminology is explained in the next section:

<table>
  <tr><th>Features</th><th>Description</th></tr>
  <tr><td>‘Unamed: 0’</td><td>	Its just a useless index feature that will be removed later</td></tr>
  <tr><td>‘Total Volume’</td><td>	Total sales volume of avocados</td></tr>
  <tr><td>‘4046’</td><td>	Total sales volume of Small/Medium Hass Avocado</td></tr>
  <tr><td>‘4225’</td><td>	Total sales volume of Large Hass Avocado</td></tr>
  <tr><td>‘4770’</td><td>	Total sales volume of Extra Large Hass Avocado</td></tr>
  <tr><td>‘Total Bags’</td><td>	Total number of Bags sold</td></tr>
  <tr><td>‘Small Bags’</td><td>	Total number of Small Bags sold</td></tr>
  <tr><td>‘Large Bags’</td><td>	Total number of Large Bags sold</td></tr>
  <tr><td>‘XLarge Bags’</td><td>	Total number of XLarge Bags sold</td></tr>
</table>

