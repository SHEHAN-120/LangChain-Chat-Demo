# LangChain Sentiment Demo

This is a simple demonstration of using **LangChain** to create a basic sentiment analysis app with few-shot learning. It showcases how to engineer prompts and classify user input as **positive**, **neutral**, or **negative** using OpenAI's GPT models.

## Features

* Built using `PromptTemplate` and `FewShotPromptTemplate`
* Shows how to structure few-shot examples in LangChain
* Minimal code — ideal for learning or prototyping
* Outputs AI sentiment responses based on the given review

## Technologies Used

* Python
* LangChain
* OpenAI API

## How It Works

1. Few-shot examples are embedded using `FewShotPromptTemplate`
2. User input is appended at the end of the prompt
3. Output is generated using OpenAI's language model

## Example Output

```
Identify the sentiment of the user review. Here are some examples:

User:I love this product
AI:positive

User:It was an average experience
AI:neutral

User:I wonder why it is so highly rated.
AI:negative

User:What is the meaninig of Deep learninig?
AI:negative
```

## Getting Started

```python
import os
os.environ["OPENAI_API_KEY"] = "api_key"
```

Then run the script and provide a review input to get the sentiment.

