# AI Lead Enrichment & Outreach Agent

## What it does
Automates B2B lead research and cold email drafting.
Drop a LinkedIn URL in a Google Sheet → AI scores the lead 
→ writes a personalised 3-line cold email → results written back to sheet.

## Stack
n8n · Gemini API · Google Sheets · JavaScript

## Workflow
1. Google Sheets Trigger — detects new LinkedIn URL
2. Profile data (mock — swap Proxycurl API key for live scraping)
3. Gemini enrichment — fit score, pain points, ICP match
4. IF node — filters low-fit leads automatically
5. Gemini email draft — personalised 3-line cold email
6. Google Sheets update — results written back automatically
