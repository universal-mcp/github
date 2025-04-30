# Universal Mcp Github MCP Server

An MCP Server for the Universal Mcp Github API.

## 📋 Prerequisites

Before you begin, ensure you have met the following requirements:
* Python 3.11+ (Recommended)
* [uv](https://github.com/astral-sh/uv) installed globally (`pip install uv`)

## 🛠️ Setup Instructions

Follow these steps to get the development environment up and running:

### 1. Sync Project Dependencies
Navigate to the project root directory (where `pyproject.toml` is located).
```bash
uv sync
```
This command uses `uv` to install all dependencies listed in `pyproject.toml` into a virtual environment (`.venv`) located in the project root.

### 2. Activate the Virtual Environment
Activating the virtual environment ensures that you are using the project's specific dependencies and Python interpreter.
- On **Linux/macOS**:
```bash
source .venv/bin/activate
```
- On **Windows**:
```bash
.venv\\Scripts\\activate
```

### 3. Start the MCP Inspector
Use the MCP CLI to start the application in development mode.
```bash
mcp dev src/universal_mcp_github/mcp.py
```
The MCP inspector should now be running. Check the console output for the exact address and port.

## 🔌 Supported Integrations

- AgentR
- API Key (Coming Soon)
- OAuth (Coming Soon)

## 🛠️ Tool List

This is automatically generated from OpenAPI schema for the Universal Mcp Github API.

| Tool | Description |
|------|-------------|
| `star_repository` | Stars a GitHub repository using the GitHub API and returns a status message. |
| `list_commits` | Retrieves and formats a list of recent commits from a GitHub repository |
| `list_branches` | Lists all branches for a specified GitHub repository and returns them in a formatted string representation. |
| `list_pull_requests` | Retrieves and formats a list of pull requests for a specified GitHub repository. |
| `list_issues` | Retrieves a list of issues from a specified GitHub repository with optional filtering parameters. |
| `get_pull_request` | Retrieves and formats detailed information about a specific GitHub pull request from a repository |
| `create_pull_request` | Creates a new pull request in a GitHub repository, optionally converting an existing issue into a pull request. |
| `create_issue` | Creates a new issue in a specified GitHub repository with a title, body content, and optional labels. |
| `update_issue` | Updates an existing GitHub issue with specified parameters including title, body, assignee, state, and state reason. |
| `list_repo_activities` | Retrieves and formats a list of activities for a specified GitHub repository. |

## 📁 Project Structure

The generated project has a standard layout:
```
.
├── src/                  # Source code directory
│   └── universal_mcp_github/
│       ├── __init__.py
│       └── mcp.py        # Server is launched here
│       └── app.py        # Application tools are defined here
├── tests/                # Directory for project tests
├── .env                  # Environment variables (for local development)
├── pyproject.toml        # Project dependencies managed by uv
├── README.md             # This file
```

## 📝 License

This project is licensed under the MIT License.

---

_This project was generated using **MCP CLI** — Happy coding! 🚀_
