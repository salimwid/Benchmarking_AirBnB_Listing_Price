# Benchmarking_Airbnb_Listing_Price
This project aims to predict AirBnB listing price in London using sentiment analysis and Machine Learning models.

#### Models Deployed
Recommender System (Similarity Matrix), Natural Language Processing (NLP), Sentiment Analysis, Regression Model (Tree Based, Stacked Tree and Neural Network based models), Global and Local Explainability (SHAP Values and LIME).

#### Techniques Employed
Data Mining, Exploratory Data Analysis, Feature Engineering, Text Mining, Data Visualization, Machine Learning, Parallel Processing.

#### Tools Employed
Pickle, sklearn, TensorFlow, Keras, VADER, NLTK, Google Map API, Plotly

### Context
With a market valuation of USD$104B, Airbnb is the go-to platform for on-demand rentals. But with inflationary pressures weighing down on discretionary spending, the question of how to sustain growth post the pandemic becomes pressing. <br> 

The paper tackles: <br>
(a) the key role of hosts <br>
(b) how Airbnb can leverage on ML driven benchmarking and price prediction models to help property owners and their proxies calibrate price and amenity offerings.<br>

These two key contributions are especially important as COVID-19 has changed the dynamics of travel globally, with the shifts in guest behaviour driven by the prevalence of remote work and price sensitivity due to post-pandemic economic climate.

### Datasets
The main dataset adopted in this project was acquired from Inside Airbnb which was a publicly available dataset for Airbnb price listing. In this project, the main focus was listing price in London as it was the city with the most Airbnb listings. There were 2 key files used: <strong> Detailed listing file </strong> and <strong> user reviews file </strong>. <br> Detailed listing file had 66,641 unique listings with over 74 attributes and across 5 main categories. Meanwhile, user reviews file had 1,043,004 reviews with meta features on listing id, reviewer id, date and reviews description. <br>

The main dataset was enriched using data from Google Maps API which added tube station details and location to the listing information. The clean aggregated dataset has 65 features, 32 one hot encoding features and 33 numerical features. <br>

### Chosen Model & Performance
To process the list reviews, NLP and sentiment analysis were done. The sentiment was then translated as a feature in the dataset. <br>

To estimate listing price and identify important features, regression models were adopted. Two families of non-linear regression models, tree-based (ensemble and boosting methods) and neural network models, were chosen. Chosen models include LightGBM, XGBoost, Random Forest, Deep Neural Network and Wide Neural Network. Simple OLS was done as a baseline comparison for the models. In order to have a thorough understanding of the results, SHAP values and Permutation Feature Importance (PFI) were adopted. Both models highlighted the important features and their effect on price for specific units. <br>

Meanwhile, recommender system was adopted to benchmark a listed property against listings that are most similar to it. The recommender system was based on similarity matrix of the listings. Due to the absence of user interaction data, it was not possible to come up with an evaluation metric for the system.

<br>
### Collaborators
Gino Tiu <br>
Widya Salim <br>
Georgius Gary Gunawan <br>
Susan Koruthu <br>
Felipe Chapa Chamorro
