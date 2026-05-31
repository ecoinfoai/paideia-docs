# paideia-docs

Public documentation site for **[paideia](https://github.com/ecoinfoai/paideia)** —
a full-cycle data system for running a single course over one semester
(pre-diagnosis → exam authoring → result interpretation → retrospective).

📖 **Published site:** https://ecoinfoai.github.io/paideia-docs/

This repository holds only the documentation sources. The paideia code lives in
the private `ecoinfoai/paideia` repository; the docs are mirrored here so they can
be published with GitHub Pages.

## Local preview

```bash
pip install -r requirements.txt
mkdocs serve            # http://127.0.0.1:8000
```

## How it is published

A push to `main` triggers `.github/workflows/docs.yml`, which builds the site with
MkDocs Material (`mkdocs build --strict`) and deploys it to GitHub Pages.

## Updating the docs

The authoring source is `ecoinfoai/paideia` under its `docs/` directory. Copy the
updated `docs/` and `mkdocs.yml` here and push to `main` to republish.
