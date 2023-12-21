# AWS-EC2-Chatbot with Knowledge Graph using Neo4j Graph
This project aims to construct a knowledge graph from a selected section of AWS documentation. The knowledge graph will represent key entities and their relationships, providing a structured and easily accessible view of the information contained in the documentation.

## Objective
Develop a knowledge graph representing key concepts, services, and relationships from a selected
portion of AWS documentation.

## Steps
1. Selecting a Section of AWS Documentation: Choosing a specific part of the AWS documentation for analysis.
2. Extracting and Preprocess Text: Implementing text extraction and preprocessing techniques suitable for knowledge graph construction. Converting the text into a format suitable for entity and relationship extraction.
3. Identifing Entities and Relationships: Identify key entities and their relationships within the text. This involves named entity recognition, co-reference resolution, and relation extraction techniques. Using GPT 3.5 Language Learning Models (LLMs) for extraction.
4. Prompting the GPT: The GPT is prompted for the suitable use case scenario of AWS EC2 chatbot.
5.  Constructing the Knowledge Graph using Neo4j:We will extract information from the AWS EC2 documentation and construct a knowledge graph to test the pipeline. Here, we will utilize UnstructuredPDFLoader and text chunking modules provided by LangChain.
6.  Querying: Using LLMs to write insert queries that create a graph structure in Neo4j. Specifying which node labels should be extracted by the LLM. Accurately representing the extracted entities and relationships. Ensuring that the graph is correctly indexed for efficient querying
7.  Query the knowledge graph in a RAG application: Using Graph Cypher QA Chain class from langchain module for question-answering against a graph by generating Cypher statements and then using GPT 3.5 to answer questions based on the query results.

# FlowChart

![alt text](https://github.com/kushjaggi/AWS-EC2-Chatbot-KG/blob/main/Flowchart/1_qC53DXQRyTYJVyKeHZ1rbA.webp)

# Knowledge Graphs

![alt text](https://github.com/kushjaggi/AWS-EC2-Chatbot-KG/blob/main/Knowledge%20Graph/visualisation%20(7).png)
![alt text](https://github.com/kushjaggi/AWS-EC2-Chatbot-KG/blob/main/Knowledge%20Graph/visualisation%20(4).png)
![alt text](https://github.com/kushjaggi/AWS-EC2-Chatbot-KG/blob/main/Knowledge%20Graph/visualisation%20(3).png)
![alt text](https://github.com/kushjaggi/AWS-EC2-Chatbot-KG/blob/main/Knowledge%20Graph/visualisation.png)
