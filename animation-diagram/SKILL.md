Create a single self-contained HTML file that renders a live-looking “Codex Agent Tree” dashboard in a dark terminal window. No external CSS or JS libraries. Everything must be inline.

Visual style:
- Full-page dark navy/black background (#0d1117).
- Fake macOS terminal chrome at the top: three traffic-light dots, title “~/agent-tree — zsh — 92x46”.
- Header bar: “CODEX AGENT TREE” left, “GPT-6.1 SOL WORKS” center, “ASTRA ON CALL” right, with small colored legend squares.
- Monospace font (ui-monospace, SF Mono, Menlo, Consolas).
- Soft box shadows, 1px borders, rounded corners ~6px, subtle grid or connecting lines drawn with CSS or inline SVG.

Layout (top to bottom):
1. Left sidebar panel (purple border) labeled “ASTRA · architect · on call”.
   - Status line that can be “before a plan”, “error repeats”, or “before done”.
   - Short notes: “spawned only at three moments”, “never writes code itself”, last advice, call count, tokens read.
2. Center top box (teal) for the main model: “GPT-6.1 Sol · main”, “plans + writes code”, effort bars, cost line “$2 / $10 per 1M”.
3. Middle green panel “JEV · fork layer” showing three quick decisions (which file / which tool / retry or stop) with confidence bars and a running fork count.
4. Three equal child cards in a row:
   - worker (gpt-6.1-sol) — edits + runs tests
   - explorer (gpt-6-luna) — reads the code
   - researcher (gpt-6-luna) — pulls the docs
   Each shows effort, status (running / done), and a small indicator.
5. Bottom teal box: “back to sol · review + verify” and “auto_review checks approvals”.
6. Session log strip at the very bottom with timestamped lines that look like they are appending.

Behavior:
- Use a small <script> to cycle statuses, increment fork count, tokens, and append 1–2 log lines every few seconds so it feels live.
- Color coding: purple = Astra, teal = Sol, green = Jev forks, blue = sub-agents.
- Keep all text crisp and aligned like a real ops dashboard, not a marketing page.

Content to show:
[PASTE YOUR AGENT ROLES, MODEL NAMES, AND STATUS MESSAGES HERE]

Output only the complete HTML file. No explanation.