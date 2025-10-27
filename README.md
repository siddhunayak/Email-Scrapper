
# 📧 Email Scraper Workflow (No-Code Automation)

Welcome to the **Email Scraper Workflow** project — a **no-code solution** for collecting business emails automatically using **n8n**!
This workflow scrapes Google Maps for business listings, extracts their website URLs, visits each site to find email addresses, removes duplicates, and exports all data neatly into **Google Sheets** — without writing a single line of code.

---

## 🚀 Features

* 🌐 **Scrapes business websites** directly from Google Maps
* 📬 **Extracts and cleans email addresses** automatically
* ♻️ **Removes duplicates and filters invalid data**
* 📊 **Exports results to Google Sheets**
* ⚙️ Fully **no-code / low-code setup** with **n8n**
* 🕒 Supports **rate limiting and delay control** for safe scraping
* 🧩 Can be easily **modified for any business category or region**

---

## 🧩 Prerequisites

Before getting started, make sure you have:

* A running instance of [**n8n**](https://n8n.io/)
* A **Google Cloud account** to access the Google Sheets API
* **Docker** (optional, for local deployment)
* Basic familiarity with automation workflows

---

## ⚙️ Setup Instructions

For complete setup — including Docker installation, n8n configuration, Google API credentials, and workflow integration —
please refer to the step-by-step guide in the PDF below:

📘 **[Email_Scrapper_workflow.pdf](./Email_Scrapper_workflow.pdf)**

The guide covers:

* Setting up **n8n locally or on a server** (via Docker or Docker Compose)
* Configuring **HTTP Request**, **Filter**, and **Function** nodes for scraping
* Extracting and cleaning email data using **Regex expressions**
* Enabling and connecting the **Google Sheets API**
* Exporting clean, deduplicated data automatically

---

## 🧠 Workflow Overview

1. **Trigger Node** → Starts the workflow manually or on schedule
2. **HTTP Request Node** → Scrapes Google Maps listings
3. **Function Node** → Extracts and filters URLs
4. **Filter & Remove Duplicates Nodes** → Cleans invalid and duplicate URLs
5. **Loop Over Items** → Iterates through each website
6. **HTTP Request Node (Scrape Site)** → Fetches site HTML data
7. **Function Node (Extract Emails)** → Uses Regex to find email patterns
8. **Google Sheets Node** → Appends cleaned emails to your sheet

---

## 🗂 Example Output (Google Sheets)

| Business Name       | Website URL                                                         | Email Address                                               | Source Link                                |
| ------------------- | ------------------------------------------------------------------- | ----------------------------------------------------------- | ------------------------------------------ |
| Interior Design Co. | [www.designhub.in](http://www.designhub.in)                         | [contact@designhub.in](mailto:contact@designhub.in)         | [Google Maps](https://maps.google.com/...) |
| Bright Interiors    | [www.brightinteriorstudio.com](http://www.brightinteriorstudio.com) | [hello@brightinterior.com](mailto:hello@brightinterior.com) | [Google Maps](https://maps.google.com/...) |

----

## 💡 Key Benefits

* 100% **No-Code** setup using n8n
* Reusable and modular workflow structure
* Easily customizable for new locations or business types
* Integrated with **Google Sheets API** for real-time data sync
* Scalable for both small and large datasets

---

## 🧩 Future Enhancements

* Add **AI-based data enrichment** (e.g., classify businesses by niche)
* Automate daily or weekly runs using **n8n Cron triggers**
* Store output in databases like **PostgreSQL** or **Airtable**
* Include **company names and contact forms** in scraping

---

## 🏁 Summary

You now have a fully automated **Email Scraper Workflow** that can:

✅ Collect business information from Google Maps
✅ Visit websites and extract valid emails
✅ Clean and organize results automatically
✅ Export all results into a shareable Google Sheet

All of this — with **zero coding**. ⚡

