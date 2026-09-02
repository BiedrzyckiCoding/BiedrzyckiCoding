# Hi, I'm Jakub

AI/ML engineer building automated data pipelines, and founder of a client-side SEO utility platform.

---

## Work & Experience

**Data Science Intern - Ringier Axel Springer Polska**
- Delivered projects automating ML model training pipelines predicting article revenue and conversion rates.
- Improved model accuracy, increasing conversions.
- Worked with Amazon SageMaker, Athena SQL, S3, AutoGluon (Python), Airflow, and Docker in a remote development environment.

**Founder - [BentoUtils](https://bentoutils.com)**
A libre utility app platform: 230+ browser tools (calculators, converters, generators) that run entirely client-side, no uploads, no tracking. Deployed as a Cloudflare Worker PWA in vanilla JS, no framework, no build step.
- Built the SEO system end to end: static content-depth sections on every tool, FAQPage/BreadcrumbList/SoftwareApplication schema, a generated internal-linking graph across the whole site, and an `llms.txt` index tuned for AI-citation crawlers like GPTBot and ClaudeBot.
- Runs on Claude Code routines that generate and check that SEO surface automatically (related-tools linking, sitemap drift, blog indexing) so it stays in sync as new tools ship.
- Handles billing and auth through Stripe checkout, Resend magic links, and Cloudflare KV-backed license tokens, monitored with Cloudflare Web Analytics.

**Technical Lead - [Daybreak Brief](https://daybreak-brief.com)**
An automated news briefing product built as four services chained on a GitHub Actions schedule, backed by Supabase:
- `get-articles` pulls tracked topics and domains from Supabase, then queries the GDELT news index for that day's coverage.
- `scrape-and-clean` fetches and cleans the full article text behind each result.
- `score-articles` embeds every article (MiniLM, 384-dim), drops near-duplicates by cosine similarity, clusters by topic with DBSCAN, and scores each one on topic importance and cluster centrality.
- `summarise-and-send` deduplicates the day's scored set, summarises it with an LLM, and sends the newsletter.
- A Flask + Supabase site handles the public front end, Stripe billing, and rate-limited routes.

**CTO - Picxelit**
A custom brick-mosaic kit business: customers turn a photo into a physical LEGO-style kit they build by hand. Built the funnel end to end, from client-side photo pixelization through Stripe checkout, and learned to keep two live frontends (a static production build and a Python dev server) honestly in sync.

---

## Personal & Hobby Projects

**[CIFAR-10 Convolutional Neural Network](https://github.com/BiedrzyckiCoding/convolutional-neural-network)**
A from-scratch CNN image classifier (3 conv blocks, batch norm, increasing dropout, built-in augmentation) trained on CIFAR-10, reaching ~83-86% test accuracy. Ships with a GitHub Actions pipeline that lints and smoke-tests the training script on every push.

**[NumPy MLP from Scratch](https://github.com/BiedrzyckiCoding/numpy-mlp-from-scratch)**
A multi-layer perceptron with forward pass, backpropagation, and gradient updates written by hand in NumPy, no PyTorch, no TensorFlow, no autograd. Wrapped in a Flask UI that walks through data loading, batch and online training, and evaluation, backed by 93 unit tests in CI. [Live demo](https://jakub-biedrzycki-mlp-from-scratch.vercel.app/).

**[Ball Tracker](https://github.com/BiedrzyckiCoding/ball_tracker)**
An OpenCV computer vision project that isolates a red ball by HSV color threshold, cleans the mask with morphological opening and closing, then tracks it frame by frame through video using image moments to find its centroid.

---

## Extracurricular Activities

**YNG Chapter Leader (YPO Next Generation)**
- Organizes professional events with high-performing individuals.
- Maintains strong member engagement and community relationships.
- Oversees budgeting and event planning to ensure efficient and successful chapter operations.

[yponextgen.org](https://www.yponextgen.org/)

---

## Socials

[![GitHub](https://img.shields.io/badge/GitHub-BiedrzyckiCoding-181717?style=flat&logo=github&logoColor=white)](https://github.com/BiedrzyckiCoding)
[![X](https://img.shields.io/badge/X-@jakubbied-000000?style=flat&logo=x&logoColor=white)](https://x.com/jakubbied)

---

## Languages

- Polish (Native)
- English (Fluent, C1)
- Japanese (Basic)

---

## Interests

AI/ML systems: training pipelines, embeddings and clustering, LLM summarisation, and agentic coding workflows.

Technical SEO: structured data, crawlable site architecture, and optimising for AI-citation crawlers.
