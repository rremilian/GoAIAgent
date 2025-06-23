# GoAIAgent

GoAIAgent is a command-line AI agent powered by Anthropic's Claude models, designed to interact with users and perform a variety of tasks through a set of built-in tools. The agent can read and edit files, list directory contents, execute safe shell commands, and fetch web content.

## Features

- **Conversational AI**: Chat with Claude in your terminal.
- **File Operations**: Read, list, and edit files in your working directory.
- **Command Execution**: Safely execute shell commands with user confirmation and guardrails.
- **Web Fetching**: Retrieve and extract visible text from web pages.
- **Extensible Tools**: Easily add new tools by defining their schema and logic.

## Requirements

- Go 1.18+
- [Anthropic Claude API key](https://docs.anthropic.com/claude/docs/quickstart)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/rremilian/GoAIAgent.git
   cd GoAIAgent
   ```
2. Install dependencies:
   ```bash
   go mod tidy
   ```

## Usage

1. Set your Anthropic API key as an environment variable:
   ```bash
   export ANTHROPIC_API_KEY=your_api_key_here
   ```
2. Run the agent:
   ```bash
   go run main.go
   ```
3. Start chatting! Type your message and press Enter. Use `ctrl-c` to quit.

## Built-in Tools

- **read_file**: Read the contents of a file by relative path.
- **list_files**: List files and directories at a given path.
- **edit_file**: Replace text in a file or create a new file.
- **command_execution**: Execute safe shell commands (with confirmation and restrictions).
- **fetch_url**: Fetch and extract visible text from a web page.
