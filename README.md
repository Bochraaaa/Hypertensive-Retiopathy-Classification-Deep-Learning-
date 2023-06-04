# Project Description :  Hypertensive Rttinopathy Classification using TensorFlow, OpenCV, Matplotlib, Pandas, and NumPy-
The goal of this project is to develop a real-time disease  system using deep learning techniques. The project utilizes various libraries such as TensorFlow, OpenCV, Matplotlib, Pandas, and NumPy to achieve this objective.
The project workflow can be described as follows:
1. Data Preprocessing: The first step is to preprocess the input data. This includes scaling pixel values and normalizing the data to ensure compatibility with the MobileNetV3 model. The preprocessing module from the tensorflow.keras.layers.experimental package is used for this purpose.

2. MobileNetV3 Model: The pretrained MobileNetV3 architecture is employed for object classification. The last layer of the model is removed to enable transfer learning. By removing the last layer, the model can be fine-tuned to adapt to the specific task of object classification, in this case, RH (Hypertensive Retinopathy) classification.

3. Transfer Learning and Fine-tuning: The MobileNetV3 model is fine-tuned using transfer learning techniques. Transfer learning leverages the knowledge gained from pretraining on a large dataset to improve performance on a smaller, task-specific dataset. By adapting the pretrained model to the RH classification task, it can achieve better accuracy and performance.

4. Early Stopping: To prevent overfitting and optimize training, the project incorporates early stopping. If the model does not show improvement over 15 epochs, training is automatically stopped. Early stopping helps prevent excessive training and ensures that the model is not overly specialized to the training data.

5. Evaluation: The model's performance is evaluated using several metrics, including recall, precision, loss, and accuracy curves. These metrics provide insights into the model's ability to correctly classify RH objects. Additionally, four layers with the ReLU activation function are added to enhance the model's learning capabilities.

6. Training Epochs: The fine-tuned model is trained for a total of 29 epochs. Each epoch represents a complete pass through the training data, allowing the model to learn from the dataset in an iterative manner
