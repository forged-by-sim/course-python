🌐 Module 4 — Chapter 12
Programs That Surf the Web

Course: Python for Everybody – Course 3
Platform: Coursera
Completed: ✅ June 2025
Directory: module4-ch12-programs-that-surf-the-web

This module introduces foundational web-scraping and web-navigation techniques using Python. The assignments reinforce how to retrieve data from live webpages, parse HTML structures, extract meaningful information, and process linked data.

Across the two assignments, I used urllib, BeautifulSoup, and structured data files (HTML, XML, JSON) to build programs that interact with the web programmatically.

⸻

📚 Module Contents

module4-ch12-programs-that-surf-the-web/
│
├── following-links-in-HTML-using-beautifulsoup/
│     ├── README.md
│     ├── Following Links in Python_Instructions1.png
│     ├── Following Links in Python_Instructions2.png
│     ├── Following Links in Python.txt
│     ├── Results_SlightlyDifferentCode.png
│     └── known_by_Jemma.html
│
├── scraping-numbers-from-HTML-using-beautifulsoup/
│     ├── README.md
│     ├── comments_2237805.html
│     ├── comments_2237807 (1).xml
│     ├── comments_2237808.json
│     ├── Scraping HTML Data_Instructions.png
│     └── Scraping Numbers from HTML using BeautifulSoup.txt
│
└── reading-web-data-from-python.txt


Each folder includes:

The original assignment instructions

The code used to complete the assignment

My written explanation and analysis

Screenshots of execution

Any provided .html, .xml, or .json files

⸻

🧠 Learning Objectives

By completing both assignments in this module, I demonstrated the ability to:

✔ Retrieve and process HTML from a remote URL

Using urllib.request to open URLs, read raw HTML, and prepare it for parsing.

✔ Parse HTML using BeautifulSoup

Selecting tags such as <a> and <span>, extracting text, and handling attributes (href).

✔ Follow hyperlinks programmatically

Building scripts that navigate from page to page by dynamically updating URLs.

✔ Extract structured data

Converting extracted text into integers, storing values, and computing aggregated results.

✔ Work with multiple data formats

Handling:

.html

.xml

.json

which mirrors real-world data processing tasks.

✔ Write reproducible scraping scripts

Using consistent indexing logic, safe tag extraction, and preserved copies of provided files.

⸻

🧩 Assignment Summaries
1️⃣ Following Links in HTML (Web Navigation)

Start at a given URL

Extract all <a> tags

Choose the link at a specified position

Follow the link

Repeat the process a fixed number of times

Print every name encountered

Report the final name retrieved

Final Answer (June 2025 Run): Shaiza
→ (Full breakdown is in the subfolder README.)

2️⃣ Scraping Numbers from HTML (Web Scraping)

Retrieve or open an HTML file

Parse all <span> tags

Extract numbers

Convert to integers

Compute the sum

Print both count and total

This assignment establishes core scraping habits that carry over into XML and JSON parsing later in the course.

⸻

🔧 Tools & Libraries

Python 3

urllib.request — Web retrieval

BeautifulSoup (bs4) — HTML parsing

OnlineGDB — Debugging & testing environment

Local .html, .xml, .json files

Text documentation for assignment summaries

⸻

🧠 What This Module Demonstrates

This module serves as the foundation for all future Python data-gathering work I’ll do.
It shows that I can:

Connect to live web resources

Read and parse HTML content

Navigate linked pages

Extract structured data cleanly

Apply logic across networks of data

Document my code and findings with clarity

These are essential skills for:

Data analysis

Web scraping

Automation

API integration

Research scripting

Backend data workflows

⸻

✅ Status

This module is fully completed, documented, validated, and graded at 100%.
All artifacts (code, instructions, screenshots, data files) are included for transparency and reproducibility.