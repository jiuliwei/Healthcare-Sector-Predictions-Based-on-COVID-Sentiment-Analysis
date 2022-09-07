# Healthcare-Sector-Predictions-Based-on-COVID-Sentiment-Analysis
The Project of Predictive Analytics 2022 Summer

## How to run:

Run the **Main.ipynb** file using [**jupyter notebook**](https://jupyter.org/install#jupyter-notebook).

## Packages:

Make sure you have install **yfinance**, **pandas**, **numpy**, **seaborn**, **matplotlib.pyplot**, **sklearn** and **lightgbm** packages before run the code.

## The main code:

- **Main.ipynb**: The main code of this project. It will import the Yahoo finance data(import by API), import the Twitter data(output_percent.csv) and merge them into merged data. Preprocessing every dataset, predict with different Machine Learning models and generate the prediction result(accuracy, precision, recall and f1-score).


## Twitter Data Preprocessing:

- **Raw Twitter Data**: This file is too large (5GB+), we only contain the preprocessed dataset(**output_precent.csv**). You can download it by this [**link**](https://www.openicpsr.org/openicpsr/project/120321/version/V12/view?path=/openicpsr/120321/fcr:versions/V12/Twitter-COVID-dataset---June2022/tweetid_userid_keyword_sentiments_emotions_United-States.zip&type=file).

- **TwitterDataPrepare.ipynb**: Input is the Raw Twitter data. Merge the same day data into one row, delete the weekend(no weekend stock price) and convert the number of sentiment into percentage. Because the Raw Twitter Data is too large(5GB+) and we have preprocessed it, you do not need to run this file. If you want to run it, please download the Raw Twitter Data by the link above.

- **output.csv**: The result of merging the same day raw Twitter data into one row.

- **output_without_weekend.csv**: The result of deleting the weekend(no weekend stock price).

- **output_percent.csv**: The result of converting the number of sentiment into percentage. We use this data as the preprocessed twitter data in Main.ipynb file.