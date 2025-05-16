# n8n-prj1
This is a repository to save all my n8n workflow data in JSON format.
This particular JSON file contains data regarding a sample n8n woorkflow i developed.
Now this workflow has a LLM model (openAI Chat GPT 4o-mini) connected to an AI agent.
The AI agent is also connected to a buffer storage for memory of upto 5 chats and a google spreadsheet containing some sample data.
Now the agent is triggered via a chat message, and the software processes the query in the chat as follows:
1. the agent accepts the query and sends it to the LLM model to help understand the task needed to be perfomed by the query, and stores this in the buffer. 
2. the agent then connects with the data in the sheet to execute the query, programmed by the LLM model based on the user input.
3. The result of the query is passed on to the agent which then sends it back to the LLM model to generate an output in a human like format.
4. As this output is produced, the query data is also stored in the memory for future reference.

This is how the AI agent executes the command. It is connected with the data in a live format and hence can also perform CRUD operations. 
In my further projects, I will add analysis and visualisation tools to produce better insights.