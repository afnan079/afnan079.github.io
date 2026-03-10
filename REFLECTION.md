# Reflection

## Q1: HTTP Path (Browser to HTML)

When you enter a URL in the browser, the browser first asks DNS to resolve the domain name to an IP address. Once it has the IP, the browser sends an HTTP request to that server. The server receives the request and responds by sending back the HTML (and other resources). The browser then renders the HTML to display the page.

## Q2: Docker vs GitHub Pages

Docker is a platform that runs applications inside containerized environments—lightweight, isolated runtimes that bundle an app with its dependencies and a slice of the OS. GitHub Pages is a static site hosting service that serves pre-built files (HTML, CSS, JS) from a repository; it does not run containers or servers you control.

Docker containers are strictly required to run GitHub Pages.

## AI Attribution

Code generated partially by Cursor AI. Logic error regarding Docker usage was manually corrected.

## Part 2 - Q1: Flexbox Direction

`flex-direction: row` lays items out horizontally from left to right (in left-to-right languages), while `flex-direction: column` stacks items vertically from top to bottom.

## Part 2 - Q2: Relative vs Fixed Units

Relative units like `%`, `vh`, and `rem` scale fluidly based on screen size or the root font size, allowing layouts and text to adapt to different devices, while fixed `px` values stay rigid and can cause content to overflow or be clipped on smaller screens.

## Part 2 - Q3: AI Attribution

Prompt used: "How do I make a 3-column grid?" The AI suggested using `grid-template-columns: 33% 33% 33%;`, but I modified it to `repeat(3, 1fr)` because fractional units handle the grid-gap math much better without overflowing the container.
