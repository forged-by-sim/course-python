📘 Following Links in HTML Using BeautifulSoup

Course: Python for Everybody – Course 3
Module: Chapter 12 – Programs That Surf the Web
Platform: Coursera
Completed: ✅ June 2025
Directory: module4-ch12-programs-that-surf-the-web/following-links-in-HTML-using-beautifulsoup

⸻

🎯 Assignment Objective

This assignment demonstrates how to:

Retrieve HTML from a webpage using urllib

Parse and navigate <a> tags using BeautifulSoup

Extract hyperlink (href) values

Follow links programmatically

Repeat traversal a fixed number of times

Identify the final name encountered at a specified position

The challenge is designed so manual clicking will not work — the HTML visually shifts to force automated retrieval. The program must rely solely on the structure of the HTML.

⸻

🧪 Problem Summary

For this module, I wrote a Python program that:

Starts at the URL:

http://py4e-data.dr-chuck.net/known_by_Jemma.html

Finds the <a> tag at position 18 (1-based index → position 18 = list index 17)

Follows that link

Repeats the process 7 times

Prints each name encountered along the traversal

Displays the final name retrieved — which must start with S

⸻

🧠 Strategy

Retrieve HTML → parse → extract <a> tags

Convert 1-based indexing to Python’s 0-based indexing (position - 1)

Follow the href of the selected link

Store the link text (the "name")

Repeat the loop until the traversal count is reached

The included HTML file (known_by_Jemma.html) shows the exact data as it appeared during my June 2025 run. This preserved snapshot makes the results reproducible.

⸻

🧾 Final Python Script

import urllib.request as ur
from bs4 import BeautifulSoup

url = "http://py4e-data.dr-chuck.net/known_by_Jemma.html"
count = 7
position = 18

print("Retrieving:", url)

final_name = None
for i in range(count):
    html = ur.urlopen(url).read()
    soup = BeautifulSoup(html, 'html.parser')
    tags = soup('a')
    tag = tags[position - 1]
    final_name = tag.text.strip()  # This is the name encountered
    url = tag.get('href', None)
    print(f"Step {i+1}: Name = {final_name}, URL = {url}")

print("\n Final answer (name of 7th link clicked):", final_name)


⸻

🧩 Output (June 2025 Run)

The sequence of names retrieved during my execution was:

Morven

Solomon

Kaiwen

Ze

Tala

Cohen

Shaiza ← Final name

✔ Final Answer: Shaiza

(Matches the hint: name must start with S)

⸻

📁 Folder Contents

following-links-in-HTML-using-beautifulsoup/
│
├── Following Links in Python_Instructions1.png
├── Following Links in Python_Instructions2.png
├── Following Links in Python.txt
├── Results_SlightlyDifferentCode.png
└── known_by_Jemma.html   <-- HTML snapshot used in June 2025 run


What each file contains:

Instructions PNGs — Screenshots of the exact Coursera assignment prompt

Following Links in Python.txt — My written summary and notes

Results_SlightlyDifferentCode.png — Screenshot of my successful OnlineGDB output

known_by_Jemma.html — The original scraped HTML file (critical reproducibility artifact)

⸻

🧠 What I Learned

How to parse, navigate, and extract HTML data using BeautifulSoup

How to traverse linked data structures across multiple pages

How to handle indexing safely when dealing with lists of tags

How Python web scraping differs from manual navigation

Why deterministic scripts matter for reproducibility

How PY4E uses randomized HTML to enforce programmatic scraping

⸻

🔧 Tools & Libraries

Python 3

urllib.request — Fetching remote HTML

BeautifulSoup (bs4) — Parsing HTML tags

OnlineGDB — Used for testing and debugging

.html snapshots — Provided by the course and saved locally

⸻

✅ Status

This module is fully completed, validated, and graded at 100% on Coursera.
All code, outputs, and HTML snapshots have been preserved for portfolio reference.