#  Deep Research Assistant

Deep Research Assistant is an AI-powered research automation tool designed to streamline the process of collecting and summarizing information from the web. It utilizes intelligent agents to search the web based on user queries and generates concise summaries optimized for quick understanding and further synthesis.

##  Features

-  Web-based search using intelligent agents
-  Succinct 2–3 paragraph summaries under 300 words
-  Email delivery of research results using SendGrid
-  Asynchronous execution using Python's asyncio
-  Secure API key management using dotenv

##  Tech Stack

- **Python**
- **Pydantic** – for input modeling
- **SendGrid** – for sending summaries via email
- **dotenv** – for environment configuration
- **Custom Agent Framework** – handles web search and summarization

##  Project Structure

```
deep_research/
├── agents/                # Contains custom Agent, WebSearchTool, and utility logic
├── .env                   # Environment variables (e.g., SendGrid API key)
└── deep_research.ipynb    # Main notebook for running the assistant
```

##  Usage

1. **Install dependencies** (using `requirements.txt`):
    ```bash
    pip install -r requirements.txt
    ```

2. **Set up environment variables** in a `.env` file:
    ```
    SENDGRID_API_KEY=your_api_key
    FROM_EMAIL=your_verified_email@example.com
    TO_EMAIL=recipient@example.com
    ```

3. **Run the notebook**:
    Open `deep_research.ipynb` in Jupyter and follow the instructions inside.

##  Emailing Results

The assistant can send the summarized results via email using SendGrid. Ensure your SendGrid credentials are correct in the `.env` file, and that the sender email is verified.

##  License

MIT License – Feel free to use and modify for personal or professional research workflows.

##  Author

Cheran C
