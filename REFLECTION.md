# Reflection

1. Explain the difference between flex-direction: row and flex-direction: column.

flex-direction: row places items side-by-side horizontally, like words in a sentence (left to right). flex-direction: column stacks the items vertically one on top of the other, which is exactly what I used in my media query to make the navigation stack neatly on mobile screens.

2. Why is it important to use relative units (like %, vh, or rem) instead of fixed pixels (px) for
responsive design?

Fixed pixels (px) are completely rigid. If I make a container 800px wide, it will stay 800px even on a tiny iPhone screen, which causes ugly horizontal scrolling. Relative units like %, vh, or rem scale dynamically based on the screen size or the root font size, so the layout automatically shrinks or grows to fit whatever device the user is holding.

3. AI Attribution: List the prompt you used if you consulted GenAI. Identify one specific
piece of CSS code the AI provided that you had to modify to make it work for your layout.

Prompt used: "How do I align my logo to the left and nav links to the right using flexbox?"

CSS Modification: The AI generated the CSS for my navigation bar, but it put padding: 10px; specifically inside the nav a:hover rule. This was a bad piece of code because it made the links physically expand and shift the whole layout every time my mouse hovered over them. I had to manually modify the CSS by moving the padding to the base nav a rule, and then only change the background-color on hover so the transition was smooth without breaking the layout.