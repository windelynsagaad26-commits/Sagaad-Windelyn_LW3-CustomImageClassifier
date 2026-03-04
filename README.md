LW3                                                                                                                              03-04-2026

📊 Model Training, Visualization, and Improvement
🔗 Colab Notebook

You can view and run the full implementation here:
👉 Colab Link: https://colab.research.google.com/drive/1leUAOiqRhOGnN6SpJtY3vx6aAUGOMcw0

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
