# Must-Know Terminology for Web Penetration Testers

## Basic Web Penetration Testing Terminology
- **HTTP (Hypertext Transfer Protocol)**: The protocol used for communication between a client (browser) and a web server. It defines how messages are formatted and transmitted.
- **HTTPS (Hypertext Transfer Protocol Secure)**: The secure version of HTTP, using SSL/TLS encryption to protect the integrity and confidentiality of data transmitted between the client and the server.
- **URL (Uniform Resource Locator)**: The address used to access resources on the web, consisting of the protocol (e.g., `http`), domain (e.g., `example.com`), and path (e.g., `/index.html`).
- **HTML (Hypertext Markup Language)**: The standard language used to create and structure web pages, consisting of elements like `<div>`, `<p>`, and `<a>`.
- **JavaScript**: A programming language used to add interactivity to web pages, commonly for client-side scripting.
- **Cookies**: Small pieces of data stored on the client side, often used to remember user preferences, sessions, and authentication states.
- **Sessions**: A server-side concept used to store data about the user's interaction with a website. Sessions often use cookies (like session IDs) to maintain state between requests.
- **Cross-Site Scripting (XSS)**: A vulnerability that allows an attacker to inject malicious JavaScript into a web application, which is executed by a victim's browser.
- **Cross-Site Request Forgery (CSRF)**: A vulnerability that forces an authenticated user to perform unwanted actions on a website without their consent.
- **SQL Injection**: A type of injection attack that allows an attacker to execute arbitrary SQL queries in a web application's database.
- **Directory Traversal**: A vulnerability that allows an attacker to access files and directories outside the intended directory on a web server, potentially exposing sensitive information.
- **File Upload Vulnerabilities**: Flaws in the handling of file uploads, often leading to arbitrary file uploads or remote code execution.

## Common HTTP Headers
- **Host**: Specifies the domain name of the server, allowing multiple websites to share a single IP address.
- **User-Agent**: Contains information about the client (browser or device) making the request, used to identify the client type.
- **Content-Type**: Specifies the media type (e.g., `text/html`, `application/json`) of the content being sent in a request or response.
- **Content-Length**: Indicates the size (in bytes) of the body of the request or response.
- **Authorization**: Contains credentials for HTTP authentication (e.g., `Bearer token`, `Basic` authentication).
- **Accept**: Specifies the types of content that the client is willing to receive from the server (e.g., `text/html`, `application/json`).
- **Set-Cookie**: Used by the server to send cookies to the client for storing session information or preferences.
- **Cache-Control**: Directs caching behavior (e.g., `no-store`, `max-age=0`), specifying whether content should be cached and for how long.
- **Referer**: The URL of the page making the request, allowing the server to track where requests are coming from.
- **X-Content-Type-Options**: A security header that prevents MIME type sniffing, which could lead to malicious content execution.
- **X-Frame-Options**: Prevents a web page from being embedded in an iframe, mitigating clickjacking attacks.
- **Strict-Transport-Security (HSTS)**: A security header that instructs the browser to only communicate with the server over HTTPS, preventing downgrade attacks.
- **Content-Security-Policy (CSP)**: A header that controls what resources the browser is allowed to load, mitigating attacks like XSS and data injection.

