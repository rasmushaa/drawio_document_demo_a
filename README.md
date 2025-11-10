# Project repo for sub-component A

[![Docs](https://img.shields.io/badge/Architecture-Drawio-red.svg)](https://viewer.diagrams.net/?url=https://raw.githubusercontent.com/rasmushaa/drawio_document_demo_a/refs/heads/main/doc/arc.drawio)

## 📘 Overview

This repository demonstrates how to document your codebase using **Draw.io (diagrams.net)** — not just as static images, but as **live, interactive cloud diagrams**.

Instead of exporting `.drawio` files to `.svg` or `.png`, you can link directly to the diagram hosted in your repository.  
This approach keeps your documentation always up to date, interactive, and version-controlled alongside your code.

---

## 🧩 The Traditional Way

A typical workflow looks like this:

1. Create a `.drawio` file and edit it in VS Code using the **Draw.io Integration** extension.  
2. Export it as `.svg` into your documentation directory.  
3. Embed the exported image in your README or docs.

This works fine for smaller diagrams and scales reasonably well.  
However, it lacks the **interactivity** of the original multilayered diagram — and you must remember to re-export the static image every time you make changes.

This introduces unnecessary manual steps and prevents you from leveraging Draw.io’s full potential.

![image info](./doc/arc.svg)


## 🌐 Draw.io Viewer

A much better solution is to use the **Draw.io Viewer**, available at: `https://viewer.diagrams.net/?url=<your-file-location>`.  

This is a **cloud-based web application** provided by [diagrams.net](https://www.diagrams.net/), the same team behind the Draw.io desktop and VS Code extensions.  
It runs entirely in your browser — no installation or authentication required — and can load diagrams directly from any public URL (for example, from **GitHub**, **GitLab**, or **Google Cloud Storage**). It is the same application used to view exported `embedded url`-files from **Drawio desktop**.  

When you pass your `.drawio` file’s **raw file URL** to the viewer, it renders the full interactive diagram online.  
This means you can explore layers, follow embedded links, and view component-level connections — all without exporting to `.svg` or `.png`.

In this repository, the link points to the `./doc/arc.drawio` file located within **this same repo**.  
When you open it with the Draw.io Viewer, it fetches the diagram directly from GitHub and renders it as an interactive, layered visualization.

The best part is that the diagram **updates automatically** whenever the `.drawio` file is modified and the changes are **pushed to the remote repository**.  
There’s no need to re-export or manually update any static images.

> ⚠️ **Note:**  
> Always use the **Raw file URL** from GitHub — not the one visible in the repository’s file explorer.  
> The raw link is what allows the Draw.io Viewer to access and render your diagram directly.

For example the badge uses this code:
```
[![Docs](https://img.shields.io/badge/Architecture-Drawio-red.svg)](https://viewer.diagrams.net/?url=https://raw.githubusercontent.com/rasmushaa/drawio_document_demo_a/refs/heads/main/doc/arc.drawio)
```

You can open this directly in any browser, and the viewer will fetch the latest version of the diagram from your repository in real time.
This is ideal for keeping architecture diagrams and documentation interactive, automatically updated, and tightly integrated with your codebase.