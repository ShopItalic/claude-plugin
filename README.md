# Italic for Claude

Italic turns what you say into text: quick Clips and longer Memos from the Sudo ring, Glyph, Dex or the Italic apps. This plugin connects Claude to your Italic account, so you can search and recap your notes, save new ones, and review what your workflows drafted without leaving the conversation.

## What's inside

- **The Italic connector** (`.mcp.json`): Italic's MCP server at `https://app.italic.com/api/v1/mcp`. You sign in with your Italic account and choose what Claude may do.
- **Skills**: `italic` (how to search, save and edit well), `italic-recap` (decisions, to-dos and open questions from a day or a week of notes) and `italic-drafts` (review and approve what your workflows prepared).

## Use it

1. Add the plugin from Claude's directory, or in Claude Code run:

   ```
   /plugin install italic --marketplace ShopItalic/claude-plugin
   ```

   Then connect Italic from the plugin's **Connectors** tab, or with `/mcp` in Claude Code, and sign in.
2. Ask Claude, for example:
   - "What did I say about the Lisbon trip?"
   - "Recap my Italic notes from this week."
   - "Save these meeting notes to Italic."
   - "What drafts are waiting in Italic?"
   - "Open my Italic library."

You need an Italic account. Get the app at [italic.com](https://www.italic.com).

## Data

Claude sends Italic what each request needs, such as a search query or the text of a note to save, over HTTPS to `app.italic.com`. Italic returns your recordings' text, settings and workflow drafts, never audio. Approving a draft sends it through the account it was drafted for, such as your Gmail. The plugin itself is Markdown and JSON: it stores nothing and runs no code.

- Privacy policy: https://app.italic.com/privacy
- Terms: https://app.italic.com/terms
- Support: technology@italic.com
