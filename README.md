# Telecom_customer_churn

**Data Preprocessing:**

I loaded data from a CSV file.
Dropped the 'customerID' column as it's not relevant.
Converted the 'TotalCharges' column to a numeric type.
Removed rows with spaces in 'TotalCharges'.
Handled columns with 'No internet service' or 'No phone service' by replacing them with 'No'.
Converted categorical columns with 'Yes' and 'No' values to 1 and 0.
Performed one-hot encoding for categorical columns with multiple categories.
Scaled numerical features using Min-Max scaling.

**Data Visualization:**

Created histograms to visualize the distribution of tenure and monthly charges for both churned and non-churned customers.

**Model Building:**
- Created a Sequential model with three layers in Keras.
- Compiled the model with binary cross-entropy loss and the Adam optimizer.
- Trained the model on the training data for 100 epochs.
- Training process is ongoing, and shared the first 71 epochs. The model is optimizing its weights to minimize the binary cross-entropy loss, and the accuracy is gradually improving.

After training, we can evaluate the model on our test data to assess its performance and further fine-tune it if necessary. Additionally, we may want to monitor metrics like precision, recall, and F1-score, as mentioned at the beginning, to evaluate the model's ability to predict customer churn effectively.
