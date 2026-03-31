LW3                                                                                                                              03-04-2026

📊 Model Training, Visualization, and Improvement
🔗 Colab Notebook

You can view and run the full implementation here:
👉 Colab Link: [https://colab.research.google.com/drive/1leUAOiqRhOGnN6SpJtY3vx6aAUGOMcw0](https://colab.research.google.com/drive/1aVdLRRzG6Olx0XuMG3mQb9Sv-i3RoJcN?usp=sharing)

https://colab.research.google.com/drive/1aVdLRRzG6Olx0XuMG3mQb9Sv-i3RoJcN?usp=sharing

https://colab.research.google.com/drive/1aVdLRRzG6Olx0XuMG3mQb9Sv-i3RoJcN?usp=sharing


🔹 1. Dataset Preparation

Q: How did you organize your dataset in Google Drive?
I organized my dataset by creating one main folder named ImageDataset, and inside it, I created separate folders for each plant category. Each folder contains images belonging to one class only.

Q: Why is folder structure important for TensorFlow image loading?
Folder structure is important because TensorFlow automatically uses the folder names as labels. This makes it easier to classify images correctly without manually labeling each image.

🔹 2. Model Training

Q: What is the role of convolutional layers in image classification?
Convolutional layers help detect important features in images such as edges, shapes, and textures. These features are used by the model to identify and classify images correctly.

Q: Why do we split data into training and validation sets?
We split the data to train the model using the training set and evaluate its performance using the validation set. This helps check if the model is learning properly or just memorizing the data.

🔹 3. Performance Analysis

Q: What accuracy did your model achieve?
The model achieved an accuracy of approximately (e.g., 85%–95%), depending on the dataset quality and training process.

<img width="767" height="343" alt="image" src="https://github.com/user-attachments/assets/af657b57-2ff6-4d4e-8c01-77d50d005ca9" />


Q: How did the number of images affect the model’s performance?
A larger number of images improved the model’s performance because it provided more examples for learning. Small datasets may lead to poor accuracy or overfitting.

🔹 4. Critical Thinking

Q: What challenges did you encounter while using your own dataset?
Some challenges include:

Slow training due to large number of images
Inconsistent image quality
Limited variety in some classes
Incorrect or noisy data

Q: How can data augmentation improve your model?
Data augmentation creates modified versions of images (like flipping, rotating, zooming), which increases dataset diversity and helps the model generalize better.

🔹 5. Application

Q: Suggest a real-world application for your trained model.
This model can be used in a plant identification app where users take a photo of a plant and the system identifies its species.

Q: How can this system be integrated into a mobile or web application?
The trained model can be deployed using an API and connected to a mobile or web app where users upload images and receive predictions in real time.


🧠 Guide Questions
Student Explanation & Reflection
📉 Visualization & Overfitting
1. What signs indicated overfitting in your first model?

Overfitting was observed when the training accuracy continued to increase while the validation accuracy stopped improving or started decreasing. Additionally, the training loss became very low, but the validation loss increased, indicating that the model was learning the training data too well and failing to generalize to new data.

2. How did data augmentation affect validation accuracy?

Data augmentation helped improve validation accuracy by increasing data diversity. By applying transformations such as rotation, flipping, and zooming, the model was exposed to varied versions of the same images, reducing overfitting and improving its ability to generalize to unseen data.

🛠️ Model Improvement
3. What is the purpose of dropout layers?

Dropout layers are used to prevent overfitting by randomly disabling a portion of neurons during training. This forces the model to learn more robust features and prevents it from relying too heavily on specific neurons.

4. Why does data augmentation improve generalization?

Data augmentation improves generalization by simulating real-world variations in the dataset. This helps the model learn invariant features and perform better on new, unseen data rather than memorizing the training set.

📈 Performance Comparison
5. Compare accuracy before and after improvements.

Before applying improvements such as data augmentation and dropout, the model showed high training accuracy but lower validation accuracy. After the improvements, validation accuracy increased and became more stable, indicating better generalization performance.

6. Which technique contributed most to improvement?

Data augmentation contributed the most to the improvement because it effectively increased the dataset size and variability, helping the model learn more generalized features.

🚀 Deployment & Application
7. Why is saving the model important?

Saving the model allows it to be reused without retraining. This is essential for deployment, testing, and future improvements, saving both time and computational resources.

8. How can this model be deployed in a real-world system?

The model can be deployed in real-world applications such as web or mobile apps by integrating it into a backend server or converting it into formats compatible with deployment platforms. It can be used for tasks like image classification, automated detection systems, or decision-support applications.
