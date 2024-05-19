# LangChain Chatbot Repository

This repository contains two Python scripts that utilize the LangChain framework for creating LLM-based chatbots. Each script demonstrates how to leverage different models for chatbot applications. Both applications can be monitored using LangSmith.

## Scripts

1. **app.py** - Uses OpenAI's GPT-3.5-turbo model to create a chatbot with a sarcastic tone.
2. **llama.py** - Utilizes the open-source LLaMA model via Ollama to create a similar chatbot with a sarcastic tone.

## Installation

To run these scripts, you need to have Python installed along with the required dependencies. You can install the necessary packages using the following command:

```bash
pip install -r requirements.txt
```

Create a `.env` file in the root directory of the repository and add your OpenAI and LangChain API keys:

```env
OPENAI_API_KEY=your_openai_api_key
LANGCHAIN_API_KEY=your_langchain_api_key
```

## Usage

### app.py

This script creates a chatbot using OpenAI's GPT-3.5-turbo model.

```bash
streamlit run app.py
```

### llama.py

This script creates a chatbot using the open-source LLaMA model via Ollama.

```bash
streamlit run llama.py
```

## Monitoring

Both applications can be monitored using LangSmith. Ensure that LangSmith tracking is enabled by setting the appropriate environment variables in your `.env` file:

```env
LANGCHAIN_TRACING_V2=true
```

## Example

After running either script, you can interact with the chatbot via the Streamlit interface. Simply input your query and get responses with a sarcastic tone.

## Contributing

Feel free to fork this repository, make improvements, and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License.

---

### `requirements.txt`

Make sure to include a `requirements.txt` file with the necessary dependencies:

```
streamlit
python-dotenv
langchain_openai
langchain_core
langchain_community
```

### Directory Structure

```
.
├── app.py
├── llama.py
├── requirements.txt
├── .env
└── README.md
```

This structure ensures that your repository is organized and easy to navigate for anyone who wants to use or contribute to your project.
