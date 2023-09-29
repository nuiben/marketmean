<p align="center">
  <img src="assets/market_mean_logo.png">
</p>

<p align="center">
  <img src="https://img.shields.io/github/license/nuiben/marketmean?style=for-the-badge">
  <img src="https://img.shields.io/github/stars/nuiben/marketmean?style=for-the-badge">
  <img src="https://img.shields.io/github/issues/nuiben/marketmean?color=blueviolet&style=for-the-badge">
  <img src="https://img.shields.io/github/forks/nuiben/marketmean?color=teal&style=for-the-badge">
  <img src="https://img.shields.io/github/issues-pr/nuiben/marketmean?color=tomato&style=for-the-badge">
</p>
<hr>
<p align="center">AI Laptop Price Predictor</p>
<p align="center">Author: Ben Porter</p>
<hr>
<p> Pulled from a [Kaggle Library](https://www.kaggle.com/datasets/juanmerinobermejo/laptops-price-dataset) (Merino, 2023), this csv text data originates from a Spanish website containing information on PC components. Prices are based on regional currencies, so the nominal value should not be considered to reflect currency adjustments or inflation. As the data was primarily created using Euros, this is the most appropriate figure for describing the final price. For training, we split the data for preprocessing amongst the categorical and nominal datasets.</p>
<p align="center">
  <img src="assets/figure_a1.png">
</p>
<p>From these two classifications, the model’s preprocessor can interpret categorical features based on their unique values before merging them with the nominal data. Now that we’ve described the breadth of the data, we should represent the depth. Figure A-2 below shows that this dataset represents 2,160 records, and its numerical data ranges for each feature are also listed.</p>
<p align="center">
  <img src="assets/figure_a2.png">
</p>

<ul>
  <li><b>Mean Absolute Error (MAE):</b> This metric measures the average of the absolute differences between predicted and actual values. It provides a clear and direct interpretation of how far off our predictions were, on average.</li>
<li><b>Mean Squared Error (MSE): </b> MSE gives the average of the squared differences between predicted and actual values. It penalizes larger errors more severely than smaller ones, which makes it particularly useful when we want to identify significant discrepancies in predictions.</li>
<li><b>R-Squared Score: </b>This metric provides an indication of how well the input data explain the variance in the output, dependent variables. The closer the R-Squared value is to 1, the more confidence the model has in the relationship between input and output (Fernando 2023).</li>
</ul>

<p align="center">
  <img src="assets/figure_d7.png">
</p>


<h2><b>Installation</b></h2>

<p>For Installation of MarketMean on Windows 10/11.</p>
<ol>
  <li>Visit Python.org</li>
  <ul>
    <li><a href="https://www.python.org/downloads/">Download the latest version of Python 3 for Windows.</a></li>
    <li>Run the installer. Be sure to add Python to PATH.</li>
  </ul>
  <br>
  <li>Install Jupyter Notebook:</li>
  <ul>
    <li>Open Command Prompt as an administrator.</li>
    <li>Enter the following command: `pip install notebook`</li>
    <li>Once installation is complete, you can launch Jupyter Notebook by entering: `jupyter notebook`</li>
    <li>For Git Bash the run: `python -Xfrozen_modules=off -m notebook`</li>
  </ul>
  <br>
  <li>Install Required Python Libraries</li>
  <ul>
    <li>wheel</li>
    <li>pandas</li>
    <li>sklearn</li>
    <li>numpy</li>
    <li>joblib</li>
    <li>ipywidgets</li>
    <li>IPython</li>
  </ul>
  <br>
  <li>Run marketmean.ipynb.</li>
  <ul><li>This is where the first read of the “laptops.csv” file is conducted by Pandas, and the dataframe object is construct, and the raw data is processed.</li></ul>
  <li>Proceed to Section 2 “Crafting and Training MarketMean”.</li>
  <ul><li>If your machine has the “joblib” module already installed from Anaconda, your “joblib” import call might be located in “sklearn.externals” or “sklearn.extensions”.</li></ul>
  <br>
  <p align="center"><i>Optionally, if you would like to train a new model, you can uncomment lines 35-40.</i></p>
  <p align="center">
    <img src="assets/figure_x01.png">
  </p>
  <li>Section 3 Training Performance Results. Load the joblib file with the correct name. Your results will be printed below.</li>
  <li>Section 4 Configure your own Laptop:</li>
  <p align="center">
    <img src="assets/figure_x02.png">
  </p>
</ol>
