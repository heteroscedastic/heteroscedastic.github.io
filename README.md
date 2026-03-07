# Stochastic Rambling

**Statistics of life and few other outliers !!**

Personal website and blog built with [Hugo](https://gohugo.io) and the [HugoBlox Academic](https://hugoblox.com) theme.

**Live site**: [heteroscedastic.github.io](https://heteroscedastic.github.io)

## Tech Stack

- [Hugo](https://gohugo.io) (Extended) — Static site generator
- [HugoBlox Academic](https://hugoblox.com) — Theme with resume, projects, publications, and blog
- [Tailwind CSS](https://tailwindcss.com) v4 — Styling
- [Pagefind](https://pagefind.app) — Full-text search
- GitHub Pages + GitHub Actions — Hosting and CI/CD

## Quick Start

```bash
# Install dependencies
pnpm install

# Start development server with live reload
pnpm dev
# or
hugo server --disableFastRender

# Build for production
pnpm build
# or
hugo --minify
```

Requires [Hugo Extended](https://gohugo.io/installation/) v0.156.0+ and [Node.js](https://nodejs.org) 20+.

## Project Structure

```
.
├── config/_default/       # Site configuration
│   ├── hugo.yaml          #   Hugo settings (baseURL, build options)
│   ├── params.yaml        #   Theme, colors, typography, header/footer
│   ├── menus.yaml         #   Navigation menu
│   ├── languages.yaml     #   Language settings
│   └── module.yaml        #   Hugo module imports
├── content/               # Site content (Markdown)
│   ├── _index.md          #   Homepage (landing page sections)
│   ├── blog/              #   Blog posts
│   ├── projects/          #   Project portfolio
│   ├── publications/      #   Academic publications
│   ├── events/            #   Talks and events
│   └── slides/            #   Presentation slides
├── data/authors/me.yaml   # Author profile (bio, experience, skills, education)
├── assets/media/          # Images and media files
├── static/uploads/        # Static files (resume PDF, etc.)
├── .github/workflows/     # GitHub Actions deployment
├── go.mod                 # Hugo module dependencies
└── hugoblox.yaml          # HugoBlox build/deploy config
```

## Customization

### Author Profile

Edit `data/authors/me.yaml` to update your name, bio, education, experience, skills, and social links.

### Theme & Colors

Edit `config/_default/params.yaml` under `hugoblox.theme`:

- **Mode**: `light`, `dark`, or `system` (follows OS preference)
- **Colors**: Set `primary` and `secondary` to any Tailwind palette name (e.g., `indigo`, `rose`, `emerald`) or hex value
- **Typography**: Choose `sans`, `serif`, or `native` fonts

The theme picker in the navbar lets visitors switch between color schemes.

### Navigation

Edit `config/_default/menus.yaml` to add, remove, or reorder menu items.

### Content

- **Blog posts**: Create a folder in `content/blog/` with an `index.md`
- **Projects**: Create a folder in `content/projects/` with an `index.md`
- **Publications**: Create a folder in `content/publications/` with an `index.md` and optional `cite.bib`

## Deployment

The site deploys automatically to GitHub Pages via GitHub Actions on every push to `main`.

**Setup**: In your GitHub repo, go to **Settings > Pages** and set the source to **GitHub Actions**.

## License

Content is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/). Theme is [MIT licensed](https://github.com/HugoBlox/kit/blob/main/LICENSE.md).
