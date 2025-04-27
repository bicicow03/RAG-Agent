# RAG-Agent(LangChain)

Desgined to assist in task planning on notion with 2 main functions:
1.Grab general information and content about a specific document
2.Help plan out a task on notion by gathering all current information about the task available in the database and creating a guide on what needs to be done by specific dates to complete the task/project before the due date.

Link to notion database page: [https://www.notion.so/192dbce6201c80e490b9df38dd0af15c?v=192dbce6201c806eb49a000c89ab4dc5&pvs=4 ](https://www.notion.so/192dbce6201c80e490b9df38dd0af15c?v=192dbce6201c806eb49a000c89ab4dc5&pvs=4)

Code instructions:
1. Signup and get your own API for the NVDIA models for the code to run.(its free*) https://build.nvidia.com/explore/discover?ncid=no-ncid 
2. It requireas multiple libraries to be installed which will come up as errors when you first try to run the code. Installation of these libraries will fix the issues.
   
Note: The model is still under progress and being refined and some one the first function may not work correctly yet due issue with the embedder and retriever not always giving the LLMs the correct documents.
Update (3/4/2025): The model now works perfectly except that it won't show content inside any document despite been given both meta data and content of document; working on the cause and a fix currently.

# RAG-Agent(LangGraph)

A RAG Agent model with ability to keep track and adapt to conversation flow, retrieve informatino on documents in the notion database specified above. 
This model has same capabilites as the one above, however, it's able to handle more complex request for information on the database, while also being a chatbot.(shown in code)
There is a tool function to update status update of task/docuemtns in the notion database. however, it doesn't work after mutliple attempts to try and debugg it(using Gemini). This is likely
because we're using the Notion DataBase to retrieve information and we can only update of we used a Notion Page first; as one of the key things needed to update task in Notion requires a PageID
and we only have a DataBase ID. 

(There's no demo video for LangGraph RAG Agent, look at code for demonstration and outputs of model)
Upcoming/Future improvements:
Better Prompt engineering to improve model response and flow
Replace current tool function with a websearch tool function instead.
