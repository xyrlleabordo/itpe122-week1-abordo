## Part A - Trace a URL

URL example:
https://www.dorsu.edu.ph

Command used: 

<img width="935" height="34" alt="Screenshot 2026-11-27 060016" src="https://github.com/user-attachments/assets/d2b6f158-437a-41cd-8d6c-035354f95ea1" />



Output:

<img width="959" height="321" alt="Screenshot 2026-11-27 060031" src="https://github.com/user-attachments/assets/9b704d3e-2731-40f7-9a35-cf6211600e63" />


## The Journey of a URL

There are six stages:
- The URL
- DNS Lookup
- Connection
- HTTP Request
- HTTP Response
- Rendering

1. The URL

I used the URL https://www.dorsu.edu.ph as an example. The protocol (https://) tells the browser how to communicate securely with the website, while the domain name (www.dorsu.edu.ph) identifies the website's address. The path (/) identifies the specific page or location being requested.

2. DNS Lookup

Computers communicate using IP addresses, so the browser needs to translate the domain name into an IP address before it can locate the website's server. The browser sends a DNS query to a DNS server, which looks up the domain name and returns its corresponding IP address. I used the nslookup command to find the IP addresses associated with www.dorsu.edu.ph.

3. Connection

After obtaining the IP address, the browser gets the site's IP address and then connects to the web server using TCP. If the site is secure, like those that use HTTPS, the browser also sets up a secure connection with TLS. This encrypts the data that goes back and forth between the browser and server, which helps keep your personal info safe.

4. HTTP Request

Once the connection is established, the browser sends an HTTP request to the web server to ask for the requested webpage. It uses the GET method, with the path / when requesting the DOrSU homepage, and includes headers that provide additional information about the request, which tells the server which resource the browser wants to access.

5. HTTP Response

The web server receives the HTTP request, processes it, and then sends back an HTTP response to the browser. The response will contain a status code, a set of headers, and the requested content (e.g., HTML, which is the structure of the page).

6. Rendering

Once the HTML document has been received, the browser gets to work rendering the page. It builds the DOM from the HTML, creates the CSSOM from the CSS, works out the layout of the elements (the layout phase), and then paints the page (the painting phase). It will also make further requests to get the CSS, JS, and images that are required to fully render the page.

# URL Trace Diagram
<img width="3816" height="2012" alt="trace-diagram" src="https://github.com/user-attachments/assets/ea22d6b2-8e2f-42d6-88d4-c2a44b3eed05" />

1. In your trace, which computer is the client and which is the server?

My computer using Google Chrome acts as a client, as it is issuing requests for data from the DOrSU web page. The server is the computer that is hosting the DOrSU website from the University itself. It accepts these requests and then replies to my browser by providing the relevant web page.


2. If the DNS lookup fails, what does the user see in the browser?

If the DNS lookup fails, then it will not know what IP Address the website has and will therefore be unable to connect. Instead, you will receive an error message: "This site can't be reached" or “DNS_PROBE_FINISHED_NXDOMAIN”.

3. What is the difference between status codes 200, 301 and 404? Give a real-life situation for each.

A status code of 200 means that the request was successful and the server returned the requested resource. For example, when I open the DOrSU homepage, a status code of 301 refers to a permanent relocation of a webpage. For example, if someone accesses an outdated webpage and is then automatically transferred to the updated page, a status code of 404 indicates that the server is unable to locate the required information. For example, if I attempt to access a DOrSU webpage but input, or there is, an incorrect/ non-existent web address.
