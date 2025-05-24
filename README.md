# 🕸 Retail Store Scraping Portfolio – Belgium

## 📊 Executive Summary
This project is a real-world freelance case study where I extracted structured store data from **9 major retail chains** in Belgium. Each site presented unique technical challenges — from static HTML and JavaScript-rendered content to hidden REST and GraphQL APIs.

The goal: deliver **clean, geolocated, and contact-rich datasets** for each retailer, suitable for mapping, BI analysis, or internal tooling.

> 💼 This was my **first Upwork contract** and was completed under a 3-day deadline and 10-hour budget.

---

## 🧠 Skills Demonstrated
| Area                  | Details                                                                 |
|-----------------------|-------------------------------------------------------------------------|
| Web Scraping          | HTML parsing, dynamic page navigation, API reverse-engineering         |
| API Integration       | REST APIs, GraphQL with persisted queries, Google Maps geocoding       |
| Data Engineering      | Data normalization, fallback handling, field mapping, batch exports     |
| Tools & Libraries     | `requests`, `beautifulsoup4`, `selenium`, `pandas`, `json`, `time`      |

---

## 🗂 Retail Websites Processed

| Retailer     | Method Used                             | Notes                                                                 |
|--------------|------------------------------------------|-----------------------------------------------------------------------|
| **AVA**       | BeautifulSoup + detail page scraping     | Store manager & email parsed from nested subpages                     |
| **Carrefour** | Hidden REST API                          | Full metadata via `/locations?` endpoint, filtered by brand           |
| **Maxi Zoo**  | Selenium navigation                      | JavaScript-based region > store detail traversal                      |
| **Brico**     | CloudFront JSON + REST store detail API | Merged lat/lng from base JSON with contact info from detail endpoint |
| **Medi-Market** | Static HTML + Google Maps API         | Parsed contact info & enriched lat/lng via geocoding                  |
| **Jumbo**     | Deeply nested frontend JSON             | Recursive parsing of React-style JSON structure                       |
| **Intersport** | Static HTML copy parse                  | Extracted address, phone, and daily schedules                         |
| **Krëfel**    | Nested JSON structure                    | Full address, geoPoint, temporary closure, and contact info           |
| **Action**    | GraphQL API (persisted query)           | Used hashed query ID, probed store ID range (2000–3000)               |

---

## 📦 Output Fields
All datasets include:
- ✅ Store Name  
- ✅ Full Address  
- ✅ Latitude & Longitude  
- ✅ Country  
- ✅ Parking Type (if available)  
- ✅ Contact Phone & Email  
- ✅ Contact First/Last Name (if available)  
- ✅ Opening Hours (where applicable)

Final output was exported as `.xlsx` or `.csv` for each retailer and validated for formatting and completeness.

---

## 📁 Repository Structure

