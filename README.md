# Book_Recommendation_System
This is a book recommendation system using the KNN algorithm. It takes the user's input and recommends books based on the user's input. It has been trained on a dataset of more than 10,000 books.

## Data Preprocessing
The data is preprocessed to remove null values and to convert the data into a suitable format for the KNN algorithm.

## Model Building
The KNN algorithm is used to build the model.

## Architecture
The recommendation system is built using a neural network architecture defined by the `BookRecommenderNet` class. The architecture consists of an encoder-decoder structure:
- **Encoder**: 
  - Input layer with size equal to the number of features.
  - Two hidden layers with 128 and 64 neurons, respectively, using the ReLU activation function.
  - Output layer with 32 neurons, which represents the encoded book embeddings.
  
- **Decoder**: 
  - Input layer with 32 neurons.
  - Two hidden layers with 64 and 128 neurons, respectively, also using the ReLU activation function.
  - Output layer that reconstructs the input features.

## Loss Function
The model uses Mean Squared Error (MSE) as the loss function during training. This function measures the average squared difference between the predicted and actual values, which helps in minimizing the reconstruction error of the input features.

## Activation Function
The ReLU (Rectified Linear Unit) activation function is used in the hidden layers of both the encoder and decoder. ReLU is defined as \( f(x) = \max(0, x) \), which introduces non-linearity into the model and helps in learning complex patterns in the data.

## Conclusion
The KNN algorithm, combined with a well-structured neural network architecture, provides a robust solution for the book recommendation system. The model's ability to learn complex patterns and deliver accurate recommendations enhances the user experience, making it a valuable tool for book enthusiasts seeking personalized suggestions.
