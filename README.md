# Multi-Agent-Financial-Research-Assitant
This project aims to build a multi-agent architecture for financial investment research and anlysis. 
The website used to get the relevant articles link is Newsapi website. 
The first the user gives the query to the news api. 
For Example
ALL Stocks about gold prices. 
The the news api returns the list of the articles with their links, and short description. 

# We will be utilizing CrewAI 
-------------------------------------------
#Project Architecture: 


We will organize the project into separate components, each responsible for a specific task.
📁 investment_research_assistant/ (Root Project Folder)
├── 📁 agents/ → CrewAI agents for handling different tasks
│ ├── news_scraper.py → Fetches financial news
│ ├── sentiment_analysis.py → Analyzes sentiment of articles
│ ├── rag_retrieval.py → Stores & retrieves relevant articles
│ ├── summarization.py → Generates investment insights
│
├── 📁 tools/ → Reusable AI tools used by agents
│ ├── scraper_tool.py → Handles web scraping logic
│ ├── sentiment_tool.py → Uses FinBERT for sentiment analysis
│ ├── vector_db.py → Stores embeddings in a vector database
│ ├── rag_tool.py → Retrieves relevant articles using similarity search
│
├── 📁 data/ → Stores raw scraped articles and embeddings
│ ├── articles/ → Raw news articles
│ ├── embeddings/ → Vector database storage
│
├── 📁 configs/ → Configuration settings for API keys, models, etc.
│ ├── config.yaml → Stores API keys, database URLs, etc.
│
├── main.py → Orchestrates the entire workflow

