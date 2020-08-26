# <div align="center">Predicting Passenger Survival</div>

### <div align="center">Project Overview</div>
Skills Demonstrated: *machine learning, exploratory data analysis, text analysis*<br/>
Libraries and Programs: *Python, Jupyter Notebook, pandas, numpy, regrex(re), seaborn*<br/>

Using the Titanic competition dataset available on Kaggle<sup>1</sup>, I created a model to predict which passengers would survive the 1912 sinking of the Titanic. The dataset includes passenger attributes such as Name, Age, Sex, and Economic Class, as well as information about their trip, such as their Cabin, Embarkment Location, and Ticket Price.<br>

### <div align="center">Exploratory Data Analysis</div>
#### 1. Know Your Data
I like to begin any analysis by learning some basics about the dataset. I want to know its shape (.shape), its columns (.columns), and their contents (.sample(), .describe(), .info(), .value_counts()).<br> 

**Figure 1.** Ten sample rows from the 'train' dataset.<br>

![alt_text](https://github.com/nphorsley59/Predicting_Passenger_Survival/blob/master/Figures/train_sample.png "'train' sample")<br>

Once I have a good understanding of the dataset, I like to visualize some of the distributions and relationships that I think might be informative. I like to use Seaborn (such as .distplot(), .barplot(), .boxplot(), and .scatterplot()) for straight-forward visualizations and Matplotlib.pyplot for visualizations that require more flexibility.<br>

**Figure 2.** A passenger's probability of surviving the wreck was non-random. It was strongly dependent on attributes such as age, sex, and economic class.<br>

![alt_text](https://github.com/nphorsley59/Predicting_Passenger_Survival/blob/master/Figures/agesexclass_survivalrate.png "Attributes Predicting Survival")<br>

Sometimes, it is helpful to bin features that have too many values to visualize neatly using pd.cut(). With text analysis tools like regrex, this is especially useful for grouping and ordering unordered, non-numerical values.<br>

**Figure 3.** Binning passenger cabin assignments by deck to see if deck level influenced survival.<br>

#### 2. Clean Your Data
Next, I like to clean and streamline my dataset so it is easy to work with. This includes tasks like dealing with NULL values, checking for errors, transforming skewed features, renaming unintuitive columns or values, removing outliers, and engineering new features. 

**Figure 4.**

#### 3. Strategize for Modeling

I conclude Exploratory Data Analysis by bringing everything I've learned about the dataset together to prepare for modeling. I like to identify important features in the dataset,  drop any data that won't benefit the model, and brainstorm a few promising modeling approaches.

**Figure 5.**

### <div align="center">Modeling</div>

### <div align="center">Resources</div>
<sup>1</sup> https://www.kaggle.com/c/titanic <br/>
