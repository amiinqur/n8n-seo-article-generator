# SEO Article Generator (n8n + AI Agents)

This project automates the generation and publishing of high-quality, SEO-optimized articles using **n8n workflows** and AI agents. It is designed for content teams, marketers, and developers looking to streamline content creation and improve search engine visibility with minimal manual effort.  

## Overview

The SEO Article Generator leverages workflow automation and AI to convert raw web data into polished articles. By integrating multiple services, the system can autonomously fetch country-specific topics, search for relevant information, extract content, and generate SEO-friendly articles ready for publication.  

Key objectives:  
- Automate repetitive content creation tasks.  
- Ensure articles are SEO-optimized and unique.  
- Reduce dependency on manual research and writing.  
- Provide an end-to-end solution from data collection to publication.  

---

## Workflow Description

The workflow consists of the following steps:

1. **Fetch Countries**  
   - Reads a list of countries from **Google Sheets**.  
   - Each country serves as the basis for generating localized content topics.  

2. **Generate Search Query**  
   - An AI agent creates a relevant search query for each country.  
   - Queries are designed to target high-impact SEO topics.  

3. **Google Search**  
   - Executes the generated queries using the **Google Custom Search JSON API**.  
   - Retrieves the most relevant web links for the given topic.  

4. **Scrape Data**  
   - Extracts text and structured content from the retrieved links.  
   - Handles dynamic content and parses relevant information for article generation.  

5. **Generate Article**  
   - AI agent processes the scraped data and creates a unique, SEO-friendly article.  
   - Ensures proper keyword placement, readability, and relevance to the target audience.  

6. **Publish Article**  
   - Posts the generated article to a website via API integration (WordPress or other CMS).  
   - Supports scheduling, content categorization, and tagging for SEO purposes.  

---

## Technology Stack

The system integrates multiple tools and technologies for seamless automation:

- **n8n** – Workflow automation platform for orchestrating the pipeline.  
- **Google Sheets API** – Fetches dynamic lists of countries and topics.  
- **Google Custom Search JSON API** – Retrieves top search results for query generation.  
- **AI Agent (LLM integration)** – Generates search queries and processes content into polished articles.  
- **Web Scraping Nodes** – Extracts structured content from web pages.  
- **Website/WordPress API** – Publishes the final articles directly to the target site.  
## Repository Structure

