# Setup env

```
git clone git@github.com:snorkel-ai/mcp-atlassian.git
cd mcp-atlassian

uv venv  # creates a virtual environment if you haven’t yet
source .venv/bin/activate

uv pip install -e .  # install your project in editable mode
```
Now the mcp-atlassian is available by calling `<path to dir>/.venv/bin/mcp-atlassian`, for example: `/Users/jiohyoo/projects/mcp-atlassian/.venv/bin/mcp-atlassian`


# Setup MCP in Claude Desktop App
```
{
    "mcpServers": {
        "mcp-atlassian": {
            "command": "<path to dir>/.venv/bin/mcp-atlassian",
            "args": [],
            "env": {
              "JIRA_URL": "https://snorkelai.atlassian.net",
              "JIRA_USERNAME": "<your email@snorkel.ai>",
              "JIRA_API_TOKEN": "<jira api token>"
            }
        }
    }
}
```
