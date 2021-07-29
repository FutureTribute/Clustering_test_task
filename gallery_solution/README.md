# Clusterisation_test_task

Data: mostly photos from my phone gallery, but some photos from public resources

As the task was to cluster some images, labels provided in the dataset are completely ignored when performing KMeans.

Since the task is based around mobile phone gallery, using MobileNet seems like a best solution because of its good performance and, most importantly, its size. 

This solution might suffer from different problems because there isn't much data as I almost don't use my phone camera. 

Idea behind the solution is next:
1. Using pretrained network, apply transfer learning to it for more relevant outcomes;
2. Using network from step 1, extract features from images;
3. Perform KMeans with different values of n_clusters to assign clusters to images;
4. Select best model from step 4 based on silhouette_score and visualize results.

Training performance:
![image](https://user-images.githubusercontent.com/25502260/127489271-bdec53e7-f18e-45b9-9e01-09f973904d0d.png)

Images by clusters:
![image](https://user-images.githubusercontent.com/25502260/127489138-6b4171eb-7e2f-4b87-b83b-10e5b2e44cac.png)

