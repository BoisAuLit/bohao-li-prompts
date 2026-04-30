Create a clean, readable SVG architecture diagram.

Goal:
Help me understand how this file cluster works.
This is for one-time learning, not future editing.

Output rules:
- Output ONLY valid SVG.
- No markdown.
- No explanation.
- No foreignObject.
- No HTML.
- Use only: svg, defs, marker, rect, text, tspan, line, path.
- Must open directly in a browser.

Canvas:
- width: 1800
- height: 1200
- viewBox: 0 0 1800 1200
- white background

Visual style:
- Font: Arial
- Title: 30px bold
- Section labels: 18px bold
- Normal text: 14px
- Small notes: 12px
- Rectangles only
- No rounded corners
- Stroke width: 1.5
- Light colors only

Color legend:
- Entry point / main file: #DAE8FC
- Coordinator agent: #E1D5E7
- Subagents: #E1D5E7
- Tools / MCP: #D5E8D4
- Context: #FFE6CC
- State: #F8CECC
- Output / final result: #FFF2CC
- Notes: #F5F5F5

Diagram type:
Show a dependency + runtime-flow diagram for a multi-file AI agent system.

Required layout:
1. Top row: file dependency map
2. Middle row: runtime execution flow
3. Bottom row: context/state/data accumulation
4. Bottom-right: small legend

For each file:
- Show filename as the box title
- Show 3–5 most important responsibilities
- Show imports/dependencies with arrows
- Do NOT include low-level code details

For agent systems:
- Clearly separate:
  - user request
  - coordinator agent
  - wrapper tools
  - subagents
  - MCP tools
  - regular tools
  - runtime context
  - mutable state
  - final output

For each subagent:
Show:
- Agent name
- Main purpose
- Tools it uses
- Context fields it reads
- Whether it writes state

Text constraints:
- Max 6 lines per box
- Max 34 characters per line
- Split large concepts into smaller boxes
- Use <tspan> for line breaks
- Text must stay inside boxes
- No text overflow

Box constraints:
- Normal box width: 180–260
- Normal box height: 70–140
- Large container max width: 360
- Avoid empty space inside boxes
- No oversized rectangles

Arrow rules:
- Use straight lines or simple paths
- Define arrow marker in <defs>
- Label important arrows with short text
- No arrows crossing text
- No messy edge routing

Content extraction rules:
- First identify all files and their roles
- Then identify import dependencies
- Then identify runtime call flow
- Then identify context/state flow
- Then generate the SVG

Learning emphasis:
Make the diagram teach these ideas clearly:
- which file starts the system
- which file defines shared schemas
- which file creates MCP tools
- which file creates subagents
- how the coordinator delegates work
- how context is passed read-only
- how state is written over time
- how final output is assembled

Validation before output:
- Every box has readable text
- No text overflows
- No overlapping boxes
- No arrows through text
- Diagram fits in one page
- The main story is understandable in 10 seconds
