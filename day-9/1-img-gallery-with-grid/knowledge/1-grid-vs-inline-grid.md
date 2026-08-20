# `display:grid` vs `display:inline-grid`

The primary difference between `display: grid` and `display: inline-grid` is **how the grid container itself interacts with surrounding elements on the page**. Inside the container, both behave exactly the same way and treat their direct children as grid items.

## Quick Comparison

| **Feature**                | **`display: grid`**                       | **`display: inline-grid`**                  |
| -------------------------- | ----------------------------------------- | ------------------------------------------- |
| **Container Type**         | Block-level element                       | Inline-level element                        |
| **Default Width**          | Takes up **100%** of the parent's width   | Shrinks to **fit the width of its content** |
| **Sibling Behavior**       | Forces a line break; sits on its own line | Sits on the same line next to text or spans |
| **Internal Grid Behavior** | Identical 2D row/column mechanics         | Identical 2D row/column mechanics           |

---

## Deep Dive

### `display: grid`

When you apply `display: grid`, the container acts like a `<div>` or a `<p>` tag.

- It takes up the full width available to it, even if the content inside is very small.
- It pushes any elements that come after it down to a new line.
- Use this for major layout structures like full-page setups, headers, footers, or multi-column content areas.

## `display: inline-grid`

When you apply `display: inline-grid`, the container acts like a `<span>` or an `<a>` tag.

- It only wraps tightly around its internal content rather than filling the screen horizontally.
- Other inline elements (like text, images, or buttons) can sit right next to it on the same line.
- Use this when you need a micro-layout inside a paragraph of text, or a small component like a custom pill badge with an icon and text aligned perfectly via a grid structure.
