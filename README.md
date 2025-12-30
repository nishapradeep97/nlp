# nlp
🤖 NLP Chatbot using TF-IDF & Cosine Similarity

This project implements a simple NLP-based chatbot using Python, NLTK, and Scikit-learn.
The chatbot works on a retrieval-based approach, where it selects the most relevant response from a given text dataset using TF-IDF vectorization and cosine similarity.

 **Features**

Text preprocessing using NLTK

Tokenization (sentence & word level)

Lemmatization using WordNet

Greeting detection

TF-IDF based response generation

Cosine similarity for matching user queries

Interactive command-line conversation

****Technologies Used**
Python 3

NLTK

NumPy

Scikit-learn

Random

String

**Project Structure**
├── chatbot.py
├── chatbot.txt
├── README.md


chatbot.py → Main chatbot implementation

chatbot.txt → Knowledge base (text corpus)

README.md → Project documentation

⚙️ Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/your-username/nlp-chatbot.git
cd nlp-chatbot

2️⃣ Install required libraries
pip install numpy nltk scikit-learn

3️⃣ Download NLTK resources (first run only)
import nltk
nltk.download('punkt')
nltk.download('wordnet')
nltk.download('omw-1.4')

▶️ How to Run
python chatbot.py


You’ll see:

Chatbot: Hai! Let's have the conversation!
(Type 'bye' to exit)

**Example Conversation**
User: hello
Chatbot: hi there

User: what is data science?
Chatbot: data science is an interdisciplinary field that uses scientific methods...

User: bye
Chatbot: Good Bye and take care

**How It Works**

Reads and preprocesses text from chatbot.txt

Converts sentences into TF-IDF vectors

Uses cosine similarity to compare user input with dataset sentences

Returns the most relevant sentence as a response

Falls back to a default message if similarity is zero
