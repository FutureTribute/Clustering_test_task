# Clusterisation_test_task

Dataset: https://www.kaggle.com/olgabelitskaya/flower-color-images

As  task was to cluster some images, labels provided in the dataset are completely ignored.
Some photos were manually picked for future evaluation based on Adjusted RandIndex.

Idea behind the solution is next:
1. Using pretrained network, extract features from images;
2. Apply PCA to reduce numbers of features;
3. Perform KMeans to assign clusters to images;
4. Apply steps 1-2 to test data, predict clusters, based on results from step 3;
5. Compare results from step 4 to manual results.
