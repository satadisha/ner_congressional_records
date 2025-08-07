***graphs.ipynb*** builds upon Gabriel's Label Distribution graphs to improve visuals. 

***RandomForestClassifier-Flags.ipynb*** creates a Random Forest model using flags created from the full_name column for word count, common PAC words, and common organization words. Will be improved later with a vocabulary list created with the most common words from the training corpus.

***RandomForestClassifier-TFIDF.ipynb*** creates a Random Forest model using TF-IDF on the full_name column

***SupportVectorClassifier.ipynb*** creates a Support Vector Machine model using TF-IDF on the full_name column

***unlabeled.ipynb*** used to look at and compare the predictions on unlabeled michigan data


We noticed some problems with the TF-IDF vectorizer:
- it is ignoring single characters (ex. middle initials) which could be important
- Also it seems to ignore org endings (ex. inc., llc, etc.) which we suspect to be very clear organization identifiers
