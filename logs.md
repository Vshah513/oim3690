# Class Logs

Log what you did each class below. Add a new entry for each session.

---

## Class 1 — [Date]

*What we did:*

*What I learnt:*

*Notes:*

---

## Class 2 — [Date]

*What we did:*
We set up the repo with a README that had the course title, my name, when and where the class meets, and links. I created this logs file so I could write down what we do each week.

*What I learnt:*
I learnt how to organise a GitHub repo for a web class so someone can land on it and know what the project is. Using Markdown for the README and for this log made it easy to add headings and links without writing HTML.

*Notes:* Repo is ready. Next step was building the actual course page.

---

## Class 3 — [Date]

*What we did:*
We redesigned the course page so it had a proper nav bar at the top, a hero section, a profile card, sections for assignments and the weekly log, a resources bit, and a footer. We added a dark mode toggle so you can switch themes. We looked at babson.edu to get ideas for layout and structure and I saved a copy of their HTML as babson.html so I could look at the markup offline. I put my profile photo in an images folder and hooked it up to the profile card. We ran the site locally with a Python server to test everything before pushing.

*What I learnt:*
I learnt how to break a page into sections (nav, hero, cards, footer) and build it in HTML and CSS. Looking at a real site like Babson’s helped me see how they use the same building blocks. Keeping images in a folder and linking to them from the page made sense. Using a local server meant I could refresh and see changes straight away instead of opening the HTML file directly.

*Notes:* The page felt like a real course site after this. I kept babson.html for later when we did more markup stuff.

---

## Class 6 — [Date]

*What we did:*
We looked at the “better” way to mark up a site header: using `<header>`, `<h1>`, and `<nav>` with a link inside instead of just divs. The slides showed why that’s better (clear structure, screen readers understand it, proper heading hierarchy).

*What I learnt:*
I learnt that semantic HTML isn’t just for looks. Using `<header>` and `<nav>` gives the page a real structure that assistive tech can use, and having one `<h1>` for the site title sets up the document outline properly. In my demo file I put the exact code from the slides and then added a live example so you can see the same structure on the page. I also wrote a short bit explaining the three benefits so the instructor can see what I took away.

*Notes:* s06-demo.html has the header/nav snippet, the “what’s better” list, and a small live demo box. Everything links back to course.html.

---

## Class 7 — [Date]

*What we did:*
We went through basic HTML elements: headings h1 to h6, paragraphs, line breaks, horizontal rules, text formatting (strong, bold, em, italic, underline), unordered and ordered lists including nested lists, links (external, internal, new tab), images with src and alt, buttons, divs as containers, span for inline styling, and footer. The class had a full example page with all of these.

*What I learnt:*
I learnt how each of these tags is used and when to pick one over another (e.g. strong vs b for importance). For the demo I recreated the same content from the slides but styled it to match our course theme so it doesn’t look like a plain HTML dump. I used a placeholder for the image so it works without the cat photo. The page is basically the class example but cleaned up and with the same nav and back link as the other demos.

*Notes:* s07-demo.html. All the elements from the slides are there so the instructor can see we covered them.

---

## Class 8 — [Date]

*What we did:*
We connected CSS to the page in two ways: an external stylesheet with `<link rel="stylesheet" href="/css/styles.css" />` and an inline `<style>` block. We also had a demo page with a heading, paragraphs, a link to Babson, the campus image, another section with more text and an image, and a list of links. The order of the stylesheet and the style tag mattered for what overrides what.

*What I learnt:*
I learnt that the browser applies CSS in order, so if you put the external file after the inline style, the external rules can override. I also learnt to use rel="noreferrer" when opening links in a new tab. In the demo I fixed the alt text typo, used placeholder images where we didn’t have the file, and linked to our real pages (course.html etc). I added a “what we learnt” section about external vs inline CSS and a best practice note about preferring one main stylesheet and only using inline for overrides.

*Notes:* s08-demo.html. The live demo shows the same content as class but with our styling and a takeaways box at the bottom.

---

## Class 9 — [Date]

*What we did:*
We added Google Fonts with preconnect and the font link (Libertinus Keyboard and Oswald), and we used inline styles for h1 and p. In the HTML we used classes like yellow and id like second-paragraph, and we had an element with two classes (julissa yellow). So we were mixing element selectors, class selectors, and id selectors.

*What I learnt:*
I learnt that preconnect speeds up font loading because the browser sets up the connection early, and display=swap means the text shows right away with a fallback font and then swaps when the custom font loads. I learnt that a class can be on many elements but an id should be unique on the page, and that you can put multiple classes on one element and then target them together in CSS with something like .julissa.yellow. In the demo I loaded the same fonts and built a live box that uses the same HTML from class so you can see the colours and the effect of the second class. I wrote a short summary of what we learnt so it’s clear for the instructor.

