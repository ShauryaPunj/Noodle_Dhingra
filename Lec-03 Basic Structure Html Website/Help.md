# 🩷 *Mini Site* Crash Notes 

hey bestie! ✨ here’s your speedy, aesthetic, brain-friendly guide to this lil web project. skim it once, ace it forever. let’s gooo 🚀

---

## 🧩 What’s in the folder?
- **index.html** → the skeleton (structure of the page). It sets the title, pulls in CSS + JS, and prints “Hola Amigos!” on the page.  
- **style.css** → the glam squad (how it looks). It paints the whole page **aqua**.  
- **script.js** → the brain (how it behaves). It pops a welcome **alert** when the page loads.  

---

## 🧠 Big picture (HTML → CSS → JS)
1) Browser reads **HTML** to build the DOM (your page’s structure).  
2) It loads **CSS** and applies styles (colors, spacing, vibe).  
3) It runs **JS** to add behavior (alerts, clicks, actions).  

End result: a page titled **“Shaurya Punj”**, with an aqua background, that says **Hola Amigos!** and shows a welcome pop-up.  

---

## 🏗️ index.html (the structure)
**What it does**
- Declares the doc type and language.  
- Sets metadata (charset + mobile viewport), page **title**, links **style.css**, and loads **script.js**.  
- Puts the text **Hola Amigos!** in the `<body>`.  

**Why it’s placed like this**
- CSS is in the `<head>` so styles apply ASAP. JS is just before `</body>` so the DOM exists before scripts run (no null element drama).  

**Mini template mental model**
```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Page Title</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    Hola Amigos!
    <script src="script.js"></script>
  </body>
</html>
🎨 style.css (the glow-up)

One global rule: body { background-color: aqua; } → paints the entire page background aqua. It’s simple but powerful because body wraps the whole visible page.

Try swaps

background-color: pink; for soft vibes

background-color: #111; color: white; for dark mode

⚡ script.js (the sparkle)

Runs an alert as soon as the script loads: “Hello welcome to shaurya punj website”. This shows a modal popup in the browser.

Level-up ideas

// replace alert with a friendlier inline message:
document.body.insertAdjacentHTML("afterbegin", "<p>Welcome, legend ✨</p>");

// add an interactive button:
const btn = document.createElement("button");
btn.textContent = "Click me!";
btn.addEventListener("click", () => alert("you’re awesome 😎"));
document.body.appendChild(btn);

🔗 How files connect (super key)

<link rel="stylesheet" href="style.css"> tells HTML to pull styles from style.css. (Path must be correct!)

<script src="script.js"></script> tells HTML to run JS from script.js after the page content.

If file names or paths don’t match, styles/JS won’t load — double-check spelling + location.

🧪 Quick practice (5-min glow-ups)

Change the page title in index.html to your vibe.

Swap the background color in style.css.

Update the welcome text in script.js or replace the alert with a cute inline message.

Add an emoji to Hola Amigos! (e.g., “Hola Amigos! 🥑”).

🧠 Tiny glossary (zero-stress)

Element: an HTML building block like <body> or <title>.

Attribute: extra info inside a tag (e.g., href="style.css").

DOM: live, in-memory tree of your HTML that JS can change.

Selector: the part in CSS that chooses what to style (body { ... }).

🛟 Debug like a pro (snackable)

If styles don’t show: confirm the <link> path + check DevTools “Sources”.

If JS doesn’t run: confirm the <script src> path + peek at the Console for errors.

If text doesn’t update: refresh with cache bypass (Ctrl/Cmd+Shift+R).