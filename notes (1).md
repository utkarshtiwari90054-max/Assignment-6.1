# Assignment 6.1 - Box model notes

All three boxes have `width: 250px`, but they render at different sizes:

| Box | box-sizing | Padding | Border | Margin | Rendered width (content + padding + border) |
|-----|-----------|---------|--------|--------|------------------------|
| A | content-box | 20px | 5px | 10px | 250 + 40 + 10 = **300px** |
| B | content-box | 40px | 10px | 30px | 250 + 80 + 20 = **350px** |
| C | border-box | 30px | 8px | 20px | **250px** (content shrinks to 250 - 60 - 16 = 174px) |

**Difference:** with `content-box`, `width` sets only the content area, so padding and border make the box larger. With `border-box`, `width` includes padding and border, so the box stays 250px and the content area shrinks instead. Margin is outside the border in both cases and is never part of the width.

## Screenshot steps (to complete yourself)
1. Open `index.html` in Chrome, press F12, click the element picker and select Box A.
2. In the Computed tab (or the Styles pane) find the box model diagram: content in the centre, then padding, border and margin rings.
3. Hover the diagram to highlight each layer on the page, then take a screenshot (Chrome's "Capture node screenshot" or your OS tool).
4. Annotate it with arrows or text boxes labelling **content, padding, border, margin**, and repeat for Box C to show the border-box difference.
