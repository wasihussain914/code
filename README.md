# RateMyProfessors Scraper

Selenium-based scraper for [RateMyProfessors.com](https://www.ratemyprofessors.com) that auto-clicks through a department listing, loads all professors via the "Show More" button, and exports structured data to JSON.

## What it collects

| Field | Description |
|---|---|
| Name | Professor's full name |
| Total Ratings | Number of student ratings |
| Quality | Overall quality score |
| Would Take Again | Percentage who'd take again |
| Difficulty | Average difficulty rating |

## Usage

1. Install dependencies:
   `bash
   pip install selenium
   `
2. Update scraper.py with your ChromeDriver path and browser binary.
3. Run:
   `bash
   python scraper.py
   `
4. You'll have 10 seconds to select a department on the page; the script then auto-loads and scrapes all results.
5. Output: professors_data.json

## Stack

- Python 3
- Selenium WebDriver (Brave/Chrome)
- JSON output