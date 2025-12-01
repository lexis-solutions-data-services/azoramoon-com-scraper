![banner](https://i.ibb.co/rf2MPgGs/azoramoon.png)

# Azoramoon Scraper

Easily extract manga and series information from Azoramoon using this Apify actor built with Crawlee and TypeScript. Perfect for researchers, manga enthusiasts, and developers who want structured data from Azoramoon.

<p align="center">
  <img src="https://apify-image-uploads-prod.s3.us-east-1.amazonaws.com/DevbkY3adMTBuoECt-actor-LVG0RyQbS1jqYiRfE-H9Por6P98d-Screenshot_2025-07-29_at_10.24.36.png" alt="Azoramoon Scraper" style="height: 60px; margin-right: 15px;" /><a href="https://apify.com/lexis-solutions/azoramoon-com-scraper" target="_blank">
    <img src="https://img.shields.io/badge/Try%20it%20on-Apify-0066FF?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDA4IiBoZWlnaHQ9IjQwOCIgdmlld0JveD0iMCAwIDQwOCA0MDgiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxnIGNsaXAtcGF0aD0idXJsKCNjbGlwMF8zNDFfNDE1NykiPgo8cGF0aCBkPSJNMjE4LjY5NSAxMDRIMzAwLjk3QzMwMi42NDMgMTA0IDMwNCAxMDUuMzU3IDMwNCAxMDcuMDNWMjMyLjc2NkMzMDQgMjM1Ljc3OCAzMDAuMDgzIDIzNi45NDUgMjk4LjQzNCAyMzQuNDI1TDIxNi4xNTkgMTA4LjY5QzIxNC44NDEgMTA2LjY3NCAyMTYuMjg3IDEwNCAyMTguNjk1IDEwNFoiIGZpbGw9IndoaXRlIi8+CjxwYXRoIGQ9Ik0xODkuMzA1IDEwNEgxMDcuMDNDMTA1LjM1NyAxMDQgMTA0IDEwNS4zNTcgMTA0IDEwNy4wM1YyMzIuNzY2QzEwNCAyMzUuNzc4IDEwNy45MTcgMjM2Ljk0NSAxMDkuNTY2IDIzNC40MjVMMTkxLjg0IDEwOC42OUMxOTMuMTU5IDEwNi42NzQgMTkxLjcxMyAxMDQgMTg5LjMwNSAxMDRaIiBmaWxsPSJ3aGl0ZSIvPgo8cGF0aCBkPSJNMjAyLjU5MSAyMDQuNjY4TDEwOS4xMjcgMjk4LjgzNUMxMDcuMjI5IDMwMC43NDcgMTA4LjU4MyAzMDQgMTExLjI3OCAzMDRIMjk2LjhDMjk5LjQ4MyAzMDQgMzAwLjg0MiAzMDAuNzcgMjk4Ljk2NyAyOTguODUyTDIwNi45MDggMjA0LjY4NUMyMDUuNzI2IDIwMy40NzUgMjAzLjc4MiAyMDMuNDY4IDIwMi41OTEgMjA0LjY2OFoiIGZpbGw9IndoaXRlIi8+CjwvZz4KPGRlZnM+CjxjbGlwUGF0aCBpZD0iY2xpcDBfMzQxXzQxNTciPgo8cmVjdCB3aWR0aD0iMjAwIiBoZWlnaHQ9IjIwMCIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEwNCAxMDQpIi8+CjwvY2xpcFBhdGg+CjwvZGVmcz4KPC9zdmc+Cg==&logoColor=white" alt="Try it on Apify" style="border-radius: 12px; height: 60px;" />
  </a>
</p>


---


## 📊 Actor Stats

| Stat | Value |
|------|-------|
| **Version** | `0.0.2` |
| **Last Update** | Dec 1, 2025 |

---



## 💻 Integration Examples

This repository includes example code showing how to integrate the `azoramoon-com-scraper` actor into your projects.

You can find example implementations in the [`examples/`](./examples) folder:
- **TypeScript/JavaScript**: See [`examples/typescript/`](./examples/typescript) for a complete TypeScript example
- **Python**: See [`examples/python/`](./examples/python) for a complete Python example

Each example includes:
- Ready-to-use code templates
- Setup instructions
- Documentation links

---


## ✨ Key Features

- 🔎 Scrape manga/series details including **title, summary, cover image, categories, and rating**
- 📄 Outputs clean, structured JSON for easy integration
- ⚡ Fast, reliable, and customizable with Crawlee and Apify
- 🏷️ Supports scraping multiple pages and series

---

## 🛠 Input Schema

```json
{
  "startUrls": [{ "url": "https://azoramoon.com/series/" }],
  "maxItems": 100 // Optional, default is 100
}
```

- `startUrls` (required): Array of objects with `url` fields pointing to Azoramoon listing or series pages.
- `maxItems` (optional): Maximum number of series to scrape (default: 10).

---

## 📤 Output Schema

Each result is a JSON object with the following fields:

```json
{
  "url": "https://azoramoon.com/series/the-sleepless-night-of-the-maid/",
  "title": "The Sleepless Night of the Maid",
  "summary": "إيفا مايسي ، التي كانت تعيش حياة صعبة كخادمة في منزل أحد معارفها بعد سقوط عائلتها النبيلة ، تقابل خطيبها السابق ، الأمير إدوارد ، عن طريق الصدفة. بعد مغادرته ، تدرك إيفا أنه حبها الأول ، وتتخلى عن مشاعرها الحالية ، قائلة إن هذه نهاية علاقتها به. بعد التغلب على مثل هذا الوقت الصعب ...",
  "primaryImage": "https://azoramoon.com/wp-content/uploads/2022/08/xxlarge.webp",
  "categories": ["إثارة رومانسي شوجو", "إثارة رومانسي شوجو"],
  "rating": "3.9"
}
```

- `url`: Series detail page URL
- `title`: Series title
- `summary`: Series summary/description
- `primaryImage`: Cover image URL
- `categories`: Array of category strings
- `rating`: Series rating (as string)

---

## Need to scrape more data

Check out our other scrapers:
- **Manga & Anime** 愛
  - [HiAnimez Scraper](https://apify.com/lexis-solutions/hianimez-to-scraper): Extract anime metadata, genres, ratings, and more from HiAnimez.
- **Business & Real Estate** 🏢
  - [Redfin Scraper](https://apify.com/lexis-solutions/redfin-scraper)
  - [Hemnet.se Scraper](https://apify.com/lexis-solutions/hemnet-se-scraper)
- **Marketplace & E-commerce** 🛒
  - [Alibaba Scraper](https://apify.com/lexis-solutions/alibaba-scraper)
  - [BizBuySell Scraper](https://apify.com/lexis-solutions/bizubuysell)

---

## 🤝 About

This scraper is part of the [Lexis Solutions](https://www.linkedin.com/company/lexis-solutions) open-source web scraping monorepo. All scrapers are SEO-optimized and published to the Apify Store.

For custom solutions or support, contact us at [scraping@lexis.solutions](mailto:scraping@lexis.solutions).

---
