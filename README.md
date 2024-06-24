# Wine Review Text Classification

This project demonstrates a text classification task using TensorFlow and Keras. The goal is to classify wine reviews as high quality or low quality based on their descriptions.

## Dataset : - https://drive.google.com/drive/folders/1HWh7mA0xZP6DIbk39gKsGxrBn5P6R9UZ?usp=drive_link

The dataset used in this project is `wine-reviews.csv`, which contains the following columns:
- `country`: Country of origin
- `description`: Review text
- `points`: Wine rating
- `price`: Wine price
- `variety`: Grape variety
- `winery`: Winery name

## Project Structure

1. **Data Loading and Preprocessing**:
   - Load the dataset and clean it by dropping rows with missing values.
   - Create a binary label for wine quality based on the `points` column.
   - Split the dataset into training, validation, and test sets.

2. **Dataset Preparation**:
   - Convert the DataFrame into a TensorFlow dataset with shuffling, batching, and prefetching.

3. **Model 1: Using Pre-trained Embeddings**:
   - Use a pre-trained embedding layer from TensorFlow Hub.
   - Build a sequential model with dense layers and dropout layers.
   - Compile and train the model.

4. **Model 2: LSTM Network**:
   - Use a `TextVectorization` layer to tokenize and vectorize the text data.
   - Build an LSTM-based sequential model.
   - Compile and train the model.

