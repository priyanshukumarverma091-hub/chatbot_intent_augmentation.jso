# Student Helpdesk Chatbot

A machine-learning chatbot that helps students with common college-related questions, including attendance, exams, results, scholarships, hostel facilities, library services, Wi-Fi, and placements.

The project uses **TF-IDF** text vectorization and **Logistic Regression** to identify the intent behind a user's message. It supports English and Hinglish-style queries from the included training data.

## Features

- Classifies student questions into predefined intents
- Shows the predicted intent and confidence score
- Includes training and test examples
- Saves the trained model and supporting files for reuse

## Technologies Used

- Python
- scikit-learn
- NumPy
- Matplotlib
- Joblib
- Google Colab

## Project Files

- `chatbot_v2.ipynb` — training, evaluation, and chatbot testing notebook
- `chatbot_intent_augmentation.json` — dataset containing training text and intent labels
- `chatbot_v2_model.pkl` — saved trained model
- `chatbot_v2_vectorizer.pkl` — saved TF-IDF vectorizer
- `chatbot_v2_label_encoder.pkl` — saved label encoder
- `chatbot_v2_intents.pkl` — saved intent data

## How to Run

1. Download or clone this repository.
2. Open `chatbot_v2.ipynb` in Google Colab or Jupyter Notebook.
3. Install the required packages:

   ```bash
   pip install scikit-learn numpy matplotlib joblib
   ```

4. Upload `chatbot_intent_augmentation.json` when the notebook asks for it.
5. Run the notebook cells in order to train, test, and save the chatbot.

## How It Works

1. The dataset is loaded from a JSON file.
2. User text is converted into numerical features using TF-IDF.
3. A Logistic Regression model is trained to predict intent labels.
4. The chatbot predicts an intent for a new message and returns a matching response from the data.

## Note

The current notebook uses example training sentences as responses. For more useful replies, add a dedicated response field for every intent in the dataset.

## Future Improvements

- Add curated answers for each intent
- Build a web interface with Streamlit or Flask
- Support more languages
- Improve the dataset with additional queries and intents
# chatbot_intent_augmentation.jso
ML-based student helpdesk chatbot that classifies queries about attendance, exams, results, scholarships, hostel, library, Wi‑Fi, and placements using TF-IDF and Logistic Regression.
