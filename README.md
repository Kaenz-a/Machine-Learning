# Machine-Learning
Credit scoring with Machine Learning 

install requirements.txt with "pip install -r requirements.txt"



First code part is where we train our models and evaulate our metrics. Brute force parameter search and Grid search parameter search are added as comments. They runned before and their results are also added as comments. 

X_train,y_train(%60 of original data), X_val,y_val(%20 of original data), X_test,y_test(%20 of original data), X_train_resampled,y_train_resampled(after smotenc, test and val data doesnt change), X_train_encoded,y_train_resampled(train set after one_hot encode), X_val_encoded, y_val(validation set after one_hot encode), X_test_encoded, y_test(test set after one_hot encode)

Random forrest: rf_model (model variable name), y_pred_rf_val(prediction for validation set), score_rf_val(f1 score for validation set), y_pred_rf(prediction for test set), score_rf(f1 score for test set)

XGBoost: xgb_model (model variable name), y_pred_xgb_val(prediction for validation set), score_xgb_val(f1 score for validation set), y_pred_xgb(prediction for test set), score_xgb(f1 score for test set)

Random forrest after Hyper Parameter: rf_model_hp (model variable name), y_pred_rf_hp_val(prediction for validation set), score_rf_hp_val(f1 score for validation set), y_pred_rf_hp(prediction for test set), score_rf_hp(f1 score for test set)



Second code part creates confisuon matrix and roc curves. If you want to generate them for different models change 'model' variable to desired model variable name.



Third code part is created for measuring error rates by changing 'Status' with a desired collumn name and by changing 'results_df' variable to desired prediction of any model error rates for that model and collumn can be seen



Forth and fifth code parts created for genereting 'Model F1 Score Comparison (Test Set)' and 'Most Important Features for Credit Risk' tables. 

At forth code by changing model_scores variable 'Model F1 Score Comparison (Test Set)' graph can be recreated.

At fifth code part by changing importances's variable model variable importances graph for that spesific model can be seen. It doesnt change for models that much We generated it for tuned Random forrest model.
