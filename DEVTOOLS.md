## Part B - DevTools Investigation

 # Elements Panel
<img width="860" height="411" alt="b1-elements-1" src="https://github.com/user-attachments/assets/eb8b329a-2a52-4bbe-9b0f-af63a3461ec4" />


Right-clicking on the DOrSU logo and clicking ‘Inspect’ opens up the Elements section of Chrome DevTools. This highlighted the element, which includes the source (src), alternative text (alt), width, and height of the logo.

<img width="845" height="414" alt="b1-elements-2" src="https://github.com/user-attachments/assets/52ad13ed-5fbd-4a4e-bb93-d6e3b3de3422" />


I then looked for an editable text box. Upon double-clicking it, I typed in my full name and reloaded the web page to see what would happen.

The change disappeared after reloading the page because editing the HTML through Chrome DevTools only makes temporary changes in the browser and does not modify the original website files.

# Styles Panel
<img width="857" height="413" alt="b2-styles-1" src="https://github.com/user-attachments/assets/e78f824a-0dbb-4909-9aab-264a7ffed578" />


With an element selected, I found its color, font-family, and font-size in the Computed tab. Here are my findings:
- Color: rgb(255, 255, 255)
- Font-family: Poppins, sans-serif
- Font-size: 32px

<img width="859" height="413" alt="b2-styles-2" src="https://github.com/user-attachments/assets/04afe47e-b068-4091-8843-072e0a00beb7" />


Inside the Styles tab, I found some CSS properties crossed out.

That is because another CSS rule has higher priority or overrides it. I also changed the background color using the Styles panel and observed that the webpage's appearance changed immediately.

<img width="959" height="409" alt="b2-styles-3" src="https://github.com/user-attachments/assets/78d280b1-d8a8-4c46-8fd4-6aa3e6370db9" />

I also changed the element's background color.

