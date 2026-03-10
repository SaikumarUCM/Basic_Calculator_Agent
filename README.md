# Calculator Agent

A simple AI-powered calculator agent built with LangChain and LangGraph. The agent can perform basic arithmetic operations (addition, subtraction, multiplication, division) by interpreting natural language instructions.

## Features

- Performs sequential arithmetic operations based on user queries.
- Uses OpenAI's GPT-4 for reasoning and tool calling.
- Handles errors gracefully (e.g., division by zero).

## Requirements

- Python 3.8+
- OpenAI API key

## Installation

1. Clone or download the repository.
2. Install dependencies:
   ```
   pip install langchain-openai langgraph python-dotenv
   ```
3. Create a `.env` file in the project root and add your OpenAI API key:
   ```
   OPENAI_API_KEY=your_openai_api_key_here
   ```

## Usage

Run the example script:
```
python User.py
```

This will execute a sample arithmetic sequence and print the results.

## Files

- `calculator_agent.py`: Defines the agent, tools, and graph.
- `User.py`: Example usage script.

## How It Works

The agent uses LangGraph to manage a conversation flow:
- Receives a user query.
- Calls appropriate arithmetic tools.
- Returns the final result.

For more details, see the code comments.