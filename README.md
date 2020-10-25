# Weather Classification
Lab 4 assignment of Image Processing course, November 2019.

Team member:
- Gagah Pangeran Rosfatiputra
- Muhamad Achir Suci Ramadhan
- Sage Muhammad Abdullah

In this assignment, we were asked to create a classifier that classify the images into three classes: Clear, Haze, and Underwater.

We were doing this task using four approaches:
1. **Hand-crafted features**. We extract the color features (R, G, B, Saturation) and the textures (Contrast, Angular Second Moment, Homogeneity) of the images, and classify the images based on the features using Support Vector Machine.
2. **PCA**. We directly extract the PCA of the images and classify it using Support Vector Machine. However, we are prohibited to use any PCA library.
3. **Hand-crafted features + PCA**. We extract the PCA of the extracted features that is mentioned in approach (1) and use SVM to classify the images based on its PCA.
4. **Neural Network**. We use CNN to classify the images.

To overcome the small dataset problem, we did some image augmentation by resizing, adding random noise, rescaling intensity, adjusting gamma, and blurring the image using gaussian filters.

## Notes
- Unfortunately, I am not sure to share the datasets here because I have not asked my professor for permission.
- The datasets is very small. Only 30 images for the training set (10 for each class) and 15 images for the test set (5 for each class).
- After the image augmentation, the training set is expanded to 180 images.
- The classification result seems suspicious, too good to be true. However, it actually makes sense since the dataset is pretty small and the distinction between classes is very clear.
- There were several mistakes in the Neural Network part when we did and submitted this assignment. However, it is already fixed.
