# commvault_chatbot
The Commvault Chatbot is an NLP-powered tool designed to help Commvault employees quickly find relevant documentation and resolve technical issues. Combining intent recognition and semantic similarity streamlines the process of accessing helpful resources. Key features include:
- Intent Recognition: A PyTorch-based neural network classifies user queries into predefined categories using training data from intents.json.
- Article Recommendation: Integrates with xml_nlp.py to suggest relevant URLs based on user queries, improving resource discovery.
- Dynamic Responses: Provides predefined replies for general intents and fallback responses for low-confidence predictions.
- Custom Training: Includes train.py for retraining the model with new intents or data, with results stored in data.pth.
- Interactive CLI: Runs on a lightweight command-line interface for direct user interaction.
With these features, the chatbot improves productivity by delivering fast, context-aware responses to employee queries. It is extensible and can be enhanced for web deployment using the included Flask-based web components.

How to Use:
First, install all necessary libraries: numpy, pandas, pytorch (torch), NLTK, flask, transformers, scikit-learn, and python's XML library 
After installing all libraries, run nltk_utils.py and uncomment the "nltk.download()" program to download the necessary nltk packages *You do not need to run it after the first time so you can re-comment or delete it* 
There is a data.pth file included, but changes to this file are needed, run train.py to create a new one
To run the app, run app.py
