# osint-harvester — archived research prototype

![Python](https://img.shields.io/badge/Language-Python-3772AB?style=flat-square)
![Status](https://img.shields.io/badge/Status-Archived%20%C2%B7%20Do%20not%20run-B00020?style=flat-square)

> **Archived.** This was a Playwright experiment for collecting publicly
> reachable web data. It is kept only as a record of what not to do. It is not
> maintained, not supported, and must not be run against any third-party
> service.

---

## Why it is archived

The prototype talked to an intelligence platform through **undocumented
endpoints instead of its official API**, without an API key or authorization.
That is a terms-of-service violation and, depending on where you live and what
is collected, may also violate computer-misuse and data-protection law. The
approach is intentionally not documented here.

Use the platform's official API with your own key, or a public dataset, instead.
If you need a general Playwright scraping example, use a site that permits
automated access and respect its `robots.txt`, rate limits and terms.

## Data in this repository

`output/` contains files produced by past runs that include **personal data**
(names, addresses, phone numbers, account identifiers). Those files:

- must not be redistributed;
- should be deleted from the working tree **and from the Git history** (a normal
  commit does not remove them from history);
- must never be committed again — add `output/` to `.gitignore`.

If any of that data belongs to a third party, delete it and notify the affected
party where required by law.

## Repository contents

```text
scripts/
  scraper.py    # archived entry point (not runnable without private config)
  console.js    # browser-side collector
output/         # past run output containing personal data - do not reuse
```

## Status

No fixes, no updates, no pull requests. The correct action for this repository
is to archive it, purge `output/`, and start over with an official API if the
research is still needed.

## License

No license is granted. All rights reserved.
