# MCP Server Development Flow

Build Model Context Protocol (MCP) servers to extend AI capabilities.

---

## Step 1: Plan the Server

**Human**: Identify what tools/resources you want to expose to AI.

Think about:
- What APIs or software does the AI need to interact with?
- What actions should the AI be able to perform?
- What data should the AI be able to read?

---

## Step 2: Generate the Server

(Prompt)
```
Implement an MCP server about <software/service>.
- use fastmcp
- use uv to manage dependencies
- include tools for <list of actions>
- include resources for <list of data sources>
```

---

## Step 3: Configure and Test

**Human**: Add the server to your MCP configuration.

(Prompt)
```
Generate a config.toml for this MCP server.
Include:
- server name and description
- connection settings
- any required API keys as environment variables
```

---

## Step 4: Iterate

(Prompt)
```
Add a new tool to the MCP server:
- name: <tool-name>
- description: <what it does>
- parameters: <inputs>
- returns: <output format>
```

---

## Example: Browser Extension MCP

```
Build an MCP server that lets AI control a web browser.
- use fastmcp
- tools: navigate, click, type, screenshot, get page content
- use playwright for browser automation
```

---

## Example: File System MCP

```
Build an MCP server for advanced file operations.
- use fastmcp
- tools: search files, batch rename, find duplicates, organize by date
- resources: file metadata, directory trees
```

---

## Tips

- Start with 2-3 essential tools, expand as needed
- Write clear tool descriptions for better AI usage
- Include error handling in your tools
- Test tools with various edge cases
