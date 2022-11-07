# Identify-Customer-Segments

![Contributors](https://img.shields.io/github/contributors/walidsi/identify-customer-segments?style=plastic)
![Forks](https://img.shields.io/github/forks/walidsi/identify-customer-segments)
![Downloads](https://img.shields.io/github/downloads/walidsi/identify-customer-segments/total)
![Stars](https://img.shields.io/github/stars/walidsi/identify-customer-segments)
![Licence](https://img.shields.io/github/license/walidsi/identify-customer-segments)
![Issues](https://img.shields.io/github/issues/walidsi/identify-customer-segments)

### Goal
The goal of the project is to apply unsupervised learning techniques to identify segments of the population that form the core customer base for a mail-order sales company in Germany. These segments can then be used to direct marketing campaigns towards audiences that will have the highest expected rate of return.

### Process
- Assess and clean the population demographic data in order to convert it into a usable form.
- Use dimensionality reduction techniques (mainly PCA) to help surface the main signals and associations in the data.
- Organize the general population into clusters.
- Apply the techniques and models that were fit on the demographic data to the customers data.
- Compare the distribution of people by cluster for the customer data to that of the general population to identify the clusters of the population that should be targeted.

### Results
The analysis provided the following information about the popular demographic for the company:
- They are males (ANREDE_KZ = 1)
- living in micocells in PLZ8 with lower share of 6-10 family home (PLZ8_ANTG3 = 1)
- and no 10+ family homes (PLZ8_ANTG4 = 0)
- with estimated age 46+ years old (ALTERSKATEGORIE_GROB 3 and 4)
- with very high FINANZ_MINIMALIST (FINANZ_MINIMALIST = 5)
- with very high FINANZ_SPARER (FINANZ_SPARER = 1)
- with average affinity for SEMIO_TRADV and SEMIO_REL (SEMIO_TRADV and SEMIO_REL = 4)
- and high affinity for SEMIO_KAEM (SEMIO_KAEM = 3)

### Install

This project requires **Python 3.x** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [Seaborn](https://seaborn.pydata.org/)

You will also need to have software installed to run and execute an [iPython Notebook](http://ipython.org/notebook.html)

### Code

Code is provided in the `Identify_Customer_Segments.ipynb` notebook file.

### Run

In a terminal or command window, navigate to the top-level project directory (that contains this README) and run one of the following commands:

```bash
ipython notebook Identify_Customer_Segments.ipynb
```  
or
```bash
jupyter notebook Identify_Customer_Segments.ipynb
```

This will open the iPython Notebook software and project file in your browser.

### Data

The dataset consists of two files:
  - Udacity_AZDIAS_Subset.csv
  - Udacity_CUSTOMERS_Subset.csv

**Features**
- Features are defined in the Data_Dictionary.md file and AZDIAS_Feature_Summary.csv file.
