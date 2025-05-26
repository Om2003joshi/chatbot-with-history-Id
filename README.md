# chatbot-with-history-Id
Build  a simple   chatbot with using goq api ,using history and id

In this ipynb We'll go over an example of how to design and implement an LLM-powered chatbot. This chatbot will be able to have a conversation and remember previous interactions.

We can use a Message History class to wrap our model and make it stateful. This will keep track of inputs and outputs of the model, and store them in some datastore. Future interactions will then load those messages and pass them into the chain as part of the input. Let's see how to use this!

Prompt Templates help to turn raw user information into a format that the LLM can work with. In this case, the raw user input is just a message, which we are passing to the LLM. Let's now make that a bit more complicated. First, let's add in a system message with some custom instructions (but still taking messages as input). Next, we'll add in more input besides just the messages.
