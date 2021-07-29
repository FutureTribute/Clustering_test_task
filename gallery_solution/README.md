# Clusterisation_test_task

Data: mostly photos from my phone gallery, but some photos from public resources

As the task was to cluster some images, labels provided in the dataset are completely ignored.

Since the task is based around mobile phone gallery, using MobileNet seems like a best solution because of its good performance and, most importantly, its size. 

This solution might suffer from different problems because there isn't much data as I almost don't use my phone camera. 

Idea behind the solution is next:
1. Using pretrained network, apply transfer learning to it for more relevant outcomes;
2. Using network from step 1, extract features from images;
3. Perform KMeans with different values of n_clusters to assign clusters to images;
4. Select best model from step 4 based on silhouette_score and visualize results.

Images from dataset:
![image](https://user-images.githubusercontent.com/25502260/126874034-f1b86d95-966c-452d-9e12-61a7a8cc1fc5.png)

Images by clusters:
![image](https://user-images.githubusercontent.com/25502260/126874105-3accc6e7-2272-45d8-b98a-7a8b7fedc1b9.png)

Metrics:
* ```RandIndex: 0.7655172413793103```
* ```Adj RandIndex: 0.06773963104593016```
