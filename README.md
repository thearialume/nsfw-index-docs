<p align="center">
  <a href="https://nsfw-index.thearialume.com">
    <img src="https://nsfw-index.thearialume.com/assets/banner.png" alt="nsfw-index">
  </a>
</p>

<p align="center">
  Documentation source for nsfw-index project
</p>

---

**⭐ Website:** <a href="https://nsfw-index.thearialume.com" target="_blank">https://nsfw-index.thearialume.com</a>  
**👾 Crawlers:** <a href="https://nsfw-index.thearialume.com/bots" target="_blank">https://nsfw-index.thearialume.com/bots</a>    
**✉️ Contact:** <a href="mailto:thearialume@gmail.com" target="_blank">thearialume@gmail.com</a>

---

## 📘 About This Repository

This repository contains the **source code of the official documentation website** for the **nsfw-index** project.

It is part of the nsfw-index ecosystem and is responsible for:

- Project documentation  
- API references  
- Crawlers and data format descriptions  
- Contribution guides  
- Public project information  

👉 The main scraping and indexing logic lives in the [`nsfw-index`](https://github.com/thearialume/nsfw-index) repository.

> [!WARNING]
> This documentation, datasets, and API are related to **adult-oriented platforms and materials**.
>
> The service **does not host, store, or distribute any adult content**. Only **publicly available metadata** (such as titles, descriptions, tags, and technical attributes) is collected and indexed.
>
> This project is intended for **legal adults only** and for professional development, research, or analytical purposes.

---

## 🛠 Tech Stack

The documentation site is built with:

- 📚 **MkDocs Material**  
  👉 https://github.com/squidfunk/mkdocs-material  

- 🐳 **Docker for deployment:**  
  👉 `nginx:stable-alpine`

- 🚀 **Deployment platform:**  
  👉 [Coolify](https://github.com/coollabsio/coolify)

---

## 🚀 Local Development

Want to preview the docs locally?

1. **Clone the repository:**
```bash
git clone https://github.com/thearialume/nsfw-index-docs.git
cd nsfw-index-docs
```

1. **Install dependencies:**
```bash
python3 -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
pip install mkdocs-material
```

1. **Run development server:**
```bash
mkdocs serve --livereload
```

1. **Open in browser:**
```
http://127.0.0.1:8000
```

Changes to `.md` files will auto-reload! ✨

---

## ⚙️ Build Process

To build the documentation into static files for production:
```bash
apk add --no-cache python3 py3-pip && \
python3 -m venv .venv && \
. .venv/bin/activate && \
pip3 install mkdocs-material && \
mkdocs build
```

This generates a static site inside the `site/` directory, which is then served by **nginx**.

---

## 🤝 Contributing

If you'd like to improve the documentation:

* Fix typos
* Improve explanations
* Add guides or examples
* Improve structure or navigation

You're very welcome to contribute via pull requests 💜

---


## License 

**Code:** MIT  
**Data:** CC-BY-SA 4.0