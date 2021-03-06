# ML Project 2: CODE
This folder contains the Python files used to train the Logistic Regression classifier and make the predictions.
- `models`: folder containing the files created during the training. Specifically:
  - `clf_logreg.p`: pickle file containing the pre-trained Logistic Regression classifier, as described in `train.py` below.
  - `corpus_data_tfidf_fitted.p`: pickle file containing the TF-IDF transformer of the trained model.
  - `vocabulary.p`: pickle file containing the vocabulary generated by the TF counter.
- `other_helpers`: folder containing Python modules for pre-processing described in the report but not used by the best classifier.
- `results`: folder containing the `.csv` file generated by `run.py`.
  - `submission.csv`: predictions used for the top Kaggle submission. If you do not specify a different name in `run.py`, it will be overwritten when running the latter.
- `hash_replacers.py`: Python module that removes the pound sign (#) in front of words in a text.
- `helpers.py`: Python module containing functions used to load the data, pre-processing it and creating the `.csv` submission file.
- `run.py`: Python file to predict labels for a data file (default: `../data/test_data.txt`) using the models generated by `train.py` in the `modules/` folder. The file containing the predicted values is stored in the `results` folder.
- `train.py`: Python file to train the Logistic Regression classifier. It saves the vocabulary and the trained classifier in the `models` folder.

The description of the pre-processing performed during training and testing, and the hyperparameters used to obtain the top Kaggle submission are described in the README file in the parent directory.
