## Strict Design Requirements for the drawio diagram

### 1. Layout & Structure

- Use a clean left-to-right + top-to-bottom flow.
- Split content into multiple small boxes instead of large text blocks.
- Avoid wide rectangles with lots of empty space.
- Each box should tightly fit its text with minimal right/bottom whitespace.
- Long content **must** be split into multiple nodes.

### 2. Text Rules

- Keep each node to about 5–8 lines max.
- Use short lines and avoid long sentences.
- Prefer bullet points or numbered lists.
- Never allow text to overflow outside shapes.
- Do not rely on HTML tricks.
- Do not use div padding hacks.

### 3. Spacing & Padding

Use draw.io native spacing only:

```
spacing=4;spacingTop=4;spacingLeft=4;spacingRight=4;spacingBottom=4;
```

- Do not use `overflow=fill`.
- Do not use HTML padding.

### 4. Font & Readability

Use these font sizes:

- Title: `26`
- Section: `18`
- Normal: `13–14`

Use simple formatting:

- Bold for titles.
- Minimal color usage.
- Only highlight keywords.

### 5. Shapes

- Use rectangular boxes only.
- Do not use rounded corners.
- Use consistent sizes for similar nodes.
- Avoid oversized containers.

### 6. Arrows

- Prefer straight or slightly diagonal edges.
- Avoid unnecessary orthogonal arrows.
- Ensure arrows do not cross text.

### 7. Colors

Use clean, minimal colors:

- User: light orange
- Claude: light purple
- Tool: light green
- State: light red
- Notes: light gray

### 8. Critical Rule

The diagram must look visually balanced:

- No large empty space inside boxes.
- No text overflow.
- No giant blocks with tiny text.

If a block becomes too big, split it.

---

## Content Requirements

Visualize an LLM agent loop with:

1. User query
2. Messages state
3. API calls
4. `tool_use`
5. Tool execution
6. `tool_results`
7. Final answer

Show at least 3 rounds:

```
search → extract → final
```

---

## Output Format

- Output only valid draw.io XML.
- No explanation.
- Must be directly importable into draw.io.

---

## Quality Check Before Output

Ask yourself:

- Are any boxes too big? If yes, split them.
- Is there empty space? If yes, reduce width/height.
- Is there any overflow? If yes, fix immediately.

Only output when all checks pass.
