# Fake Crawler

A url crawler.

![image](https://github.com/user-attachments/assets/0acb465c-58ba-46c4-ada1-04e618a47ec3)

## Installation


```bash
git clone https://github.com/anubhavv106/FakeCrawler.git
```

## Usage

```python
Clone the Repository

# Install the Requirements
   pip install -r requirements.txt

# Executing
  python3 FakeCrawler.py -h

# Options
   -h, --help            show this help message and exit
  --url URL             An initial URL to target.
  --email EMAIL         A comma-separated list of email domains to look for in page content. Defaults to the root
                        domain of the passed-in URL.
  --threads THREADS     The max number of threads to use. Defaults to 10.
  --limit LIMIT         The number of URLs to process before exiting. Defaults to 500. Set to 0 for no limit
                        (careful).
  --proxy PROXY         Specify a proxy to use.
  --headers HEADERS     Override defaults with the indicated headers. ex: "{'user-agent':'value','accept':'value'}"
                        ~/.aws/credentials file.
  --region REGION       The AWS region to create FireProx resources in.
  --json                Output in JSON format
  --robots              Search pages found in the robots.txt file
  --sitemap             Search pages found in the site's sitemap.
  --suppress_progress   Only show final output.
  --comments            Return HTML comments extracted from crawled pages
  --tags                Return tags (UA,GTM,etc.) extracted from crawled pages
  --ips                 Return IP addresses extracted from crawled page content
```
## Demo Usage

## License

[MIT](https://github.com/anubhavv106/Osint-Project/blob/master/LICENSE)
