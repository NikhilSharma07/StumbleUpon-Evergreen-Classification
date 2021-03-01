# StumbleUpon-Evergreen-Classification

Approach of solving the problem
1. Imported the dataset using the pandas library.<br />
2. Checked whether the dataset is balanced or not. It was a balance both the
labels had almost equal instances.<br />
3. Checked in “boilerplate” it was having title and body. Separated both the
title and body using json.loads and dictionary and created two columns title
and body from them.<br />
4. Cleaning the text-<br />
➔ Convert the text to lowercase.<br />
➔ Removed the special characters using the regex module.<br />
➔ Converted the text into tokens.<br />
➔ Removed the stopwords present in the text using nltk.<br />
➔ Performed spelling correction of misspelled words.<br />
➔ Performed stemming of words using PorterStemmer.<br />
5. Combined the cleaned title and body column to form the boilerplate column
again.<br />
6. Saved the cleaned dataset to a csv file.<br />
7. Used the pretrained GloVe embedding ( glove.6B.300d.txt) to convert
words into vectors.<br />
8. Using Pytorch, trained the dataset using LSTMClassifier.<br />
9. Created a custom loss function to improve the precision and recall while
training the dataset.<br />
10.With all these steps I was able to achieve the following results.<br />
