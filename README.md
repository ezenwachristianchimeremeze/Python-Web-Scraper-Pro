# Python Web Scraper Pro — Development Archive

A collection of small Python scraping and website-audit experiments developed while learning web data extraction and technical SEO.

> **Status: experimental.** This repository is not currently a single, production-ready application. It contains multiple scripts and nested project directories that are being reviewed and separated into focused repositories.

## Main scripts

| File | Purpose | Current scope |
|---|---|---|
| `scraper.py` | Demonstration scraper for a public practice website | Fetches a sample page and prints a few team names |
| `app.py` | Flask-based website audit prototype | Fetches a supplied page and reports title presence, H1 count, and images missing alt text |
| `audit.py` | Additional audit experiment | Review source before relying on it |
| `cvs.py` | Small standalone experiment | Review source before relying on it |

The repository also contains unrelated experiments and nested projects. Those are not dependencies of the two main scripts above.

## Run the scraper example

Python 3.10 or newer is recommended.

    python -m venv .venv
    source .venv/bin/activate
    pip install -r requirements.txt
    python scraper.py

The example targets a public practice site. Use scraping responsibly, respect the target site's terms and robots policy, rate-limit requests, and do not collect personal or restricted data without permission.

## Run the Flask prototype

    python app.py

The prototype is intended for local evaluation only. **Do not expose it as a public service yet.** Its URL-fetching route needs stronger SSRF protections, destination validation, redirect controls, and tests before deployment.

## Development status

- The scripts are learning and prototype work, not a maintained production package.
- Automated tests and CI checks have not yet been established for this repository.
- Dependencies are listed in `requirements.txt`.
- Keep credentials, local device files, caches, virtual environments, databases, generated data, and personal configuration out of Git.

## Planned cleanup

1. Separate unrelated projects into their own repositories.
2. Add focused tests for the scraper and audit functions.
3. Add URL validation and SSRF protections to the Flask prototype.
4. Add linting and CI checks.
5. Publish only sample datasets that are safe to redistribute.

## Author

**Ezenwa Christian Chimeremeze**

- [GitHub](https://github.com/ezenwachristianchimeremeze)
- [LinkedIn](https://www.linkedin.com/in/ezenwa-christian-chimeremeze-b77115440)
- [Medium](https://ezenwachristianchimeremeze.medium.com/)
