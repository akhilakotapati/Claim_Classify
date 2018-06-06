# Claim_Classify
Initially, the dataset consists of 481 data items. After removing rows that are missing art unit information, we are left with 445 data items. This is an unbalanced data set where there are very few data items that belongs to "True" class. There are two ways to handle this issue, one is upsampling and the other is downsampling. Downsampling makes the data very small, so I have used upsampling and made the data almost balanced.
On the new sampled data set, I have implemented "Count Vectorizer", "Tf-Idf" on three columns namely "All Claims", "Abstract", "Title". I have taken Logistic Regression as my baseline algorithm. And then implemented SVM.
Initially, when I have implemented SVM on the original dataset, the accuracy was around 94%. However, it failed to get the best result when I ran grid-search. The results were between 49% - 61%. Later, when the algorithms were implemented using upsampled dataset, the results for both Logistic Regression and SVM were around 96%. 
