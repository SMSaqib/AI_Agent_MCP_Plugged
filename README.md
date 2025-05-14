# AI Agent MCP-Plugged 🤖

## Overview
AI Agent MCP-Plugged is an intelligent assistant powered by OpenAI's Gemini model and integrated with MCP tools for enhanced functionality. It provides insightful, well-structured responses and supports calculations such as tax computation, loan repayment, and compound interest.
demo: https://saqibkareem-sk-ai-agent.hf.space/
## Features
- **Conversational AI**: Engages in meaningful conversations using OpenAI's Gemini model.
- **MCP Tool Integration**: Supports tax calculation, loan repayment, and compound interest computations.
- **Tech Blogging Capability**: Generates blogs exclusively on tech topics using the `how_many_words` tool.
- **Streamlit UI**: Provides an interactive chat interface for seamless user interaction.
- **Chat History**: Maintains conversation history for context-aware responses.

## Installation

### Prerequisites
- Python 3.8+
- OpenAI API Key (Gemini)
- MCP Server Access
- Streamlit

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/ai-agent-mcp.git
Navigate to the project directory:

bash
cd ai-agent-mcp
Install dependencies:

bash
pip install -r requirements.txt
Set up environment variables:

Create a .env file in the root directory.

Add your OpenAI API key:

env
GEMINI=your_openai_api_key
Run the application:

bash
streamlit run app.py
Configuration
Modify the Agent initialization in app.py to customize the assistant:

python
agent = Agent(
    name="Assistant",
    instructions="""You are a highly capable assistant that provides accurate, insightful, and well-structured responses using available tools and MCP servers. Your goal is to efficiently assist users with clear, relevant, and comprehensive answers while maintaining an engaging and professional tone.
    You have additional capability to generate blogs exclusively on tech topics using the 'how_many_words' tool.""",
    mcp_servers=[mcp_server],
    model=model
)
Usage
Chat Interaction: Users can type messages, and the assistant will respond dynamically.

MCP Tool Utilization: The assistant can calculate tax, loan repayment, and compound interest.

Tech Blogging: Generates blog content on technology topics using specialized tools.

API Integration
The assistant integrates with MCP servers for enhanced capabilities:

python
async with MCPServerSse(
    name="Tax Calculator MCP Server",
    params={
        "url": "https://saqibkareem-mcp-server-tool.hf.space/sse",
        "cache_tools_list": True
    }) as mcp_server:
    tool_list = await mcp_server.list_tools()
Contribution
Contributions are welcome! To contribute:

Fork the repository.

Create a new branch.

Make your changes and submit a pull request.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Contact
For questions or support, reach out via:

Email: saqib.kareem.gmb@gmail.com

GitHub Issues: Create an issue

This README.md provides a comprehensive guide to your AI assistant, covering installation, usage, configuration, and contribution details. Let me know if you need any modifications! 🚀

make single file so i can copy paste
Sure! Here's the complete README.md file in a single block so you can easily copy and paste it:

markdown
# AI Agent MCP-Plugged 🤖

## Overview
AI Agent MCP-Plugged is an intelligent assistant powered by OpenAI's Gemini model and integrated with MCP tools for enhanced functionality. It provides insightful, well-structured responses and supports calculations such as tax computation, loan repayment, and compound interest.

## Features
- **Conversational AI**: Engages in meaningful conversations using OpenAI's Gemini model.
- **MCP Tool Integration**: Supports tax calculation, loan repayment, and compound interest computations.
- **Tech Blogging Capability**: Generates blogs exclusively on tech topics using the `how_many_words` tool.
- **Streamlit UI**: Provides an interactive chat interface for seamless user interaction.
- **Chat History**: Maintains conversation history for context-aware responses.

## Installation

### Prerequisites
- Python 3.11+
- OpenAI API Key = dummy
- Gemini API Key
- MCP Server Access
- Streamlit

### Steps
1. Clone the repository:
   ```bash
git clone https://huggingface.co/spaces/saqibkareem/SK_AI_Agent
Navigate to the project directory:

bash
cd ai-agent-mcp
Install dependencies:

bash
pip install -r requirements.txt
Set up environment variables:

Create a .env file in the root directory.

Add your OpenAI API key:

env
GEMINI=your_openai_api_key
Run the application:

bash
streamlit run app.py
Configuration
Modify the Agent initialization in app.py to customize the assistant:

python
agent = Agent(
    name="Assistant",
    instructions="""You are a highly capable assistant that provides accurate, insightful, and well-structured responses using available tools and MCP servers. Your goal is to efficiently assist users with clear, relevant, and comprehensive answers while maintaining an engaging and professional tone.
    You have additional capability to generate blogs exclusively on tech topics using the 'how_many_words' tool.""",
    mcp_servers=[mcp_server],
    model=model
)
Usage
Chat Interaction: Users can type messages, and the assistant will respond dynamically.

MCP Tool Utilization: The assistant can calculate tax, loan repayment, and compound interest.

Tech Blogging: Generates blog content on technology topics using specialized tools.

API Integration
The assistant integrates with MCP servers for enhanced capabilities:

python
async with MCPServerSse(
    name="Tax Calculator MCP Server",
    params={
        "url": "https://saqibkareem-mcp-server-tool.hf.space/sse",
        "cache_tools_list": True
    }) as mcp_server:
    tool_list = await mcp_server.list_tools()
Contribution
Contributions are welcome! To contribute:

Fork the repository.

Create a new branch.

Make your changes and submit a pull request.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Contact
For questions or support, reach out via:

Email: saqib.kareem.gmb@gmail.com

GitHub Issues: Create an issue
