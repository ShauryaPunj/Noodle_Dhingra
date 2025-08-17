# 🩷 *HTML Lists + Tables + Images* Crash Notes 

heyy coder bestie! ✨ this is your all-in-one, *cute but deep* revision doc for the lil project you made with lists, images, and tables. let’s snack-size the concepts so you can ace them anytime 🚀

---

## 🧩 What files you’ve got
- **lists.html** → shows off **unordered, ordered, and definition lists**. :contentReference[oaicite:0]{index=0}  
- **index.html** → page with an **image** + a **table** styled by CSS. :contentReference[oaicite:1]{index=1}  
- **style.css** → adds borders around table cells. :contentReference[oaicite:2]{index=2}  
- **Monster.png** → the pic used in the index page (monster energy drink).  

---

## 🏗️ Lists (lists.html = structure lab) :contentReference[oaicite:3]{index=3}
### 📍 Types
1. **Unordered list (`<ul>`)** → bullet points.  
   - `type="circle"` = hollow dots (can also be `"square"` or `"disc"`).  
2. **Ordered list (`<ol>`)** → numbered/lettered items.  
   - `type="I"` = uppercase Roman numerals.  
   - Other options: `"i"` (lowercase roman), `"A"` (uppercase alphabets), `"a"` (lowercase alphabets), default = numbers.  
3. **Definition list (`<dl>`)** → glossary-style.  
   - `<dt>` = the **term**, `<dd>` = the **definition**.  

### 🌈 Example mental map
```html
<ul type="circle">
  <li>Shaurya</li>
  <li>Shreya</li>
</ul>

<ol type="I">
  <li>Shaurya</li>
  <li>Shreya</li>
</ol>

<dl>
  <dt>Shaurya</dt>
  <dd>Hello I am Shaurya Punj learning web dev</dd>
</dl>


🖼️ Images (index.html = glow-up zone) 

Use <img> to show an image. Attributes:

src="Monster.png" → where the file lives.

alt="Monster Energy Drink" → fallback text if img fails.

width & height → control size (if you set one, the other adjusts automatically).

<br> = line break (forces content to the next line).

💡 Best practice: always include alt text (accessibility & SEO friendly).

📊 Tables (index.html = data palace) 

Table basics

<table> wraps the table.

<tr> = table row.

<th> = table header (bold, centered by default).

<td> = table data (normal cells).

Extra structure

<caption> → title above the table.

<thead> → header section.

<tbody> → body section.

<tfoot> → footer section.

Attributes (not used here but useful):

rowspan = cell stretches across multiple rows.

colspan = cell stretches across multiple columns.

🌈 Example mental map
<table>
  <caption>Siblings Info</caption>
  <thead>
    <tr><th>Name</th><th>Age</th></tr>
  </thead>
  <tbody>
    <tr><td>Shreya</td><td>23</td></tr>
    <tr><td>Shaurya</td><td>19</td></tr>
  </tbody>
  <tfoot>
    <tr><td>Rajni</td><td>Core</td></tr>
  </tfoot>
</table>

🎨 CSS (style.css = minimal chic) 
td {
  border: 2px solid black;
}


Applies to all <td> elements.

Gives each data cell a solid black border.

Pro tip: You can also style th or the whole table for cleaner looks (padding, collapse borders, background colors).

🛟 Debug snack-tips

If image not showing → check src path + file name (case matters).

If table looks plain → confirm style.css is linked in <head>.

If list symbols not changing → ensure correct type attribute.

Always validate HTML (missing </dl> can break layout).
