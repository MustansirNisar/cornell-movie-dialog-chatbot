
# Cornell Movie Dialog Chatbot

This project builds a chatbot using the Cornell Movie Dialogs Corpus. The implementation is done using Python and several libraries including PyTorch and TensorFlow. The chatbot is designed to learn from movie dialogues and generate responses to input sentences.

## Project Structure

- **Library Imports and Device Setup**
  - Importing necessary libraries and modules such as PyTorch, TensorFlow, CSV, JSON, and more.
  - Configuring the computation device (CPU/GPU).

- **Loading and Processing the Movie Dialog Corpus**
  - Reading and previewing the `movie_lines.txt` file to understand its structure.
  - Loading and processing the movie dialog corpus to create input-response pairs suitable for training.

- **Data Preprocessing**
  - Cleaning the text data by lowercasing and removing non-alphanumeric characters.
  - Tokenizing the text data and creating sequences of integers.
  - Padding sequences to ensure uniform length for input to the neural network.

- **Model Building**
  - Constructing an encoder-decoder model using TensorFlow's Keras API.
  - The encoder processes the input sequences while the decoder generates the output sequences.

- **Training the Model**
  - Splitting the data into subsets and saving them to disk.
  - Training the model on these subsets to handle large datasets efficiently.
  - Saving the trained model after each subset for checkpoints.

## Usage

1. **Setup Environment**: Ensure you have Python 3.10.11 installed along with the required libraries listed in the `requirements.txt`.

2. **Run Notebook**: Open and run `chatbot.ipynb` in a Jupyter Notebook environment. This will guide you through the steps of setting up the environment, loading data, preprocessing, building, and training the model.

3. **Training**: The training process is divided into subsets to manage large datasets. The model is trained for a specified number of epochs on each subset.

4. **Model Checkpoints**: After training on each subset, the model is saved. You can load these checkpoints to resume training or for inference.

## Requirements

- Python 3.10.11
- PyTorch
- TensorFlow
- NumPy
- Pandas
- Jupyter Notebook

## Acknowledgements

This project uses the Cornell Movie Dialogs Corpus, a dataset containing conversations from movie scripts. The dataset is publicly available and widely used for training conversational agents.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

Feel free to customize this README further based on any additional details or specific instructions you want to include.
