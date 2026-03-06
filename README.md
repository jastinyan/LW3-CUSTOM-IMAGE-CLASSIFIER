<h1 align="center"> 🌿LW3-CUSTOM-IMAGE-CLASSIFIER 🌿</h1>


🔗 **Google Colab Notebook:**  
https://colab.research.google.com/drive/1YWnLDF9ygclu_GDrUVAHJSGvAb3CDQyY?usp=sharing

-----
🔗 **ImageDataset from Drive:**  
https://drive.google.com/drive/folders/10xbb-jQI_sNYi7EBiRx-2FXmAZw8jZB-?usp=sharing

## 📌 Laboratory Work 3 Activity — Building a Custom Image Classifier with TensorFlow Using Personal Image Datasets from Google Drive

-----

### Guide Questions (Student Reflection & Explanation)
Students must answer the following:

**1. Dataset Preparation**
   
- How did you organize your dataset in Google Drive?

  **I created a main folder called ImageDataset in Google Drive. Inside it, I made different folders for each plant species and placed the images of that plant inside its folder. The folder names represent the labels for each category.**
  
- Why is folder structure important for TensorFlow image loading?

  **The folder structure is important because TensorFlow uses the folder names as labels for the images. This helps the system automatically group the images into the correct categories during training.**
  
**2. Model Training**
   
- What is the role of convolutional layers in image classification?

  **Convolutional layers help the model find important features in an image, like edges, shapes, and textures. These features help the model recognize and classify different images.**
  
- Why do we split data into training and validation sets?

  **We split the data so the model can learn from one set and be tested on another set for validation. This helps check if the model works well on new data.**
  
**3. Performance Analysis**

- What accuracy did your model achieve?

  **The model achieved a validation accuracy of about 70.76% after training for 10 epochs. This means the model was able to correctly classify around 70% of the images in the validation dataset.**
  
- How did the number of images affect the model’s performance?

  **Having many images helped the model learn the features of different plants better. With more training data, the model was able to improve its accuracy, although some errors still occurred when predicting new images.**
  
**4. Critical Thinking**

- What challenges did you encounter while using your own dataset?

  **One challenge was collecting enough images for each plant category. It also took time to organize the images properly and make sure they were in the correct folders.**
  
- How can data augmentation improve your model?

  **Data augmentation improves the model by creating different versions of the same images, like rotating or flipping them. This gives the model more data to learn from.**
  
**5. Application**
   
- Suggest a real-world application for your trained model.
- How can this system be integrated into a mobile or web application?

  **A real-world use of this model is a plant identification app. People can take a photo of a plant, and the system will identify the plant species automatically.**

-----

## 📌 Activity 3A: Improving and Evaluating a Custom Image Classifier

------
### Guide Questions (Student Explanation & Reflection)

**Visualization & Overfitting**

1. What signs indicated overfitting in your first model?

   **The first model showed overfitting because the training accuracy became very high while the validation accuracy stayed lower. This means the model learned the training data too well but did not perform as well on new data.**
   
2. How did data augmentation affect validation accuracy?

   **Data augmentation improved the validation accuracy by giving the model more variations of the images. This helped the model learn better and perform better on unseen images.**
   
**Model Improvement**

3. What is the purpose of dropout layers?

   **Dropout layers help reduce overfitting by randomly turning off some neurons during training. This forces the model to learn more general patterns instead of memorizing the training data.**
   
4. Why does data augmentation improve generalization?

   **Data augmentation improves generalization by creating different versions of the images, such as flipped or rotated images. This increases the variety of training data and helps the model recognize objects in different conditions.**
   
**Performance Comparison**

5. Compare accuracy before and after improvements.

   **Before the improvements, the model had high training accuracy but lower validation accuracy. After adding data augmentation and dropout, the validation accuracy improved and the gap between training and validation accuracy became smaller.**
   
6. Which technique contributed most to improvement?

   **Data augmentation contributed the most to improvement because it increased the variety of images used for training, which helped the model learn better features.**

**Deployment & Application**

7. Why is saving the model important?

   **Saving the model is important because it allows us to reuse the trained model later without training it again. It can also be used for deployment in applications.**
   
8. How can this model be deployed in a real-world system?

    **This model can be deployed in a mobile or web application where users upload or capture images. The system will then use the trained model to identify and classify the image automatically.**
