---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Flare Detector for Reddit Data"
summary: "Project done as a task for MIDAS Lab to design end-to-end pipeline to predict submission flares for Indian subreddit. Extracts data, analyses it, builds a model, develops a web application and deploys it in Heroku"
authors:
- admin
tags:
- machine learning
- flare detection
- reddit
categories: []
date: 2020-05-01T00:00:00Z 
# 2020-10-27T16:55:14+05:30

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: "https://github.com/ShreyaGupta08/Flare-Detector-for-Reddit-Data"
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---


Flair detector is a web application, deployed using Heroku. The application can be seen [here](https://flair-detector-for-reddit.herokuapp.com). It scrapes posts using the URL and then uses a Random Forest model to predict the flair of the post.

The project contains the code which performs the following functionalities:
1. Scrapping posts from Indian Subreddit according to two methods: hottest posts and distributed posts in accordance with flairs
2. Exploratory Data Analysis: contains bar graphs and pie-charts to analyse data distributions for the attributes collected in step 1.
3. Textual Pre-Processing: pre-processes textual data for attributes like Title of the post and Content of the posts.
4. Building and contrasting different models: Builds, trains and validates four ML models, Naive Bayes, Random Forest, Logistic Regression and Multi-layer Perceptron using different features and then selects the feature-model pair performing the best.
5. Building Web Application: Contains the code to build a basic web application that takes as input a post url and displays the predicted flair of the post.
6. Hosts the app on Heroku.

My experimental log on how I designed the project along with the project code and documentation on how to run it in your local machine can be found [here](https://github.com/ShreyaGupta08/Flare-Detector-for-Reddit-Data)

### Good things about the project:
- Detailed Documentation
- Prediction for Photography posts (generally)

### Scopes of improvement:
- Prediction. I realised it a little late that the 71% accuracy in using title as feature (and Random Forest as learning algorithm) is achieved because the title contained the flair in most cases. This was weird and has been mentioned in better detail in the Experimental log.ipynb file. Time remaining, I would have liked to find a way to:
    - incorporate comments, content and title with the title (and dealing with NaNs appropriately)
    - Used better learning algorithms
    - collected more data.

### Future work:

In data exploration:
- finding the number of posts in each flair for which content != None
    - finding the correlation between individual flair confusion matrix obtained from using content only with the number of samples obtained above 
    - verifying if the unequal distribution is one of the reasons behind the low flair accuracy. if yes, checking if increasing the number of sample distribution had any effect on prediction scores. Then maybe, content would not have been as useless after all. 
    
- contrasting performance with unsupervised algorithms (like K-Means)
- Find flair-wise accuracy