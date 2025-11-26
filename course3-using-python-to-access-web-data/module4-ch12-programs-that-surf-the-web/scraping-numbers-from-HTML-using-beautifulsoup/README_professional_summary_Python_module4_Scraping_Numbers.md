📘 Scraping Numbers from HTML Using BeautifulSoup

Course: Python for Everybody – Course 3
Module: Chapter 12 – Programs That Surf the Web
Platform: Coursera
Completed: ✅ June 2025
Directory: module4-ch12-programs-that-surf-the-web/scraping-numbers-from-HTML-using-beautifulsoup

⸻

🎯 Assignment Objective

This assignment demonstrates how to:

Load an HTML file from the web (or a saved local copy)

Parse its structure with BeautifulSoup

Locate specific tags (<span>)

Extract numeric content from the HTML

Convert text values into integers

Compute the sum of all extracted numbers

This introduces foundational scraping concepts: tag filtering, text extraction, and iterating through parsed elements.

⸻

🧪 Problem Summary

Given an HTML document similar to:

comments_2237805.html  

The script must:

Retrieve the HTML

Parse all <span> tags

Extract the text inside each <span>

Convert it to an integer

Add all numbers together

Print the total sum

The assignment provides several formats of similar data (HTML, XML, JSON) across different exercises, and HTML scraping is the first step in understanding structured data extraction.

⸻

🧠 Strategy

Use BeautifulSoup to retrieve all <span> tags

Loop through each tag and extract .text

Use int() to convert the number

Append values to a running total

Print the final accumulated sum

This script demonstrates how to navigate nested tags, extract values, and process them numerically.

⸻

🧾 Final Python Script

from bs4 import BeautifulSoup
import urllib.request as ur

# URL of the HTML page (or use a local file)
url = "http://py4e-data.dr-chuck.net/comments_2237805.html"

# Read and parse the HTML
html = ur.urlopen(url).read()
soup = BeautifulSoup(html, 'html.parser')

# Retrieve all <span> tags
tags = soup('span')

total = 0
for tag in tags:
    num = int(tag.text)
    total += num

print("Count:", len(tags))
print("Sum:", total)


If run locally with the downloaded file:

soup = BeautifulSoup(open("comments_2237805.html"), "html.parser")

⸻

🧩 Output (June 2025 Run)

Your .txt file records the correct values:

Count: 50
Sum: 2482

(Example numbers — your local .txt file contains your exact run results.)

⸻

📁 Folder Contents

scraping-numbers-from-HTML-using-beautifulsoup/
│
├── comments_2237805.html        # HTML to scrape
├── comments_2237807 (1).xml     # XML version (used in next assignment)
├── comments_2237808.json        # JSON version (used in next assignment)
├── Scraping HTML Data_Instructions.png
└── Scraping Numbers from HTML using BeautifulSoup.txt


File Purpose Summary

HTML/XML/JSON Files – Raw data provided by Coursera

Instructions PNG – Screenshot of assignment prompt

.txt Summary – My written explanation and recorded results

⸻

🧠 What I Learned

How to load and parse HTML files safely

How BeautifulSoup selects tags with soup('span')

How to extract numeric text from HTML nodes

How to convert extracted text into usable Python data (int())

How to handle multiple structured data formats across HTML → XML → JSON

How scraping assignments build toward real-world parsing tasks

⸻

🔧 Tools & Libraries

Python 3

BeautifulSoup (bs4)

urllib.request

Local .html, .xml, .json files for testing

OnlineGDB for debugging

⸻

✅ Status

This module is fully complete and graded at 100%.
Screenshots, files, and results have been preserved for accurate portfolio documentation.