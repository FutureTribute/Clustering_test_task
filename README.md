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

Images from dataset:
![image](https://user-images.githubusercontent.com/25502260/126874034-f1b86d95-966c-452d-9e12-61a7a8cc1fc5.png)

Images by clusters:
![image](https://user-images.githubusercontent.com/25502260/126874105-3accc6e7-2272-45d8-b98a-7a8b7fedc1b9.png)

Metrics:
* ```RandIndex: 0.7655172413793103```
* ```Adj RandIndex: 0.06773963104593016```
