# Foodie Chatbot

Conversational bot (chat-bot) which can help users discover restaurants across several Indian cities using Zomato API.

The main purpose of the bot is to help users discover restaurants quickly and efficiently and to provide a good restaurant discovery experience. The project brief provided to you is as follows.

The bot takes the following inputs from the user:
- City
- Cuisine
- Avg budget for 2 people

Based on these three inputs, bot queries the zomato API and fetches the top five restaurants based on the ranking.

## What are Chatbots?

Chatbots have become popular in a large number of business domains. Companies are building chatbots for booking hotels, flights, movies etc., customer support, enquiring bus and train schedules, tax saving advice, accessing stock market information etc.

There are two broad types of chatbots - generic chatbots and domain-specific chatbots.

Generic chatbots, also called virtual assistants, such as Google Assistant, Amazon’s Alexa, Microsoft’s Cortana or Apple’s Siri, are used to answer generic queries such as dialling a phone number, dropping a message to a contact, booking a calendar slot, fetching results from a web search, etc. These systems have been trained on massive amounts of user data, encyclopedias, conversational dialogues with humans etc.

The other type is the domain-specific, task-oriented chatbot. By domain-specific and task-oriented, we mean that it can handle queries pertaining to a particular domain or type of task. For example, a ‘weather bot’ can only tell weather predictions. It cannot book a table in a restaurant or set up an alarm. Similarly, a restaurant discovery bot can help you find restaurants in several cities, though it might not be able to answer general questions such as "Who is the prime minister of India?".

## Building Chatbot using RASA

We are going to use an open source framework for building conversational bots - RASA.

RASA - An open source Conversational AI is a set of machine learning tools for developers to create contextual text and voice-based chatbots and assistants.

Apple’s Siri, Amazon’s Alexa etc. are much more than a 'speech-based search engine'. Apart from searching for information (e.g. from Wikipedia, YouTube, Google etc.), they can 'talk' to us in natural language.

Conversation, or dialogue, is a very fundamental aspect of human language, and arguably the most interesting challenge in building truly intelligent NLP systems. A step towards building such systems is domain specific, text-based chatbots used by organisations for tasks such as booking hotels, retrieving stock market information, resolving customer queries etc.

Any conversational system has primarily two components -

Natural Language Understanding, or NLU
A Dialogue Management System which carries out the overall conversation.
In Rasa, these two components are named Rasa NLU and Rasa Core respectively.

Rasa NLU is the tool used for intent classification and entity extraction.

Rasa Core, the dialogue management layer of Rasa, takes structured input in the form of intents and entities (i.e. the output of Rasa NLU) and decides the next actions.

## Prerequisites

- Python 3.6 or above
- Rasa
- Visual Studio Community 2019 (For Windows only)

## Installation

Install Rasa 

``` bash
pip install rasa
```

Visual Studio: (For Windows only)

1. Open the Microsoft Visual Studio link: https://visualstudio.microsoft.com/downloads/

2. Select ‘Community version 2019’

3. Download the installer and select VC++ Build tools on the list

## Usage

### Training 

- Rasa NLU (make sure that you feed your data in data/nlu.md file for training on your own specific data)

``` bash
rasa train nlu
```

- Conversation Flow training using Rasa Core (modify data/stories.md and domain.yml file for training on custom data)

``` bash
rasa train core
```
