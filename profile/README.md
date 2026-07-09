# rustkit-ai

Open source developer tools for AI-assisted development, built in Rust.

We work on the parts of the workflow that still create friction when you code with an AI agent: keeping context across sessions, cutting the token cost of large tool outputs, and running semantic search locally instead of shipping your code to a cloud API.

[GitHub](https://github.com/rustkit-ai) · [rustkit.ai](https://rustkit.ai) · MIT

## What we build

**Memory and context.** Agents lose context between sessions. We build tools that give them persistent, structured memory that survives across conversations.

**Token efficiency.** Large tool outputs and code context eat into the model's budget. We build proxies and filters that trim the noise before it reaches the model.

**Local intelligence.** Embeddings and semantic search don't need a cloud API. We build on-device tooling that runs anywhere Rust runs.

## Projects

### [semtree](https://github.com/rustkit-ai/semtree)
Semantic code search for any codebase: tree-sitter parsing, local embeddings, and hybrid (vector + BM25) retrieval. Runs on-device, no API key.

```sh
cargo install semtree-cli
```

### [trimcp](https://github.com/rustkit-ai/trimcp)
An MCP proxy that compresses tool outputs before they reach the model, by stripping ANSI codes, minifying JSON, and deduplicating repeated lines. Works with any MCP client.

```sh
cargo install trimcp
```

### [tersify](https://github.com/rustkit-ai/tersify)
Strips noise from code and text before you send it to an LLM, so more fits in the context window. CLI or Rust library.

```sh
cargo install tersify
```

### [aimemo](https://github.com/rustkit-ai/aimemo)
Persistent memory for AI coding agents (Claude Code, Cursor, Windsurf, Copilot). One command to install.

```sh
cargo install aimemo
```

### [semstore](https://github.com/rustkit-ai/semstore)
Local semantic search as a library for Rust apps: store text, search by meaning, no cloud.

Everything is at [rustkit.ai](https://rustkit.ai).

## Contributing

Bug reports, feature ideas, code, docs, and feedback are all welcome. Each repo has its own contributing guide; open an issue or start a discussion.

## Team

<table>
<tr>
  <td align="center">
    <a href="https://github.com/Strawbang">
      <img src="https://github.com/Strawbang.png" width="72" /><br/><br/>
      <b>Djamel Bougouffa</b><br/>
      <sub>Co-founder, @Strawbang</sub>
    </a>
  </td>
  <td align="center">
    <a href="https://github.com/GokhanKabar">
      <img src="https://github.com/GokhanKabar.png" width="72" /><br/><br/>
      <b>Gokhan Kabar</b><br/>
      <sub>Co-founder, @GokhanKabar</sub>
    </a>
  </td>
</tr>
</table>
