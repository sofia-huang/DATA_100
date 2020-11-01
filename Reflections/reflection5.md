# Data Science Reflection
### Alexa and Natural Language Processing
-------
Amazon’s Alexa, as well as, other smart home devices obviously use artificial intelligence as the main basis of their system. I decided to research on how exactly it works and what processes are used. Alexa is built using natural language processing (NLP) to interpret the commands that users say. NLP encapsulates speech recognition and the data is broken up into individual sounds and compared with a massive database to find the words that most closely correspond with the individual sounds. Alexa records your command and sends it to Amazon’s cloud servers to interpret. The servers then send back the information Alexa needs to fulfill the order.
If it identifies certain key words, it uses them to determine what function to do in order to carry out the task at hand. For example, if Alexa heard you say “weather” it might open that app or understand that you want to know the current weather. 

First, the system must do signal processing. This cleans up the audio that was recorded by minimizing background noise and amplify the user’s voice. It determines where the sound is coming from so that it can focus on it and use acoustic echo cancellation to keep only the important part of the audio to interpret. 

Then, it uses “Wake Word Detection” to tell if you want to turn the device on, such as “Alexa”. This decreases false negatives and false positives if Alexa turns on when it does not need to or if it doesn’t turn on when needed. It converts the audio into text and analyze characteristics of the speech to turn into feature values. In order to interpret the command, it uses the features and the model to come up with the most likely sequence of words. It uses two parts, the prior and the acoustic model. The prior gives the sequence without looking at the features and just the text data. The acoustic model uses deep learning and looks at pairings of audio and text to determine the sequence. The two models are combined, in real time, to give the final most likely sequence of words. 

Alexa interprets the command by splitting it into three parts, the wake word, the invocation name, and the utterance. The invocation name is a keyword that represents a specific skill in Alexa’s capabilities and is used to start the task. The utterance is a word or phrase that specifically tells Alexa what she needs to do and what the user’s intent is.  

NLP is a combination of linguistics, computer science, and AI. It is the processes that happen when a computer analyzes natural language data and the interactions between computers and natural language. The field currently uses neural networks for machine learning vs statistical models which requires thorough feature engineering. Some NN models utilize transfer learning where scientists use the model’s previous training experience to learn a new task more quickly. This is more efficient and economical than having to start all over and is more like fine-tuning. Others make use of recurrent neural networks which create dependencies within the layers as each one relies on the previous. 

One of the major challenges for deep learning is called the Clever Hans effect. This is when the algorithm finds impressive patterns that are not useful in real-world applications. An example would be a model determining a disease based on the type of machine used. This is a correlation that cannot be used to make conclusions and need to be reassessed by the analyzers. 

-------
### Works Cited

Gonfalonieri, Alexandre. “How Amazon Alexa Works? Your Guide to Natural Language Processing (AI).” Medium. Towards Data Science, December 31, 2018. https://towardsdatascience.com/how-amazon-alexa-works-your-guide-to-natural-language-processing-ai-7506004709d3. 

Marketing, Exxact. “The Unreasonable Progress of Deep Neural Networks in NLP.” Exxact, June 3, 2020. https://blog.exxactcorp.com/the-unreasonable-progress-of-deep-neural-networks-in-natural-language-processing-nlp/. 

“Natural Language Processing.” Wikipedia. Wikimedia Foundation, October 29, 2020. https://en.wikipedia.org/wiki/Natural_language_processing. 
