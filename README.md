<div align="center">
<a href="https://svgl.app">
<img src="static/images/readme.png">
</a>
<p></p>
</div>

<div align="center">
    <a href="https://svgl.app" target="_blank">
        Discover
    </a>
    <span>&nbsp;✦&nbsp;</span>
    <a href="#-getting-started">
        Submit logo
    </a>
    <span>&nbsp;✦&nbsp;</span>
    <a href="#-terminal">
        Terminal
    </a>
    <span>&nbsp;✦&nbsp;</span>
    <a href="https://twitter.com/pheralb_">
        Contact
    </a>
    <span>&nbsp;✦&nbsp;</span>
    <a href="#%EF%B8%8F-contributing">
        Contributing
    </a>
</div>

</p>

<div align="center">

![Svelte Badge](https://img.shields.io/badge/Svelte-FF3E00?logo=svelte&logoColor=fff&style=flat)
[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fpheralb%2Fsvgl%2Fbadge%3Fref%3Dmain&style=flat)](https://actions-badge.atrox.dev/pheralb/svgl/goto?ref=main)
![GitHub stars](https://img.shields.io/github/stars/pheralb/svgl)
![GitHub issues](https://img.shields.io/github/issues/pheralb/svgl)
![GitHub forks](https://img.shields.io/github/forks/pheralb/svgl)
![GitHub PRs](https://img.shields.io/github/issues-pr/pheralb/svgl)
![Tailwind CSS Badge](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?logo=tailwindcss&logoColor=fff&style=flat)

</div>

## 🛠️ Stack

- [**Sveltekit**](https://kit.svelte.dev/) - Web development, streamlined.
- [**Typescript**](https://www.typescriptlang.org/) - JavaScript with syntax for types.
- [**mdsvex**](https://mdsvex.com/) - Markdown for Svelte apps.
- [**Shiki**](https://github.com/shikijs/shiki) - A beautiful Syntax Highlighter.
- [**Tailwindcss**](https://tailwindcss.com/) - A utility-first CSS framework for rapidly building custom designs.
- [**bits-ui**](https://www.bits-ui.com) - A collection of headless components for Svelte.
- [**clsx**](https://github.com/lukeed/clsx) + [**tailwind-merge**](https://github.com/dcastil/tailwind-merge) inspired by [shadcn/ui](https://ui.shadcn.com) - A tiny utility for constructing `className` strings conditionally.
- [**Prettier**](https://prettier.io/) + [prettier-plugin-tailwindcss](https://github.com/tailwindlabs/prettier-plugin-tailwindcss) - An opinionated code formatter.
- [**Lucide Icons**](https://lucide.dev/) + [**phosphor-svelte**](https://github.com/haruaki07/phosphor-svelte) - A clean and friendly icons libraries.
- [**svelte-sonner**](https://github.com/wobsoriano/svelte-sonner) - An opinionated toast component for Svelte.
- [**@upstash/redis** + **@upstash/ratelimit**](https://upstash.com/) - Serverless Redis for developers.
- [**Vitest**](https://vitest.dev/) - Blazing Fast Unit Test Framework.

## 🚀 Getting Started

> [!IMPORTANT]
> Before submitting the SVG, **make sure that you have permission** or that the license of the SVG allows you to add it to svgl. If you are not sure, please contact the company or author.

You will need:

- [Node.js 16+ (recommended 18 LTS)](https://nodejs.org/en/).
- [Git](https://git-scm.com/).

1. [Fork](https://github.com/pheralb/svgl/fork) this repository and clone it locally:

```bash
git clone git@github.com:your_username/svgl.git
```

2. Install dependencies:

```bash
# Install pnpm globally if you don't have it:
npm install -g pnpm

# and install dependencies:
pnpm install
```

3. Go to the [**`static/library`**](https://github.com/pheralb/svgl/blob/main/static/library) folder and add your `.svg` logo.

> [!WARNING]
>
> - Remember to optimize SVG for web, you can use [SVGOMG](https://jakearchibald.github.io/svgomg/).
> - The size limit for each .svg is **25kb**.

4. Go to the [**`src/data/svgs.ts`**](https://github.com/pheralb/svgl/blob/main/src/data/svgs.ts) and add the information about your logo, following the structure:

```json
{
  "title": "Title",
  "category": "Category",
  "route": "/library/your_logo.svg",
  "url": "Website"
},
```

or to support a different logo for light and dark themes:

```json
{
  "title": "Title",
  "category": "Category",
  "route": {
    "light": "/library/your_logo_light.svg",
    "dark": "/library/your_logo_dark.svg"
  },
  "url": "Website"
},
```

> [!NOTE]
> The list of categories is here: [`src/types/categories.ts`](https://github.com/pheralb/svgl/blob/main/src/types/categories.ts). You can add a new category if you need it.

And create a pull request with your logo 🚀.

5. (Optional) If you want to run the API locally, you will need to create a `.env` file in the root of the project with the following variables:

- [Create a Upstash account](https://console.upstash.com/).

```bash
SVGL_API_REQUESTS = 1
UPSTASH_REDIS_URL = ""
UPSTASH_REDIS_TOKEN = ""
```

## 💻 Terminal

SVG files can also be accessed directly from the terminal using [`svgls`](https://www.npmjs.com/package/svgls) CLI.

#### Quick start

If you are using yarn or npm, run this command:

```bash
npx svgls add
# or
pnpm dlx svgls add
```

For more details, check out the [GitHub repository](https://github.com/sujjeee/svgls) created by [sujjeee](https://twitter.com/sujjeeee).

## ✌️ Contributing

<a href="https://github.com/pheralb/svgl/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=pheralb/svgl" />
</a>

<p></p>

## 🔑 License

- [MIT](https://github.com/pheralb/svgl/blob/main/LICENSE).
