# Crawlers

This page describes the web crawlers operated by **nsfw-index** and is intended for
website administrators and developers who notice our crawler activity in their logs.

Our goal is to **collect publicly available metadata only**, without impacting site
performance or violating site policies.

---

## User-Agent

All official nsfw-index crawlers use the following User-Agent string:

```
nsfw-index-bot (thearialume@gmail.com; https://nsfw-index.thearialume.com/bots)
```

If you see this User-Agent in your logs, your site is being indexed for **metadata purposes only**.

---

## What we collect

nsfw-index **does not download or store media files**.

We only collect:

- Titles
- Descriptions
- Views
- Tags
- Other technical metadata

No video, image, or audio content is accessed or archived.

---

## Crawl modes

Our crawlers operate in two modes depending on site capabilities.

### Default mode
- Full site crawl by following public links
- Similar to how search engines (e.g. Googlebot) operate
- Used for initial indexing
- Runs passively or periodically (usually weekly or less)

### Incremental mode
- Supported only on sites that expose recent or updated content
- Fetches **newly published entries only**
- Runs several times per day to keep metadata fresh

---

## Crawl rate

Regardless of the mode:

- **Maximum: 1 request per second**
- Designed to be lightweight and non-intrusive

If you observe behavior that exceeds this rate or causes issues,
please contact us and we will address it immediately.

---

## robots.txt and cooperation

We **respect robots.txt directives**.

If you:

- want us to crawl your site differently
- can provide a more efficient metadata endpoint
- want to enable or disable specific crawl behavior

We are always happy to cooperate — just reach out!

---

## Open source & crawler verification

All nsfw-index crawlers are **open source**, which means anyone can technically reuse
our User-Agent string. Because of this, **User-Agent alone is not sufficient for verification**.

To verify that requests are coming from **official nsfw-index infrastructure**,
please perform a reverse DNS check.

### Step 1: Reverse lookup
```bash
host 188.137.254.69
```

Expected result (example):

```
69.254.137.188.in-addr.arpa. PTR 188-137-254-69.thearialume.com.
```

### Step 2: Forward lookup

```bash
host 188-137-254-69.thearialume.com
```

Expected result:

```
188-137-254-69.thearialume.com has address 188.137.254.69
```

If both results match, the crawler is **official and safe to allow**.

---

## Contact

If you have any questions, concerns, or suggestions regarding our crawlers,
please contact us directly:

**✉️ Email:** [thearialume@gmail.com](mailto:thearialume@gmail.com)

We are open to discussion and committed to responsible crawling! 🤍💜