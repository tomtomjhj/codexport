# codexport

`codexport` exports Codex session `.jsonl` logs to Markdown.

## Install

No installation is required. The script is directly executable:

```bash
./codexport --help
```

## Usage

Launch an interactive session selector (reads from `~/.codex/sessions`):

```bash
./codexport
```

The selector shows each session's creation/update timestamps (in local machine time),
cwd, git branch (if present), and first user prompt.

Default mode exports only chat messages:

```bash
./codexport /path/to/session.jsonl -o session.md
```

Export all records (`reasoning`, tool calls/outputs, events, turn contexts):

```bash
./codexport --all /path/to/session.jsonl -o session_full.md
```

Use a different session directory for selection:

```bash
./codexport --session-dir /path/to/sessions
```
