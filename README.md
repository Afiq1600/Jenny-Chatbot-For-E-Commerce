# Jenny-Chatbot-For-E-Commerce
Chatbot model using machine learning techniques with deep learning to get the best chatbot performance. A chatbot model is able to response answer regarding to a customer’s question with the right context. This finding is beneficial for smartphone e-commerce companies throughout the world.


# Implementation of a Contextual Chatbot in Keras.  
Simple chatbot implementation with Keras. 

- The implementation should be easy to follow for beginners and provide a basic understanding of chatbots.
- The implementation is straightforward with a Feed Forward Neural net with 1 hidden layers.
- Customization for your own use case is super easy. Just modify `intents.json` with possible patterns and responses and re-run the training (see below for more info).


## Installation

### Create an environment at anaconda 3.0
Whatever you prefer (e.g. `conda`)
```Anaconda console
conda create -n myenv Python=3.9
cd Microsoft VS Code
code
```

### Activate it
Windows:
```Anaconda console
conda activate myenv
```
### Install PyTorch and dependencies
You also need `nltk`:
 ```terminal microsoft vs code console
pip install nltk

If you get an error during the first run, you also need to install `nltk.tokenize.punkt`:
Run this once in your terminal:
 ```terminal microsoft vs code console
$ python
>>> import nltk
>>> nltk.download('punkt')
```

## Usage
Run
```terminal microsoft vs code console
python train_chatbot.py
```

```terminal microsoft vs code console
python chatgui.py
```

## Running local server
Run
```terminal microsoft vs code console
python app.py
```

## Launch Chatbot
Click base.html
```chatbotProject1/standalone-frontend/base.html
```

## Customize
Have a look at [intents.json](intents.json). You can customize it according to your own use case. Just define a new `tag`, possible `patterns`, and possible `responses` for the chat bot. You have to re-run the training whenever this file is modified.
```console
{
  "intents": [
    {
      "tag": "greeting",
      "patterns": [
        "Hi",
        "Hey",
        "How are you",
        "Is anyone there?",
        "Hello",
        "Good day"
      ],
      "responses": [
        "Hey :-)",
        "Hello, thanks for visiting",
        "Hi there, what can I do for you?",
        "Hi there, how can I help?"
      ]
    },
    ...
  ]
}
```
