🤖 Python NLP Chatbot

A simple Natural Language Processing (NLP) chatbot built with Python using NLTK, TF-IDF Vectorization, and Cosine Similarity.

The chatbot takes a user's question, compares it with a predefined collection of sentences, and returns the most similar sentence as a response.

📌 Project Overview

This project demonstrates how basic NLP techniques can be used to create a text-based chatbot without using deep learning or external AI APIs.

The chatbot:

Accepts user input from the terminal
Tokenizes text using NLTK
Uses WordNetLemmatizer for basic text normalization
Converts sentences into numerical vectors using TF-IDF
Calculates similarity using Cosine Similarity
Returns the most similar sentence from the chatbot's corpus
Continues the conversation until the user types bye
🛠️ Technologies Used
🐍 Python
🧠 Natural Language Processing (NLP)
📚 NLTK
📊 Scikit-learn
🔢 TF-IDF Vectorizer
📐 Cosine Similarity
📓 Jupyter Notebook
📂 Project Structure
Python-NLP-Chatbot/
│
├── chatbot.ipynb
└── README.md
⚙️ How It Works
1. Download NLTK Resources

The project downloads the required NLTK resources:

nltk.download('punkt')
nltk.download('punkt_tab')
nltk.download('wordnet')

These resources are used for sentence tokenization and lemmatization.

2. Create the Corpus

The chatbot uses a small predefined corpus:

Hello! How can I help you?
What is your name?
I’m a chatbot built using Python.
Tell me a joke.
Python is a great programming language.
Goodbye!
3. Sentence Tokenization

The corpus is divided into individual sentences using:

sent_tokens = nltk.sent_tokenize(corpus)
4. Lemmatization

The project uses:

WordNetLemmatizer()

to convert words into their basic forms.

5. TF-IDF Vectorization

The chatbot converts sentences into numerical representations using:

TfidfVectorizer(
    stop_words="english",
    lowercase=True
)

TF-IDF helps identify important words within the sentences.

6. Cosine Similarity

The user's input is compared against the chatbot's existing sentences using:

cosine_similarity()

The sentence with the highest similarity is selected as the response.

💬 Example
ChatBot: Ask me anything! Type 'bye' to exit.

You: What is your name?
ChatBot: What is your name?

You: Tell me about Python
ChatBot: Python is a great programming language.

You: bye
ChatBot: Goodbye!
🚀 Installation
Step 1: Clone the Repository
git clone https://github.com/your-username/Python-NLP-Chatbot.git
Step 2: Open the Project
cd Python-NLP-Chatbot
Step 3: Install Required Libraries
pip install nltk scikit-learn
Step 4: Run the Notebook

Open:

chatbot.ipynb

using Jupyter Notebook or JupyterLab.

▶️ Running the Project

Run the notebook cells in order.

The chatbot will display:

ChatBot: Ask me anything! Type 'bye' to exit.

Enter your questions in the terminal.

To stop the chatbot:

bye
🧠 NLP Concepts Used
Concept	Purpose
Tokenization	Splits text into sentences/words
Lemmatization	Converts words to their base form
TF-IDF	Converts text into numerical vectors
Cosine Similarity	Measures similarity between text vectors
NLP	Enables the chatbot to process text
📊 Algorithm
User Input
     ↓
Sentence Tokenization
     ↓
Text Preprocessing
     ↓
TF-IDF Vectorization
     ↓
Cosine Similarity
     ↓
Find Most Similar Sentence
     ↓
Generate Response
🎯 Key Features
Simple and beginner-friendly NLP project
No external AI API required
Uses machine-learning-based text similarity
Interactive command-line chatbot
Easy to expand with additional training sentences
Demonstrates practical use of NLP concepts
🔮 Future Improvements

The chatbot can be improved by:

Adding a larger conversational dataset
Adding more intelligent responses
Creating a graphical user interface
Adding speech recognition
Adding text-to-speech functionality
Using machine-learning or deep-learning models
Connecting the chatbot to a web application
Adding conversation history
Improving intent detection
📚 Learning Outcomes

Through this project, you can learn:

Python NLP fundamentals
NLTK
Text preprocessing
Tokenization
Lemmatization
TF-IDF
Cosine similarity
Basic chatbot development
Interactive Python applications
👨‍💻 Author

Pesam Dinesh

Python | Data Analytics | Machine Learning | SQL | Power BI

⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub.

#Python #NLP #Chatbot #NLTK #MachineLearning #AI #PythonProjects #DataScience
