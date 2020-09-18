# Offensive-Comments

# Run script
First, install required libraries:

`pip install nltk keras tqdm scikit-learn`

Download embeddings. I used fastText crawl-300d-2M.vec. It can be found here: https://github.com/facebookresearch/fastText/blob/master/docs/english-vectors.md

Download Kaggle data. It can be found here: https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/data

Don't forget to extract files from archives.

Next, run:

`python fit_predict.py train.csv test.csv crawl-300d-2M.vec`

You will need some time to train a model. It takes ~3-4 hours on GTX 1080 Ti. In the end, there will be a file called `predict_results/submit` containing the scores for each column.
