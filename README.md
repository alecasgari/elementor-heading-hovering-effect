# Elementor Heading Hover Effect with Text Highlight

This CSS code snippet provides a subtle and modern hover effect for heading links within Elementor. When you hover over the heading, a semi-transparent highlight smoothly expands across the text.

## Features

- Smoothly animated text highlight on hover.
- Customizable highlight color and opacity.
- Easy to integrate with Elementor's custom CSS.

## Demo

You can see a live demo of this button in action here: [https://leartme.com] and [https://www.blockchainlegals.com/]

## How to Use

1. **Add Custom Class:**

   - In the Elementor editor, select your heading widget.
   - In the "Advanced" tab, under "CSS Classes," add the class `heading-hover-effect`.

2. **Add the CSS:**

   - Go to your WordPress dashboard > Elementor > Custom CSS.
   - Paste the following CSS code:

```css
.heading-hover-effect a::before { /* Use ::before for highlight */
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  width: 0;
  height: 100%;
  background-color: #D5C7B7;
  opacity: 0.3; /* Adjust opacity as needed */
  transition: width 0.3s ease;
}

.heading-hover-effect a:hover::before {
  width: 100%;
}
```
**Note:** if you are using Elementor, add an Element like an icon or icon box then use custom css and an HTML widget

## Explanation
- The `::before pseudo-element` is used to create the highlight that sits on top of the text.
- `width: 0` initially hides the highlight.
- The `transition` property creates the smooth animation.
- On hover (`a:hover::before`), the `width` becomes `100%`, expanding the highlight across the text.