## Intermediate Web Penetration Testing Terminology
- **Web Application Firewall (WAF)**: A security system designed to filter and monitor HTTP traffic between a client and a web server, often used to detect and block malicious requests.
- **Rate Limiting**: A technique used to limit the number of requests a client can make to a web server in a given time period to prevent brute force attacks.
- **Parameter Pollution**: An attack where an attacker manipulates URL parameters to inject malicious data, potentially leading to information leakage or unexpected behavior.
- **Path Traversal**: A vulnerability that allows an attacker to access directories and files that are outside the web root directory, often resulting in sensitive file exposure.
- **HTTP Response Splitting**: A vulnerability that allows an attacker to inject headers into the HTTP response, potentially leading to cache poisoning or web cache injection attacks.
- **Clickjacking**: A malicious technique that tricks a user into clicking on something different from what they think they're clicking, potentially leading to unintended actions.
- **Content Injection**: An attack where malicious content (such as scripts or HTML) is injected into a web page, often through user input forms or URL manipulation.
- **Hidden Fields Manipulation**: A technique used by attackers to tamper with hidden form fields, which are often used for session management or tracking, to bypass authentication or inject malicious data.
- **Subdomain Takeover**: An attack where an attacker claims an unused or unclaimed subdomain (e.g., `test.example.com`) and gains control of it, often exploiting unconfigured DNS records.
- **HSTS (HTTP Strict Transport Security)**: A mechanism that forces web browsers to only connect to a website over HTTPS, enhancing security by preventing downgrade attacks and cookie hijacking.

## Advanced Web Penetration Testing Terminology
- **Session Fixation**: An attack where the attacker sets a user's session ID before the user logs in, allowing the attacker to take over the user's session after they authenticate.
- **XML External Entity (XXE) Injection**: A vulnerability that allows an attacker to inject malicious XML code that references external entities, often leading to sensitive data exposure or server-side request forgery (SSRF).
- **Server-Side Request Forgery (SSRF)**: An attack where an attacker is able to send arbitrary HTTP requests from a vulnerable server to internal or external resources, often exploiting misconfigured systems.
- **Insecure Deserialization**: A vulnerability that occurs when an attacker is able to manipulate or inject malicious objects into a deserialized input stream, often leading to remote code execution.
- **Blind SQL Injection**: A type of SQL injection where an attacker is unable to see the results of the injected query but can infer data based on server responses (e.g., timing attacks or boolean-based logic).
- **Reflected XSS**: A type of cross-site scripting where malicious input is reflected off a web server, usually via URL parameters, and executed in a user's browser.
- **Stored XSS**: A type of cross-site scripting where malicious input is stored in the server (e.g., in a database) and executed when the content is viewed by other users.
- **WebSocket Hijacking**: An attack targeting WebSocket connections by stealing or hijacking active WebSocket sessions, often leading to privilege escalation or unauthorized access.
- **OAuth 2.0 Flows**: OAuth is a widely-used protocol for authorization. Understanding its flows (authorization code flow, implicit flow, and client credentials flow) is essential for testing web applications that use third-party authentication services.
- **Open Redirect**: A vulnerability where an attacker can manipulate a URL to redirect a victim to a malicious site, often used in phishing attacks.
- **Cross-Site WebSocket Hijacking (CSWH)**: An attack that leverages WebSocket vulnerabilities to hijack an active connection, allowing an attacker to inject malicious data into ongoing communication.

## Web Application Penetration Testing Tools & Techniques
- **Burp Suite**: A powerful tool for web application security testing that includes functionality for intercepting HTTP traffic, scanning for vulnerabilities, and automating attacks.
- **OWASP ZAP (Zed Attack Proxy)**: An open-source security testing tool that helps identify vulnerabilities in web applications by proxying HTTP traffic and running automated scans.
- **Nikto**: A web server scanner that detects a variety of vulnerabilities, including outdated software, security misconfigurations, and potential issues with server configurations.
- **SQLmap**: An automated tool for detecting and exploiting SQL injection flaws in web applications.
- **Dirbuster/Dirb**: Tools used for brute-forcing directories and files on a web server to discover hidden resources.
- **Gobuster**: A tool for directory and DNS subdomain brute-forcing that can be used to discover hidden directories or vulnerable subdomains in a web application.

## Advanced Security Headers
- **X-XSS-Protection**: A browser-based header that provides protection against reflected XSS attacks by blocking the rendering of the malicious content.
- **X-Content-Type-Options**: A security header that prevents browsers from interpreting files as a different MIME type (to avoid attacks like drive-by downloads).
- **Strict-Transport-Security (HSTS)**: Instructs browsers to only communicate with the server over HTTPS, preventing downgrade attacks.

