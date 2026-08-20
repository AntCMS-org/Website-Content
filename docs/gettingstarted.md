--AntCMS--
Title: Getting Started
Author: The AntCMS Team
Description: Getting started with AntCMS.
--AntCMS--

# Getting Started with AntCMS

Due to its streamlined architecture, getting started with AntCMS is straightforward compared to many traditional CMS solutions. Follow the guide below to get your site up and running quickly.

---

## Installing AntCMS

> **Note:** AntCMS is currently in active development (Alpha). While it is highly performant and stable for standard use, please be aware that new features are still being integrated.

1.  **Verify Environment:** Ensure your server runs PHP 8.2 or greater with `curl`, `dom`, and `mbstring` enabled.
2.  **Download & Extract:** Download the [latest release](https://github.com/AntCMS-org/AntCMS/releases) and extract it to your preferred directory.
3.  **Configure Web Server:** If required, apply the [correct configuration](https://github.com/AntCMS-org/AntCMS/blob/main/configs) for your specific web server environment.
4.  **Initialize:** Access your domain via a browser. AntCMS will automatically generate its initial configuration file upon first access.
5.  **Complete:** You are ready to begin creating content!

---

## Creating Content

AntCMS utilizes **Markdown** for content creation, supporting most standard extensions including emojis and GitHub-flavored markdown elements.

### File Structure
All content is stored in the `/Content` directory as `.md` files. You can organize these into subfolders:
*   *Example:* `/Content/docs/gettingstarted.md` will be accessible via `example.com/docs/gettingstarted`.

### Page Headers (Required)
Every page must include a header block at the top of the file so AntCMS can extract essential metadata. 

```yaml
--AntCMS--
Title: An Example!
Author: The AntCMS Team
Description: Getting started with content creation.
--AntCMS--
```

### Navigation & Organization

To customize the navigation bar, rename dropdown items, or manually set the order of pages, create a meta.yaml file within your directory:
```yaml
# Sets the title of the dropdown menu
title: 'Documentation'

# Overrides the automatically selected order
pageOrder:
  gettingstarted: 1
  webservers: 2
  markdown: 3
```