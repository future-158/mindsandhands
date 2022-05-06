# assumption
you can groupby train_set by some manner( *may need domain knowledge. not sure*)
make different model in each group would make better result overall


# steps
- use umap embedding
- labeling train data using dbscan
- labeling test data using knn
- foreach group:
  - fit X_train_in_group, y_train_in_group
  - predict X_test_in_group

# needed experiments
- standard scaler
- one-hot-encoding X_3
- hyper parameter optimization
