# ziniuzheng.github.io

Source for my portfolio site: **[ziniuzheng.github.io](https://ziniuzheng.github.io)**

A single static page (HTML + CSS, no framework or build step) that showcases my projects with demo videos,
plus my skills, education and resume. It supports light and dark mode and is laid out for desktop and mobile.

**Featured projects**

- [ContextLens](https://github.com/ZiniuZheng/contextlens): a Chrome extension that explains, summarizes or rewrites selected text on any page with streaming LLM answers
- OnlineOrder: a Spring Boot + React food-ordering app deployed on AWS ECS Fargate with RDS

## Structure

```
index.html              # The whole page
styles.css              # Styles, with color tokens for light/dark mode
assets/                 # Demo videos, posters and screenshots
Ziniu_Zheng_Resume.pdf  # Resume linked from the page
```

## Running locally

```bash
python -m http.server 8000
```

Then open http://localhost:8000. Pushing to `main` deploys the site through GitHub Pages.
When `styles.css` changes, bump the `?v=` query on its `<link>` in `index.html` so browsers don't keep a cached copy.
