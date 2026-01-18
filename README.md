# Python-Job-Listings-Scraper - Fake Jobs Web Scraper

A simple Python web scraping project that extracts job posting data from **https://realpython.github.io/fake-jobs/**.

This project is designed as a learning exercise to demonstrate how to:
- Scrape data from a static website
- Parse HTML using BeautifulSoup
- Handle missing fields safely
- Store structured data into a CSV file

---

## 📌 Project Requirements

The scraper extracts the following fields for **each job posting**:

- Job title
- Company name
- Location
- Job detail page URL

The extracted data is saved into a CSV file using clean and readable Python code, with basic edge-case handling.

---

## 🛠️ Technologies Used

- Python 3.x
- `requests`
- `beautifulsoup4`
- `pandas`

---

## 📂 Project Structure

```
fake-jobs-scraper/
│
├── scraper.py        # Main scraping script
├── fake_jobs.csv     # Output CSV file (generated)
├── README.md         # Project documentation
```

---

## ⚙️ Installation & Setup

1. Clone or download this repository
2. Install required dependencies:

```bash
pip install requests beautifulsoup4 pandas
```

---

## ▶️ How to Run the Scraper

Execute the Python script:

```bash
python scraper.py
```

After execution, a file named **`fake_jobs.csv`** will be created in the project directory containing all scraped job data.

---

## 🧠 How It Works (High-Level Overview)

1. Sends an HTTP request to the target website
2. Parses the HTML content using BeautifulSoup
3. Locates all job cards on the page
4. Extracts relevant job information from each card
5. Handles missing fields gracefully
6. Saves the collected data into a CSV file

---

## 🛡️ Edge Case Handling

- If a field (title, company, location, or URL) is missing, the value is set to `None`
- The scraper continues running without crashing
- Uses helper functions to safely extract text

---

## 📄 Sample Output (CSV)

```
job_title,company_name,location,detail_page_url
Senior Python Developer,"Payne, Roberts and Davis","Stewartbury, AA",https://realpython.github.io/fake-jobs/jobs/senior-python-developer-0.html
Energy engineer,Vasquez-Davidson,"Christopherville, AA",https://realpython.github.io/fake-jobs/jobs/energy-engineer-1.html
```

---

## ⚠️ Disclaimer

This website contains **fake job postings** and is intended **only for educational and practice purposes**.

---

## 🚀 Possible Improvements

- Scrape job descriptions from detail pages
- Add logging instead of print statements
- Implement retry logic for failed requests
- Add unit tests
- Convert the scraper into a class-based design

---

## 👤 Author

Created as a learning project for practicing Python web scraping.

