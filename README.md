# WeRateDogs-data-analysis-project

## Objective
Leverage WeRateDogs Twitter data to create engaging and reliable analytics and visualizations.

## Files description
Here is the description of the project's main files.
- ‘twitter-archive-enhanced.csv’: Twitter WeRateDogs archive.
- ‘tweet_json.txt’: Twitter WeRateDogs additional data collected using Twitter API.
- ‘image_predictions.tsv’: dogs images predictions.
- ‘act_report.ipynb’: a jupyter notebook, contains all the necessary code to be executed.

## About the dataset

### Twitter inhanced archives
The WeRateDogs Twitter Archive contains basic data on the 5,000+ tweets, but not all. One column in the archive however contains: the text of each tweet, which I used to extract the rating, the dog's name and the dog's 'steps' (i.e. doggo, floofer, pupper and puppo) to make this Twitter archive "enhanced". Of the 5,000+ tweets, I filtered tweets with ratings only (there are 2356).

### Additional data collected via API
This additional data contains information about the number of retweets en favorites for each WeRateDogs tweet in the enhanced archive.

### Image predictions
A neural network predicted images of  WeRateDogs classified by race. Here are the columns description:
- tweet_id is the last part of the tweet URL after "status/" → https://twitter.com/dog_rates/status/889531135344209921
- p1 is the algorithm's number 1 prediction for the image in the tweet → golden retriever
- p1_conf indicates the degree of confidence of the algorithm in its prediction number 1 → 95%
- p1_dog indicates if prediction number 1 is a purebred dog or not → TRUE
- p2 is the algorithm's second most likely prediction → Labrador retriever
- p2_conf indicates the degree of confidence of the algorithm in its prediction number 2 → 1%
- p2_dog indicates if prediction number 2 is a purebred dog or not → TRUE

## Guidelines to use the script:
### Requirments
- anaconda distribution
### usage
- download the project.
- run conda and go to the project directory
- run the following command
```
$ jupyter notebook
```
