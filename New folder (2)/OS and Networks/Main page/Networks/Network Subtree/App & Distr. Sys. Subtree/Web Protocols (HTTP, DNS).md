# 🕸️ Web Protocols (HTTP, DNS)

### 🎯 Core Focus & Definition
Web Protocols (HTTP, DNS) establishes the application layer standards for content delivery and resource location across the internet. This component acts as the user-facing interface of the stack, mapping human-readable domain names to logical IP vectors via DNS and handling hypermedia document transactions through HTTP state frameworks.

---

### 📌 INTRODUCTION & OVERVIEW
If lower protocol layers form the physical highways and routing maps of the internet, Web Protocols act as the vehicles and addresses that normal users interact with. This leaf covers two critical engines: the **Domain Name System (DNS)**, which operates as a globally distributed database that translates human-friendly domains into raw machine-routable IP strings, and the **Hypertext Transfer Protocol (HTTP)**, which defines how modern browsers request, pull, and stream web assets from distant cloud infrastructures.

---

### ⏳ HISTORICAL CONTEXT & EVOLUTION
* **The Static Text Roots (1990s):** Early internet queries relied on a single master `HOSTS.TXT` file compiled manually to trace machine locations, while early HTTP/1.0 opened a brand-new TCP socket for every single image or text file requested, causing massive network delays and protocol overhead.
* **The Scalable Multiplexed Era:** To handle billions of active web users, DNS evolved into a massive hierarchical caching tree (Root -> TLD -> Authoritative). Simultaneously, HTTP completely replaced its connection model: migrating to HTTP/2 to send multiple files at the same time over a single TCP connection, and eventually introducing **HTTP/3**, which swaps out TCP entirely for the UDP-based **QUIC** protocol to eliminate line-of-blocking delays on volatile mobile links.

---

### 🔗 INTER-DISCIPLINARY RELATIONS & CONNECTIONS
* **Dependencies (What this specific area needs):**
  * *Network & Transport Layers:* Wholly reliant on UDP port 53 for fast DNS lookups and persistent TCP port 443 / QUIC lines to carry data streams without loss.
* **Influences (What this specific area powers):**
  * *Software Engineering:* Dictates how modern APIs, web applications, and browser security layers are designed, establishing strict parameters around data caching and state rules.

---

### 🧠 STRATEGIC PROBLEMS & OPEN CHALLENGES
* **Important Classic Problems:**
  * **The DNS Cache Poisoning Flaw:** A famous security weakness where an attacker injects fake IP routing details into a local internet provider's DNS memory cache, quietly sending thousands of normal users to malicious spoofed clone sites.
* **Open Contemporary Problems:**
  * **Deploying Encrypted DNS at Planetary Scale:** Implementing **DoH (DNS over HTTPS)** and DoT to encrypt name lookups globally, blocking network providers from spying on user browsing history, while balancing corporate network visibility needs.

---

### 👑 KEY FIGURES & PREMIER VENUES
* **Important Pioneers:**
  * **Paul Mockapetris:** Invented the Domain Name System (DNS) architecture in 1983, creating the hierarchical lookup system that allowed the internet to expand.
* **Important Venues (Conferences & Journals):**
  * *IETF HTTPBIS Working Group:* The international standards body that continuously reviews, updates, and publishes the official engineering rules for HTTP.

---

### 🌐 THE DOMAIN DIMENSIONS
* **Global Perspective:** These application protocols form the primary communication engine of global industry. Every cloud transaction, electronic payment, smartphone application update, and streaming system relies on DNS and HTTP to resolve addresses and move files across borders.
---

## 🌲 SYSTEM INTERFACE SELECTOR

> [!NOTE] Architecture Leaf Node
> "This leaf marks the deepest conceptual layer for Web Protocols (HTTP, DNS). Navigate back to parent nodes to explore other sub-systems."

* Return to: [[Application Layer & Distributed Systems]]
* Return to: [[Networks]]

---