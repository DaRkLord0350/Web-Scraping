﻿# 🕸️ Web Scraping Tool

A flexible command-line tool to scrape text, images, or structured data from websites. Designed for simple extraction or crawling multiple pages.

---

## 🚀 Features

* Scrape webpage text or images
* Save output as `.txt`, `.pdf`, `.csv`, or `.html`
* Crawl internal links with regex support
* Optional image downloading
* Custom XPath and tag attribute filters
* Simple CLI usage

---

## 📁 Project Structure

```
Web-Scraping-Tool/
│
├── scrape/                  # Main module code
│   ├── __init__.py
│   ├── scrape.py            # Main CLI entrypoint
│   ├── crawler.py
│   ├── utils.py
│   └── orderedset.py
│
├── setup.py
└── README.md                # You're here
```

---

## ⚙️ Method 1: Environment Setup

1. **Clone the Repository**

```bash
git clone <https://github.com/DaRkLord0350/Web-Scraping.git>
cd Web-Scraping-Tool
```

2. **Create Virtual Environment**

```bash
python -m venv venv
venv\Scripts\activate    # On Windows
```

3. **Install Dependencies**

```bash
pip install -e .
```

4. **Run the Scraper**

```bash
scrape https://quotes.toscrape.com -t -o quotes.txt
```

> ⚠️ If you see Unicode errors, try:
>
> ```powershell
> $env:PYTHONIOENCODING="utf-8"
> scrape https://example.com -t -o output.txt
> ```

---

## ⚡ Method 2: Run Directly from CLI

Once installed using `pip install -e .`, the `scrape` command becomes globally available.

### ✅ Example Usage:

```bash
scrape https://archive.nptel.ac.in/courses/106/105/106105217/ -t -o quotes1.txt
```

---

## 🚫 Limitations

* May not work on websites that block scraping or use JavaScript-rendered content.
* Some characters might need UTF-8 handling.

---

## ✍️ Author

**Anshuman Jha**
Email: [anshuman.jha2025@gmail.com](mailto:anshuman.jha2025@gmail.com)

---

## 📝 License

This project is licensed under the MIT License.
