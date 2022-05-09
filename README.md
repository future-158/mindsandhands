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
- every feature's cardinality is too small. test ordinal encoding or one-hot-encoding, etc.
- hyper parameter optimization
- by plotting graph, target distribution shift seems not occured. need to check covarite shift. need to find train, test data comes from same distribution.
