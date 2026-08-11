# `line-height` css property

The **`line-height`** CSS property **`defines the vertical space between lines of text`**. It sets the height of a "line box", which controls how tightly packed or spaced out your paragraphs appear.

Rather than pushing text down from the top like a margin, `line-height` distributes spacing **equally above and below** the letters on a line.

## Supported Values

You can define `line-height` using several different units:

| **Value Type** | **Example** | **Description* |
| --- | --- | --- |
| **Unitless Number** | `line-height: 1.5;` | **Recommended.** Multiplies the number by the element's current font size. |
| **Length** | `line-height: 24px;` | Sets a fixed, absolute distance regardless of the font size. |
| **Percentage** | `line-height: 150%;` | Sets the spacing relative to the current font size. |
| **Keyword** | `line-height: normal;` | Uses the browser default value, usually around `1.2.` |

## Why You Should Use Unitless Numbers

According to documentation on [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/line-height), using a **unitless number** is the best practice.

If you use percentages or fixed units like `em`, child elements inherit a hard, calculated pixel value from their parents. If a child element has a much larger font size, the text will overlap. A unitless number ensures that child elements inherit the multiplier instead, meaning the line height automatically scales up or down with the text size.

```css

/* Bad Practice (can cause text overlap in children) */
body {
  font-size: 16px;
  line-height: 24px;
}
/* Good Practice (scales dynamically across all elements) */
body {
  font-size: 16px;
  line-height: 1.5;
}
```

## Accessibility Tip

For body text and general reading paragraphs, the W3C Web Accessibility Guidelines recommend a minimum `line-height` of `1.5`. This provides enough separation to make text easier to read for individuals with dyslexia or low vision.
