# Face Expression Detection

## Project Structure
The hands on project on Facial Expression Recognition is divided into following tasks:
	
	Task 1: Generate Training and Validation Batches
		- Generate batches of tensor image data with real-time data augmentation.
		- Specify paths to training and validation image directories and generates batches of augmented data.
	
	Task 2: Create a Convolutional Neural Network (CNN) Model
		- Design a convolutional neural network with 4 convolution layers and 2 fully connected layers to predict 7 types of facial expressions.
		- Use Adam as the optimizer, categorical crossentropy as the loss function, and accuracy as the evaluation metric.
	
	Task 3: Train and Evaluate Model
		- Train the CNN by invoking the model.fit() method.
		- Use ModelCheckpoint() to save the weights associated with the higher validation accuracy.
		- Observe live training loss and accuracy plots in Jupyter Notebook for Keras.
	
	Task 4: Save and Serialize Model as JSON String
		- Sometimes, you are only interested in the architecture of the model, and you don't need to save the weight values or the optimizer.
		- Use to_json(), which uses a JSON string, to store the model architecture.
	
	Task 5: Create a Flask App to Serve Predictions

	Task 6: Create a Class to Output Model Predictions
		- Create a FacialExpressionModel class to load the model from the JSON file, load the trained weights into the model, and predict facial expressions.
	
	Task 7: Design an HTML Template for the Flask App
		- Design a basic template in HTML to create the layout for the Flask app.

	Task 8: Use Model to Recognize Facial Expressions in Videos
		- Run the main.py script to create the Flask app and serve the model's predictions to a web interface.
		- Apply the model to saved videos.