## Part B - DevTools Investigation

 # Elements Panel

Right-clicking on the DOrSU logo and clicking ‘Inspect’ opens up the Elements section of Chrome DevTools. This highlighted the element, which includes the source (src), alternative text (alt), width, and height of the logo.

<img width="845" height="414" alt="b1-elements-2" src="https://github.com/user-attachments/assets/52ad13ed-5fbd-4a4e-bb93-d6e3b3de3422" />

I then looked for an editable text box. Upon double-clicking it, I typed in my full name and reloaded the web page to see what would happen.

The change disappeared after reloading the page because editing the HTML through Chrome DevTools only makes temporary changes in the browser and does not modify the original website files.

# Styles Panel

With an element selected, I found its color, font-family, and font-size in the Computed tab. Here are my findings:
- Color: rgb(255, 255, 255)
- Font-family: Poppins, sans-serif
- Font-size: 32px

Inside the Styles tab, I found some CSS properties crossed out.

That is because another CSS rule has higher priority or overrides it.

<img width="959" height="409" alt="b2-styles" src="https://github.com/user-attachments/assets/4a8ff5c2-5cb0-4685-9af8-16f2dc8be185" />

I also changed the background color using the Styles panel and observed that the webpage's appearance changed immediately.


