# RAG-Agent

Desgined to assist in task planning on notion with 2 main functions:
1.Grab general information and content about a specific document
2.Help plan out a task on notion by gathering all current information about the task available in the database and creating a guide on what needs to be done by specific dates to complete the task/project before the due date.

Link to notion database page: https://www.notion.so/192dbce6201c80e490b9df38dd0af15c?v=192dbce6201c806eb49a000c89ab4dc5&pvs=4 

Code instructions:
1. Signup and get your own API for the NVDIA models for the code to run.(its free*) https://build.nvidia.com/explore/discover?ncid=no-ncid 
2. It requireas multiple libraries to be installed which will come up as errors when you first try to run the code. Installation of these libraries will fix the issues.
   
Note: The model is still under progress and being refined and some one the first function may not work correctly yet due issue with the embedder and retriever not always giving the LLMs the correct documents.
Update (3/4/2025): The model now works perfectly except that it won't show content inside any document despite been given both meta data and content of document; working on the cause and a fix currently.
