
The CLI interprets natural language prompting, fetches real-time Zoho Projects data (RAG), outputs structured JSON or tables, and calls functions that invoke Zoho APIs to automate actions.

## Architecture Overview

- **Prompting:**  
Uses Large Language Models (LLMs) with prompt templates to capture user intent expressed in natural language.

- **Retrieval-Augmented Generation (RAG):**  
Queries Zoho Projects API endpoints to fetch contextual data such as projects, tasks, comments, and timelines. Uses embedding-based or keyword search techniques for efficient retrieval.

- **Structured Output:**  
Formats AI-generated responses as JSON, markdown tables, or custom schemas, enabling human-friendly CLI display and automation-friendly downstream processing.

- **Function Calling:**  
Maps user intents recognized from prompting or AI-generated signals to Python functions that perform Zoho Projects API operations. Examples include creating/updating tasks, assigning users, scheduling reminders, or sending notifications.

## Zoho Projects API Integration

- Uses Zoho Projects REST API v3  
- Supports CRUD operations on projects, tasks, comments, users, and timesheets  
- API base URL: `https://projectsapi.zoho.com/api/v3/`

### Important API Features

- Retrieve project lists and details  
- Search projects, tasks, and comments  
- Create, update, or delete tasks and comments  
- Manage users and assignments within projects  

Refer to full API doc: [Zoho Projects API Documentation](https://projects.zoho.com/api-docs)


## Future Work

- Integrate with Slack, Jira, and other productivity apps for richer context  
- Develop a web dashboard to complement the CLI


## References

- Zoho Projects API docs: [https://projects.zoho.com/api-docs](https://projects.zoho.com/api-docs)  
- LangChain libraries for RAG implementation  
- GenAI API for LLM prompting and function calling

---