*Notes:* s09-demo.html. The live demo uses the same structure as the class code with both fonts applied.

---

## Class 10 — [Date]

*What we did:*
We kept the same kind of page but wrapped the content in a container div and then put each block inside a card div. So we had two cards side by side (or stacked on small screens). We also had a button, a span with class highlight for inline emphasis, and we looked at the order of the style block vs the external CSS file (s10-styles.css). There was a commented-out !important in the h1 rule.

*What I learnt:*
I learnt that container and card is a common pattern for laying out content in sections. I learnt that the order of your stylesheets matters for the cascade and that !important forces a rule to win but you shouldn’t overuse it. I also fixed the HTML in the list where the span was closed after the li (wrong order) so the markup is valid. In the demo I styled the container as a grid and the cards as panels so you can see the layout. I added a takeaways section about cascade, !important, container and cards, span, and button, plus a note about the correct way to wrap the link in the span.

*Notes:* s10-demo.html. The first card has the button and the highlight span; the second has the other section. Links go to course.html and the placeholders.

---

## Class 11 — [Date]

*What we did:*
Same page structure as class 10 but we added a second class to the first card: class="card my-element". So one card had both card and my-element, and the other card had just card. We loaded s11-styles.css so the extra class could add its own styling or be used as a hook.

*What I learnt:*
I learnt that you can give an element more than one class and then style it with .card, .my-element, or .card.my-element (only when both are present). That’s useful for a base style (card) plus a modifier (my-element) so some cards look different without changing the HTML structure. I also thought about using classes like my-element as JavaScript hooks so you can target them with querySelector. In the demo I made the first card have an accent border so you can see the effect of the modifier class. I wrote a short bit about base plus modifier and about keeping session-specific styles in their own file like s11-styles.css.

*Notes:* s11-demo.html. Only the first card has the my-element class so the difference is obvious.

---

## Class 11 — Flexbox [Date]

*What we did:*
We did a flexbox learning demo with nine small examples: row direction (default), column direction, justify-content space-between, justify-content center, align-items center with a min-height, flex wrap with fixed-width items, flex grow (one item with flex 2 and the rest flex 1), the gap property, and perfect centering (justify and align center on the container with one item inside).

*What I learnt:*
I learnt that flex-direction sets the main axis (row or column), justify-content moves stuff along that axis (center, space-between, etc), and align-items moves stuff on the cross axis. I learnt that flex-wrap lets items go to the next line when there’s not enough space and that flex: 1 and flex: 2 let items share space in proportion. Gap is nicer than adding margin to every item. For the demo I put all nine sections into one page with the same nav and back link as the other demos, and I styled the flex containers and items with our course colours so it fits the site. I added a short intro and a “what we learnt” section at the bottom so the instructor can see the main ideas. We named this one s11-flex-demo.html and put it on the course page instead of a separate session 12 card.

*Notes:* s11-flex-demo.html. Run locally with npm start and open localhost:3690/s11-flex-demo.html.

---

## Class 11 — Tables [Date]

*What we did:*
We built a student roster table with thead (ID, Name, Major, GPA, Year), tbody, and five rows of data. The table had border="1" in the HTML.

*What I learnt:*
I learnt that table, thead, tbody, tr, th, and td are the right way to mark up tabular data. I learnt that th is for header cells and you can add scope="col" so screen readers know it’s a column header. I learnt that caption gives the table a title and helps with accessibility. In the demo I removed the border attribute and did all the borders and spacing in CSS so we have proper control. I added a caption and scope on the ths and a “what we learnt” section about each tag. I also added a note that tables are for data not for page layout and that you should use CSS for styling instead of the border attribute. We named this s11-table-demo.html and linked it from the course page instead of the session 13 card.

*Notes:* s11-table-demo.html. Same roster data as class, styled to match the rest of the demos.

---

## Repo cleanup — [Date]

*What we did:*
We removed everything that was portfolio-related from the oim3690 repo. The repo is only for course work and session demos now, not for a personal portfolio site.

*What I learnt:*
I replaced the old index.html (which was the full portfolio page with hero, projects, skills, contact) with a simple home page that just says OIM3690 and has a button linking to course.html. I deleted the portfolio redesign summary doc. I updated the README so it describes the repo as course work and session demos only and lists the demo files. I changed course.html so the nav says “Home” instead of “Back to Portfolio” and the footer links to index.html as Home. In the session demos (s07 through s11) every link that said “Homepage” or “link to another page” and pointed to index.html now points to course.html so the course work page is the main place to go. I kept babson.html since it’s from a class exercise. Running the site locally is still npm start on port 3690; the root URL shows the new simple home and you can go to course work from there or open any demo directly.

*Notes:* No portfolio content left in this repo. index.html is just a landing page that links to course.html.

---

*Add more entries below as the course continues.*
