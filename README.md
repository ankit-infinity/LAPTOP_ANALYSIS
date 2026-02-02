# LAPTOP_ANALYSIS

# OVERVIEW

This project is all about finding meaningful insights related to laptop like 
best recommendation to each customer according to their profession using EDA
and analyzing the price of laptop using some models.The dataset includes various
features of laptop and find out the best possible models and related features
that effect the price of laptop.

# DATASET

1.Brand                 7.RAM_type              13 SSD
2.Name                  8.ghz                   14 HDD
3.Price                 9.display_type          15 Adapter
4.Processor_name        10.display              16battery life
5.Processor_brand       11.GPU
6.RAM_expandable        12.GPU_BRAND

# METHODOLOGY

 1. Data preparation:
  
  The dataset was cleaned and pre processed including handling missing values, 
  removing duplicates and outlier detection with outlier evaluation.
  
2.  Feature Engineering:

Extract meaningful info from  different variables.made variable much more 
interpretable using domain knowledge.

3. Exploratory Data Analysis(EDA):
 
Finding  distribution of various laptop features over price .Also finding top 
10 laptop (models,brands)for sale.For different customer recommendation 
regarding a which brand of laptop is best suited for them according to their demand.
 
 4. Modelling :
  
  A linear model and random forest regressor model was used to predict the 
  laptop price .Model assumption were checked to enure the validity of 
  linear regression .
  
5. Evaluation:

  model performance is evaluated using key metrics such as
  1.r2 score
  2.rmse
  
# Key finding and recommendation

Based on the above analysis we conclude some interesting facts:

1.Here we see brands like ('HP','LENOVO','DELL') are the top branding sales.

2.In processor brand distribution over price we see that processor brand like 'AMD' and 'intel' has 
  wide range over price distribution 

3.In Ram ditribution over price we see that ram like '16 GB','16GBLP'AND'32GB' has wider range over price
  distribution.
  
4.In brand distribution over price we see that brand like ('HP','LENOVO','DELL','ASUS','MSI')has wider range of price distribution while
  brand like (TECNO,XIAOMI,ZEBRONICS,MICROMAX,LAVA) has limited price range.
  
5.for students best laptop recoMmend according to their demand is ASUS,AVITA,DELL,HP.While for professions
  best recommended laptop is INFINIX,ASUS,ACER.

6.While comparing other feature with price we see that ram has high positive correlation with price while other feature
has low correlation.


# BEST MODEL SELECTION FOR PRICE PREDICTION:
 
  Here we test two model(linear regression ,random forest)for predicting the price under two different scenario one is with outlier and another without outlier


##  bias variance trade off insights:
  
  with outliers:
  
  high variance captured
  
  better generalization
  
  
  without outlier:
  
  lower variance 
  
  slightly lower prediction error
  
  but weaker model overall
  

# CONCLUSION:


From our analysis  of testing models for price prediction  we came to the conclusion that the random forest model with outlier is our best predictive model 
with highest test R2 score of 0.81  which indicates strong generalization and RMSE of 0.26 .Outlier in this case carry real information rather than noise.
though this selected model has slight overfitting (gap=of 14)but it is acceptable .
































