# Aris: Infrastructure for the Post-PDF Era

**Building web-native tools for academic publishing.** Open source, community-governed, designed for developers and researchers.

<br>

## Our Projects

### [Scroll Press](https://github.com/aris-pub/press) — Modern Preprint Server
A web-native preprint server with format freedom. Publish from Typst, Quarto, MyST, Jupyter, or any tool that produces HTML.

**Tech:** FastAPI • PostgreSQL • HTMX • Jinja2
**Status:** Beta
**Links:** [Live Site](https://scroll.press) • [Examples](https://github.com/aris-pub/examples-press)

### [RSM Studio](https://github.com/aris-pub/studio) — Collaborative Editor
Reference implementation and collaborative editor for RSM (Readable Science Markup). Write semantic documents that preserve meaning and render beautifully everywhere.

**Tech:** Python • TypeScript • Collaborative Editing
**Status:** Development
**Links:** [Live Site](https://rsm.studio)

### [RSM](https://github.com/aris-pub/rsm) — Readable Science Markup
The markup language powering semantic, portable academic documents. Lightweight syntax with rich mathematical and scientific notation support.

**Tech:** Python • Tree-sitter
**Status:** Active Development

<br>

## Quick Start

### Try Press with Example Papers
```bash
git clone https://github.com/aris-pub/examples-press.git
cd examples-press

# Try the Typst example
cd typst
pandoc spectral_theorem.typ -s -o spectral_theorem.html --mathml

# Try the Quarto example
cd ../quarto
quarto render iris_analysis.qmd

# Try the Jupyter example
cd ../jupyter
jupyter nbconvert --to html particle_physics.ipynb --embed-images

# Try the RSM example
cd ../rsm
pip install rsm-markup==0.4.1
uv run rsm-build damped_oscillators.rsm --css damped_oscillators.css --standalone -o damped_oscillators
```

### Run Press Locally
```bash
git clone https://github.com/aris-pub/press.git
cd press
cp .env.example .env  # Configure DATABASE_URL
just init             # Setup and seed database
just dev              # Start development server
```

<br>

## Our Principles

Every tool we build follows these foundations:

**Universal** — Works on any device, for any user. No platform lock-ins. Portable, accessible.

**Transparent** — Built on open standards. Everything is exportable and versionable. You own your work completely.

**Interactive** — Research is conversation. Enable dialogue, feedback, and knowledge that builds over time.

**Inviting** — Beautiful, effortless developer experiences. Well-documented APIs, clear architecture, intuitive patterns.

<br>

## Contributing

We welcome contributions across all projects:

- **Press**: Fully community-owned. All contributions welcome — features, bug fixes, documentation.
- **Studio**: Community-maintained reference implementation. Bug reports and maintenance contributions accepted.
- **RSM**: Core language development. Proposals and improvements welcome.

See individual repository `CONTRIBUTING.md` files for specific guidelines.

<br>

## Tech Stack Highlights

- **Backend**: FastAPI, SQLAlchemy 2.0 async, PostgreSQL, Alembic
- **Frontend**: HTMX, Jinja2 components, vanilla JS, modern CSS
- **Testing**: pytest-asyncio, Playwright, httpx
- **Infrastructure**: Fly.io, Supabase, GitHub Actions
- **Dev Tools**: uv, just, ruff, pre-commit hooks

<br>

## Governance

**Press** is fully community-owned — open source with shared governance, forever free.

**Studio** and **RSM** are community-maintained reference implementations, with bug reports and maintenance contributions accepted.

We're supported by community donations and academic grants, not venture capital. This funding model lets us prioritize researcher and developer needs over investor returns.

<br>

## Community

- **Zulip Chat**: [aris-pub.zulipchat.com](https://aris-pub.zulipchat.com/) — Real-time discussions, support, architecture decisions
- **Blog**: [aris.pub/blog](https://aris.pub/blog) — Development updates, technical deep-dives
- **Email**: [hello@aris.pub](mailto:hello@aris.pub) — Direct contact

<br>

## Philosophy

Academic publishing is trapped in formats designed for paper, not pixels. We're building the infrastructure for how research should work in the digital age: accessible everywhere, preserving context, enabling real collaboration.

LaTeX and PDF were revolutionary for print. It's time to build the next generation of tools for the web.

<br>

---

<div align="center">

**Building tools as thoughtful as the knowledge they preserve.**

[Browse Projects](https://github.com/orgs/aris-pub/repositories) • [Join Community](https://aris-pub.zulipchat.com/) • [Visit aris.pub](https://aris.pub)

</div>
