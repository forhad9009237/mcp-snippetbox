# mcp-snippetbox

MCP server template I base new tools on

Started as a weekend hack, grew on me.

## What it does

- Includes Claude Desktop config snippet
- Three tools: add / get / list notes
- State persisted to a JSON file in the home dir
- FastMCP style: decorators, zero boilerplate

## Install

```bash
pip install -r requirements.txt
```

## Examples

```bash
# claude_desktop_config.json
# {
#   "mcpServers": {
#     "notes-box": {"command": "python", "args": ["server.py"]}
#   }
# }
python server.py
```

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   ├── dependabot.yml
│   └── pull_request_template.md
├── docs/
│   ├── development.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── .editorconfig
├── .gitattributes
├── .gitignore
├── CONTRIBUTING.md
├── Makefile
├── SECURITY.md
├── requirements.txt
└── server.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## License

MIT. Do whatever you want.
