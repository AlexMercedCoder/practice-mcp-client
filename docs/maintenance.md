# Practice MCP client maintenance tracker

Audited 2026-11-24 against checkout `7c443b2`. Compared the quickstart instructions to this checkout’s origin and CLI.

Claim a row by entering your name or task ID and setting the status to **In progress**. Use **Blocked** with the missing dependency if needed. Set **Done** after the acceptance check passes and record the fix commit or PR, the command or manual check, and its result. If a newer revision already resolves the item, record that evidence and close it. Keep status in this table.

| ID | Priority | Status | Owner | Fix and verification |
| --- | --- | --- | --- | --- |
| PMCP-01 | P2 | Done | — | `ee440df`. Installed the declared requirements in a fresh Python 3.11 environment and launched the CLI from a clean Git snapshot. It reached the expected configuration check. |

### PMCP-01 · Point the quickstart at the code the reader is following

**Source comparison.** The clone command in `readme.md` sends readers to `AlexMercedCoder/langchain-mcp-client`. This repository is `AlexMercedCoder/practice-mcp-client` and its `client.py` uses a different agent factory.

**Acceptance check.** Correct the clone URL and directory. Walk the quickstart from a disposable checkout through dependency installation and the first configuration check. Verify referenced example files exist here.
