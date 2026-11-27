## Part B - DevTools Investigation

 # Elements Panel

Right-clicking on the DOrSU logo and clicking ‘Inspect’ opens up the Elements section of Chrome DevTools. This highlights the elements, which include the source (src), alternative text (alt), width, and height of the logo.

<img width="845" height="414" alt="b1-elements" src="https://github.com/user-attachments/assets/a87ad963-9ee3-47af-bc62-d1438e3ec47f" />

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

# Network Panel

<img width="857" height="411" alt="b3-network" src="https://github.com/user-attachments/assets/973e6cc7-ef22-4f22-a387-988fc5b56ee7" />

| What I checked | My finding |
| --- | --- |
| Request URL | https://dorsu.edu.ph/ |
| Request method | GET |
| Status code | 200 OK |
| Content-Type (response header) | text/html; charset=UTF-8 |
| Server (response header, if shown) | cloudflare |
| Total number of requests | 78 |
| Total data transferred | 2.5 MB |
| Load time (no throttling) | 2.25 s |
| Load time (Slow 4G) | 14.12 s |
| Largest file and its size | fa-solid-900.woff2, 80.8 kb |


Why does the page make so many requests, and what does the Slow 4G result tell you about users with weak signal here in Davao Oriental?

Various files (for example, HTML, CSS, JavaScript, images, and fonts) are requested by the DOrSU website so that a full website can be displayed. From my findings, I identified that 78 files were requested and 2.5MB of data was sent. With no throttling, the site loaded in 2.25 seconds. However, with Slow 4G, it took 14.12 seconds. Thus, students or staff in areas of Davao Oriental that have poor or inconsistent internet connections may face increased website loading times. Because of that, websites like DOrSU's should be optimised to improve loading speed and user experience.


