# Google Scholar HSI Scraper

A Python-based scraping tool designed to extract research paper data from **Google Scholar**, specifically focused on **Hyperspectral Image (HSI) Classification** using **Graph Neural Networks (GNNs)**.

## 📌 Overview
This repository contains a Jupyter Notebook (`googlescholar_scraper.ipynb`) that automates the collection of academic titles and authors. It is pre-configured to target the latest advancements (2020–present) in graph-based remote sensing.

## 🚀 Features
* **Architecture-Specific Queries:** Specialized search loops for GCN, GAT, and GraphSAGE models.
* **Temporal Filtering:** Automatically restricts results to publications from the year **2020** onwards.
* **Clean Data Extraction:** Parses HTML to isolate clean **Paper Titles** and **Author/Source** strings.
* **Pagination Support:** Scrapes multiple result pages (approx. 60 papers per query).
* **Rate Limit Protection:** Implements a `time.sleep()` delay to minimize the risk of IP blocking.

## 🛠️ Requirements
The script utilizes the following Python libraries:
* `requests`: For handling HTTP requests to Google Scholar.
* `beautifulsoup4`: For parsing the search result HTML.
* `time`: For managing request intervals.

## 📖 Usage
1. Open the notebook in **Jupyter** or **Google Colab**.
2. Define your search string in the `query` variable:
   ```python
   query = "graph attention hyperspectral image classification"
