# Predictive-Modeling-Using-Machine-Learning

DESCRIPTION 

Step 1: Import Required Libraries
The program imports the necessary Python libraries:
pandas – Used for data handling and manipulation.
matplotlib.pyplot – Used to create graphs and visualizations.
load_iris – Loads the Iris dataset.
train_test_split – Splits the dataset into training and testing sets.
RandomForestClassifier – Machine learning algorithm used for classification.
accuracy_score – Calculates the model's prediction accuracy.
confusion_matrix and ConfusionMatrixDisplay – Generate and display the confusion matrix.

Step 2: Load the Dataset
The Iris dataset is loaded using load_iris(). It contains:
150 flower samples
4 input features:
Sepal Length
Sepal Width
Petal Length
Petal Width
3 output classes:
Setosa
Versicolor
Virginica

Step 3: Split the Dataset
The dataset is divided into:
80% Training Data – Used to train the model.
20% Testing Data – Used to evaluate the model.
This ensures that the model is tested on unseen data.

Step 4: Train the Model
A Random Forest Classifier is created and trained using the training dataset.
Python
model = RandomForestClassifier(random_state=42)
model.fit(X_train, y_train)
The model learns patterns from the training data to classify flower species.

Step 5: Make Predictions
The trained model predicts the flower species for the testing dataset.
Python
y_pred = model.predict(X_test)

Step 6: Calculate Accuracy
The accuracy score measures how many predictions are correct.
Python
accuracy = accuracy_score(y_test, y_pred)
Sample Output:

Accuracy: 100%

Step 7: Generate the Confusion Matrix
The confusion matrix compares the actual labels with the predicted labels.
Python
cm = confusion_matrix(y_test, y_pred)
It helps identify:
Correct predictions
Incorrect predictions
Classification performance for each class

Step 8: Display the Graph
The confusion matrix is displayed as a heatmap using Matplotlib.
Python
disp.plot(cmap='Blues')
plt.title("Confusion Matrix")
plt.show()

OUTPUT 📌

<img width="1536" height="1024" alt="Image" src="https://github.com/user-attachments/assets/bc6c37be-8237-4526-8b94-aeb455c81cde" />
