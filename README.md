# product-category-classification

This project is about classifying the category of item names on e-commerce platform.

## Dataset
● result_online.csv: This file includes processed item id, item names and item_category concatenated with item_category2.

## Workflow
1. Balance item categories by dowsampling or upsampling each category.
2. Word segmentation using jieba.
3. Extract the features of item names with TFIDF vectorizor.
4. Dimenionality reduction. Only using the 100 best features per category.
5. Train test split (0.8 for training, 0.2 for testing).
6. Train XGBClassifier.
7. Evaluate the model with offline data.
