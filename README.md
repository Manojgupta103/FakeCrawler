# Fake Crawler

![image](https://github.com/user-attachments/assets/0acb465c-58ba-46c4-ada1-04e618a47ec3)

**Fake Crawler** is a web crawling and reconnaissance tool designed to extract useful information from websites. It performs a comprehensive crawl of a given URL and collects data on various elements including subdomains, social links, emails, files, IP addresses, and more.

## Features

- **Multithreaded Crawling:**
  - Utilizes multiple threads to speed up the crawling process and handle concurrent requests efficiently.
- **URL Handling:**

  - Normalizes and resolves relative URLs to ensure accurate crawling and discovery of all reachable pages.

- **Data Extraction:**

  - Extracts emails, IP addresses, files, HTML comments, and metadata tags from crawled pages.

- **Sitemap and Robots.txt Processing:**

  - Automatically discovers and processes pages listed in `robots.txt` and sitemap files for comprehensive coverage.

- **Proxy and Header Support:**

  - Configurable proxy settings and custom headers for requests to adapt to different crawling environments.

- **FireProx Integration:**

  - Optional integration with FireProx to manage requests through a rotating proxy service, enhancing anonymity and bypassing rate limits.

- **Alerts and Error Handling:**
  - Provides alerts for challenges such as rate limiting, Cloudflare protection, and other potential issues encountered during crawling.

## Installation

```bash
git clone https://github.com/anubhavv106/FakeCrawler.git
```

## Usage

```python
Clone the Repository

# Install the Requirements
   pip install -r requirements.txt
```

## Commands

```bash
python3 FakeCrawler.py --url <target-url> [options]
```

## Options

- `--help`, `-h`

  - **Description:** Show this help message and exit.
  - **Example:** `python FakeCrawler.py --help`

- `--url` URL

  - **Description:** An initial URL to target.
  - **Example:** `python FakeCrawler.py --url http://example.com`

- `--email` EMAIL

  - **Description:** A comma-separated list of email domains to look for in page content. Defaults to the root domain of the passed-in URL.
  - **Example:** `python FakeCrawler.py --email example.com,anotherdomain.com`

- `--threads` THREADS

  - **Description:** The maximum number of threads to use. Defaults to 10.
  - **Default:** 10
  - **Example:** `python FakeCrawler.py --threads 5`

- `--limit` LIMIT

  - **Description:** The number of URLs to process before exiting. Defaults to 500. Set to 0 for no limit (careful).
  - **Default:** 500
  - **Example:** `python FakeCrawler.py --limit 1000`

- `--proxy` PROXY

  - **Description:** Specify a proxy to use.
  - **Example:** `python FakeCrawler.py --proxy http://localhost:8080`

- `--headers` HEADERS

  - **Description:** Override defaults with the indicated headers. Must be in JSON format (e.g., `{'user-agent':'value','accept':'value'}`).
  - **Example:** `python FakeCrawler.py --headers "{'user-agent':'custom-agent','accept':'application/json'}"`

- `--region` REGION

  - **Description:** The AWS region to create FireProx resources in.
  - **Example:** `python FakeCrawler.py --region us-east-1`

- `--json`

  - **Description:** Output in JSON format.
  - **Example:** `python FakeCrawler.py --json`

- `--robots`

  - **Description:** Search pages found in the `robots.txt` file.
  - **Example:** `python FakeCrawler.py --robots`

- `--sitemap`

  - **Description:** Search pages found in the site's sitemap.
  - **Example:** `python FakeCrawler.py --sitemap`

- `--suppress_progress`

  - **Description:** Only show final output.
  - **Example:** `python FakeCrawler.py --suppress_progress`

- `--comments`

  - **Description:** Return HTML comments extracted from crawled pages.
  - **Example:** `python FakeCrawler.py --comments`

- `--tags`

  - **Description:** Return tags (UA, GTM, etc.) extracted from crawled pages.
  - **Example:** `python FakeCrawler.py --tags`

- `--ips`
  - **Description:** Return IP addresses extracted from crawled page content.
  - **Example:** `python FakeCrawler.py --ips`

## Demo Usage

https://github.com/user-attachments/assets/eb96b11e-4326-4822-af40-951be7e077e0

## Contributers

<a href="https://github.com/remarkablemark">
  <img src="https://github.com/remarkablemark.png">
</a>

## License

[MIT](https://github.com/anubhavv106/Osint-Project/blob/master/LICENSE)
