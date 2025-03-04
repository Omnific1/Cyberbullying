# Cyberbullying
AI-Powered Cyberbullying Detection with a unique reputation scoring mechanism
Cyberbullying isn’t just an abstract concept; it’s a harsh reality for millions of individuals. Picture a young student dreading to open their social media app, unsure of what hateful comment might await them. Or a parent, watching helplessly as their child struggles with the emotional toll of online harassment. These moments drive home the urgency to act.


CyberShield is an **AI-driven platform** designed to detect and prevent cyberbullying on **social media platforms**. Using **Natural Language Processing (NLP)** and **Machine Learning (LSTM networks)**, it identifies offensive content, classifies it, and enforces **real-time reputation scoring** to curb online harassment.  

## 🚀 Features  
✅ **Text, Image & Voice-Based Detection** – AI scans comments, images, and voice recordings for harmful content.  
✅ **Automated Reputation System** – Offenders get a **reduced reputation score**, discouraging toxic behavior.  
✅ **Real-Time Moderation** – Offensive content is flagged instantly to maintain a safe online environment.  
✅ **User-Friendly Dashboard** – Monitor flagged posts and user reputation with an intuitive interface.  
✅ **Multi-Language Support** – Detects harmful content in **English, Hindi, and Kannada**.  

## 🛠 Technologies Used  
- **Frontend:** HTML, CSS, JavaScript  
- **Backend:** Flask, Python  
- **Machine Learning:** LSTM, NLP, TensorFlow  
- **Database:** Firebase / MySQL  
- **APIs & Services:** Google Translate, OpenAI NLP Models  



Main Design
Data Storage with BigQuery: (GCP)
We store the dataset of online messages in Google BigQuery, which allows for efficient querying and storage of large-scale datasets.

Pretrained Word Embeddings:
The model uses pretrained word embeddings such as GloVe or Word2Vec to convert words into vectors that capture semantic meaning. This helps the model understand the relationships between different words, which is critical for detecting nuances in language.

LSTM Model:
The model leverages LSTM (Long Short-Term Memory) networks, which are ideal for sequential data such as text. LSTMs are capable of retaining context over long sequences of words, making them perfect for text classification tasks.

Data Augmentation with Vertex AI & Gemini 2 Flash:
To avoid overfitting and improve the model’s performance, we use Vertex AI along with Gemini 2 Flash for data augmentation. This allows us to synthetically generate additional data from the existing dataset, thus improving the model’s ability to generalize to unseen data.

Deployment:
Once the model is trained, it can be deployed to Google Cloud, ensuring scalability and real-time predictions.

Architecture Overview
Input Layer: Collects user-generated content from platforms like social media or forums.
Processing Layer: Analyzes sentiment and flags abusive language using Vertex AI’s NLP models.
Output Layer: Notifies moderators or takes automated action to neutralize threats.
Prerequisites
To get started, ensure you have the following:

Software & Tools:

A Google Cloud account.
Vertex AI API enabled.
Python SDK for Google Cloud (google-cloud-aiplatform).
Knowledge Requirements:

Basic Python programming language.
Familiarity with machine learning basics.
Understanding of basic natural language processing concepts.
Step-by-step Instructions
Step 1: Enable BigQuery API:

Upload Data to BigQuery:

Prepare your dataset (a collection of online messages with labels indicating whether they are bullying or not).
Upload this dataset to BigQuery using Python:

Create a new project and enable the Vertex AI API.
Configure your service account with the necessary permissions.
(if needed) Connect the cloud to external IDE like jupyter, VScode etc.,
Steps which can be used to create and initalise API
for the billing make use of the free credits which can be availed in the login page

Step 2: Leverage Pre-trained Models

Select the Text-Bison model for NLP tasks.
Can use Glovebox for pretrained dataset for running with LSTM.
Fine-tune the model with labeled datasets including:
Examples of explicit bullying language.
Subtle or indirect harassment examples.
Neutral or benign conversations for comparison.
Build an LSTM model

Step 3: Deploy and Integrate

Deploy the fine-tuned model to a Vertex AI endpoint. (Look for the documentation)
Integrate the endpoint with your platform or application.
Use real-time inference to analyze content and flag harmful messages.
Step 4: Monitor and Optimize
Use Vertex AI’s built-in tools to monitor model performance.
Continuously update the training data to improve accuracy and adapt to emerging trends.
Architecture of the project

Result / Demo
By following these steps, you’ll achieve:

A fully deployed AI model capable of detecting and addressing cyberbullying.
Integrated real-time monitoring within your application.
Improved user safety and healthier online interactions.
What’s Next?
Expand your project by:

Implementing multi-language support to cater to global audiences.
Using sentiment trend analysis for broader insights into online behavior.
Developing predictive tools to identify potential risks before they escalate.
Call to Action
The fight against cyberbullying isn’t just a technical challenge; it’s a human one. Whether you’re a developer building solutions, an educator advocating for change, or a parent protecting your child, tools like Vertex AI empower us to create a kinder digital world.

Ready to make a difference? Start building your solution today, and together, we can combat cyberbullying and foster a safer internet for all.
