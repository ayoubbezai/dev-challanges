# 🚀 AI Internship Finder – Your Personalized Internship Matchmaker

**Author:** ayoubbezai

## Description

Finding the perfect internship can be overwhelming… What if a system could match you with the best opportunities based on your skills, studies, or CV?

This challenge is about building a tool or website where users can input their skills and study areas via CLI or web interface. The system should scrape 1 or more internship websites and use the Gemini API to intelligently suggest relevant internships.

For advanced functionality, users can upload their CV for better matching and more accurate recommendations.

⚠️ **Important:** Using pre-made tools like Vibe Code will not work for this challenge. You need to implement your own logic for scraping, parsing, and matching. Using external tools may result in wrong logic, missing results, or failed matches.

## 🎯 Your Mission

Build a tool or website that:

1. Accepts user skills and study areas through CLI or web interface.
2. Scrapes internship listings from 1+ websites.
3. Uses the Gemini API to enhance recommendations.
4. (Optional/Advanced) Accepts a CV upload to refine matching.

## 🔍 Starting Point

* You may use Python, Node.js, or any language of your choice.
* The challenge can be implemented as:
   * Simple version: CLI-based input → text output of internships
   * Advanced version: Web interface + CV upload + enriched matching

## 🕵️‍♂️ Scoring

* Points: 0 – 900
* The score depends entirely on the tool you build and the results you obtain from the internship matching.
* Simple tools with CLI input are valid but earn fewer points.
* Advanced implementations with CV uploads, multiple website scraping, and Gemini API-based recommendations will score higher.

The difficulty of the challenge is flexible: it can range from very easy (basic CLI tool) to advanced (full-featured tool with web interface and CV parsing).

## 📌 Deliverables

1. Your tool or website
2. Code repository (GitHub link preferred)
3. (Optional) Demo of advanced features: CV upload, web interface, and enhanced recommendations

## ⚠️ Notes & Tips

* Make sure scraping respects website terms of service.
* Validate CV uploads carefully to avoid errors.
* Use the Gemini API to improve matching relevance.
* Your system should provide clear, structured output for the internships (e.g., title, company, location, URL).

## 📁 Project Structure

Use a good project structure to keep your code organized and maintainable.

**Example structure:**

```
ai-internship-finder/
├── src/
│   ├── scraper/
│   │   ├── __init__.py
│   │   └── internship_scraper.py
│   ├── matcher/
│   │   ├── __init__.py
│   │   └── gemini_matcher.py
│   ├── parser/
│   │   ├── __init__.py
│   │   └── cv_parser.py
│   └── main.py
├── tests/
├── requirements.txt
├── .env.example
└── README.md
```

Good luck! 🔍