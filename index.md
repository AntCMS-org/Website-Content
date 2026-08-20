--AntCMS--
Title: AntCMS
Author: The AntCMS Team
Description: AntCMS is a very fast CMS which provides easy SEO, low system resource usage, and makes writing content easy utilizing Markdown. 
NavItem: true
--AntCMS--

# AntCMS
**High-performance flat-file CMS designed for speed.**

AntCMS is a lightweight, flat-file CMS that's designed to be powerful, inexpensive on system resources, blazingly fast, and to do so without requiring you to configure it.

---

## Core Features

### ⚡ Performance & Optimization
*   **Blazing Fast:** Optimized for extreme speed with zero manual tuning required.
*   **Low Overhead:** Engineered to run efficiently on even the most modest server hardware.
*   **Smart Caching:** Automatic use of **ETags** during asset delivery to maximize client-side caching.

### 🛠️ Built-in Automation
*   **Auto-Compression:** Native support for `gzip`, `brotli`, and `zstd`.
*   **Asset Management:** Automatically compresses text-based assets (JS, HTML, CSS) and common image formats (JPEG, JPG, PNG, WEBP).
*   **SEO Ready:** Automated handling of `robots.txt` and `sitemap.xml` files for out-of-the-box visibility.

### 🎨 Content & Customization
*   **Simple Workflow:** Write content in **Markdown** and manage configuration via **YAML**.
*   **Theme Support:** Fully customizable themes with support for unique styles applied specifically to Markdown content.
*   **Extensible:** A robust plugin system allows you to expand functionality as your site grows.

---

## Minimum Requirements
To run AntCMS, your server must meet the following minimum requirements:
- **PHP Version:** 8.2 or higher
- **Required Extensions:** `curl`, `dom`, `mbstring`

### Recommended Extensions for Performance
For those looking to squeeze every bit of performance out of their instance, we recommend installing the following additional PHP extensions:

| Extension | Purpose |
| :--- | :--- |
| `zstd` | High-performance Zstandard compression |
| `brotli` | Advanced Brotli compression |
| `zlib` | Standard Gzip / Deflate support |
| `gd` | Enhanced automatic image processing |
| `opcache` | Optimizes PHP execution and enables advanced caching features. |
| `ctype` | Core type checking functionality |

---

[Explore the Documentation](#) • [View on GitHub](#) • [Get Started](#)