# What Happens When You Type google.com in Your Browser and Press Enter

When you type `google.com` in your browser and press Enter, a lot of processes happen almost instantly. Understanding these steps is crucial for Full-Stack Software Engineers, SREs, and anyone interested in how the web works.

---

## 1. DNS Request

Before your browser can contact Google, it needs to translate the human-readable domain `www.google.com` into an IP address. This process is called **DNS resolution**:

1. The browser first checks its **local cache**.
2. If not found, the operating system queries its **hosts file**.
3. If still unresolved, a request is sent to your **ISP's DNS server**.
4. Eventually, the request reaches a **root DNS server** and then a **Google authoritative DNS server**, which responds with the IP address of Google's web servers.

This IP address is used to locate the correct server on the internet.

---

## 2. TCP/IP Connection

Once the IP address is known, your browser initiates a **TCP connection**:

- TCP ensures reliable data transmission between your computer and Google’s server.
- A **3-way handshake** occurs: SYN → SYN-ACK → ACK.

This establishes a stable connection over which data can flow.

---

## 3. Firewall Check

Before reaching Google's servers, network traffic may pass through **firewalls**:

- Firewalls inspect traffic to block malicious requests.
- They ensure only legitimate requests (like HTTP/HTTPS traffic) are allowed.
- Both client-side (your computer) and server-side (Google's infrastructure) firewalls are involved.

---

## 4. HTTPS/SSL Handshake

Since the URL uses HTTPS, the browser performs an **SSL/TLS handshake**:

1. The browser verifies Google's SSL certificate to ensure authenticity.
2. Encryption keys are exchanged for secure communication.
3. A secure channel is established so that all data is encrypted in transit.

---

## 5. Load Balancer

Google has millions of users accessing their servers simultaneously. To handle this load:

- A **load balancer** distributes incoming requests across multiple servers.
- This ensures no single server is overwhelmed and improves response times.
- Load balancers can use strategies like round-robin or least-connections to balance traffic.

---

## 6. Web Server

The request then reaches a **web server**, which handles HTTP/HTTPS requests:

- It serves static content like HTML, CSS, and images.
- If the requested content requires processing, it forwards the request to an **application server**.

---

## 7. Application Server

The **application server** processes dynamic requests:

- Executes server-side logic (e.g., searching, personalization).
- Interacts with databases to fetch or update information.
- Generates HTML, JSON, or other responses for the browser.

---

## 8. Database

If the request requires data storage or retrieval:

- The application server queries a **database**.
- Databases store structured data like user profiles, search history, and content.
- The results are returned to the application server, which integrates them into the response.

---

## 9. Browser Rendering

Finally, the browser receives the response:

1. Parses HTML, CSS, and JavaScript.
2. Builds the **DOM (Document Object Model)**.
3. Renders the page visually and executes scripts.
4. The user sees the fully loaded `google.com` page.

---

## Conclusion

From DNS resolution to database queries, typing `https://www.google.com` triggers a complex chain of events. Full-Stack Engineers benefit from understanding this process to debug issues, optimize performance, and ensure security.

---

**Published on:** [Medium/LinkedIn link here]

