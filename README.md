# Contact Extractor with Click-to-Call Support

A smart contact extraction tool built for internal support teams to quickly extract and call leads or contact points from any website. This tool automatically pulls emails, mobile numbers, and landline numbers, stores them in a database, and enables click-to-call through the Knowlarity API — streamlining communication without manual copying or switching platforms.

Live Demo: [http://extractor.myclassboard.ai](http://extractor.myclassboard.ai)

---

## Project Purpose

This project was built as part of a company internship to assist the support team in:
- Quickly accessing verified contact information from educational websites
- Storing and managing these contacts in one place
- Providing a seamless Click-to-Call service for agents using Knowlarity

---

## Features

- Extract contact details (emails, mobile & landline numbers) from any website
- Detects & decodes obfuscated or cloudflare-protected email addresses
- Stores unique contact records in a MySQL database with deduplication
- Supports agent login, contact search, delete, and refresh operations
- Logs all agent click-to-call activities with timestamps
- Integrated with Knowlarity Click-to-Call API
- Simple and clean HTML-based UI

---

## Screenshot

![App UI Screenshot](https://github.com/Harshitha-hubb/contact_extractor/blob/main/assets/Screenshot%20.png)

---

## Tech Stack

| Layer               | Technology / Tool                          |
|---------------------|--------------------------------------------|
| **Frontend**        | HTML, CSS, Jinja2 Templates                |
| **Backend**         | Python, Flask                              |
| **Web Framework**   | Flask (routing, session management, etc.)  |
| **Data Extraction** | BeautifulSoup (for HTML parsing)           |
| **Regex Matching**  | Python `re` module                         |
| **HTTP Requests**   | `requests` library                         |
| **Database**        | MySQL                                      |
| **ORM/Connector**   | mysql-connector-python                     |
| **Deployment**      | Deployed to a cloud server (via IP/domain) |
| **External API**    | Knowlarity Click-to-Call API               |
| **Session Handling**| Flask `session` module                     |
| **Email Decoding**  | Cloudflare email protection handling       |
| **Logging**         | Contact refresh & call click logging       |
| **Search UI**       | HTML input filtering + Python filtering    |

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Harshitha-hubb/contact_extractor.git
cd contact_extractor
