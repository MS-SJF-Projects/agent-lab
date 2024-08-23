# The role of an Agent in Generative AI applications

To understand what an Agent is, let's first see the different kind of Generative AI apps.  

You can see them in the picture below, where the use of a pyramid denotes that each one is built on top of the other.

<img src="images/pyramid.png" width="400">  

- **Q&A**  
 The most simple 'app' where the model just replies to a single question.
  - User: *What is the capital of France?*
  - Agent: *The capital of France is Paris*  

- **CHAT**: An evolution of the Q&A app where the both questions and answers become part of a conversation, like:
  - User: *What is the capital of France?*
  - Agent: *The capital of France is Paris*
  - User: *and how many inhabitants does it have?*
  - Agent: *As of 2024, the population of Paris is approximately 2.09 million people*

    For this kind of app, the conversation is kept in a *short term memory* (the Message history)
- **RAG** (Retrieval Augmented Generation)  
  In this case the model input is enriched with information from external sources (private and/or public) in order to expand its domain of knowledge.
  - User: *Tell me the number our customers in the Zurich area who spent more than 5000 CHF this month.*
  - Agent: *The total is 1340*
  - User: *Organize them by age, gender and residential area.*
  - Agent: *...*

- **AGENT**  
  At this level the model is not just processing specific requests, but is now instructed to take decisions and execute tasks depending on the provided input.  

    Since with *task* we intend **code execution**, it means that the Agent "can run" code that:
  - *Send an email.*
  - *Store information into a database.*
  - *Invokes a remote endpoint*
  - ...

    We'll see **how** in this lab, but as you can imagine this type of possibility opens the way to an infinite number of use cases.  

- **AGENTIC**  
  It is the equivalent of architectures based on microservices, where each single service is an Agent and the orchestration is managed by frameworks such as [Autogen](https://microsoft.github.io/autogen/) or [CrewAI](https://www.crewai.com/).  

You can now understand what level of complexity we are at and how, with Agents, the role of the model changes from a simple assistant to something capable of making decisions and act autonomously based on a set of rules that have been indicated to it.  

In some ways it is like dealing with a very skilled person who however has zero knowledge of the task we want to assign to him and therefore the ability to explain what we want to achieve plays a fundamental role.  
The fact that there is also code running makes this even more intriguing.
