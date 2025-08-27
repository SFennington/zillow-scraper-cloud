# Zillow Scraper Cloud

This repository contains a cloud-based Zillow scraper using Puppeteer and Google Sheets.

## How it works

1. Google Sheets Apps Script sends a Zillow URL to Cloud Run.
2. Cloud Run runs Puppeteer headless Chrome, scrapes listings, and writes them to Google Sheets.
3. The results appear in a new top tab in the sheet.

## Files

- `index.js` → Node.js server with Puppeteer scraping code
- `package.json` → Node dependencies
- `service-account.json` → Google Sheets service account key
- `Dockerfile` → Container setup for Cloud Run
