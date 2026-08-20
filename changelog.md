--AntCMS--
Title: Changelog
Author: The AntCMS Team
Description: AntCMS's Release History and General Changelog
NavItem: true
--AntCMS--

# AntCMS Release History

---

## Preview Builds (Post-0.4.3)
*Ongoing development between releases*

**✨ New Features & Enhancements**
- **CLI System:** Introduced a CLI system for AntCMS which is modular and loads commands from plugins.
- **Markdown Support:** Added support for attributes within markdown content.
- **Cache Management:** Added new hooks for cache retrieval and optimized query key generation.

**🐛 Bug Fixes**
- **Page Ordering:** More fixes to the how page order is determined and a general cleaning of the related code.

**🛠 Improvements & Infrastructure**
- **Environment Integration:** Improved integration with the DDEV toolset.
- **Under the hood:** Improvements to code quality and style as well as regular dependency updates.

---

*Note: This section covers active development and hotfixes rolled out since the last major versioning.*

---

## Version 0.4.3
*Released: January 19, 2026*

**🐛 Bug Fixes**
- **PHP Compatibility:** Suppressed deprecation errors to resolve HTTP 500 issues when using PHP 8.5 with embedded content.

**⚙️ System Changes**
- **Architecture Migration:** Moved website content to its own repository ([Website-Content](https://github.com/AntCMS-org/Website-Content)).
- **GitHub Syncing:** We've introduced a new plugin [GitHub-Sync](https://github.com/AntCMS-org/GitHub-Sync) which will pull website content from a GitHub repository and automatically pull new changes.

---

## Version 0.4.2
*Released: January 6, 2026*

**✨ New Features**
- **Enhanced Cron:** Improved the Cron system to initialize plugins and trigger `onBeforeCronRun` and `onAfterCronRun` hooks.

**🐛 Bug Fixes**
- **Compatibility:** Updated output compression dependencies to ensure consistent performance across all modern browsers.

**⚙️ Maintenance**
- General code cleanup, styling improvements, and verified stability for PHP 8.5.

---

## Version 0.4.1
*Released: April 17, 2025*

**🐛 Bug Fixes**
- Resolved issues regarding asset and image compression functionality.

---

## Version 0.4.0
*Released: April 15, 2025*

**✨ New Features**
- **Advanced Hook System:** Introduced a new `Event` object for better tracking and parameter management.
- **Expanded Library:** Significantly increased the number of available hooks.
- **PHP Support:** Added official support for PHP 8.4.
- **Automated Assets:** Improved automated mapping of `/assets/` to active theme folders.
- **Dynamic Compression:** Enabled optional GET parameters for specifying custom image compression levels.

**🐛 Bug Fixes**
- Fixed ETag implementation for better browser caching.
- Corrected HTTPS redirection logic.

**⚙️ System Changes**
- Removed legacy support for PHP 8.1.
- Replaced internal `repairFilePath` functions with Symfony's FileSystem components.

---

## Version 0.3.0
*Released: May 27, 2024*

**✨ New Features**
- **SEO & Indexing:** Added capabilities for plugins to update `sitemap.xml` and `robots.txt`.
- **API Foundations:** Began implementation of API functionality for plugin developers.
- **Customization:** Introduced `imageQuality` configuration options.
- **Telemetry:** Hooks now track firing frequency and callback registration.

**⚙️ System Changes**
- Increased minimum PHP requirement to 8.1.
- Upgraded PHPStan scan level to 6 for improved type coverage.
- Streamlined vendor folders to reduce the overall system footprint.

---

## Version 0.2.0
*Released: May 7, 2024*

**✨ New Features**
- Introduced core Hook functionality.

**⚙️ Improvements**
- Optimized plugin implementation and documentation.
- Migrated to locally bundled/minified assets for faster performance.

---

## Version 0.1.1
*Released: May 1, 2024*

**🐛 Bug Fixes**
- Corrected issues where manual sorting orders were not being respected.

**⚙️ System Changes**
- Added OPcache "PHP Files" caching support.
- Implemented a tiered caching system (chained loading) to balance high-speed cache with filesystem fallbacks.

---

## Version 0.1.0
*Released: April 26, 2024*

**✨ Initial Launch Foundations**
- **Performance:** Reengineered the core engine for extreme speed and low memory overhead (~0.5 MB per page).
- **Native Features:** Built-in support for image, asset, and output compression.
- **Caching:** Automatic ETag tagging to ensure optimal browser caching from day one.

---
*Note: For detailed technical notes or to view the full commit history, visit the [Official Repository](https://github.com/AntCMS-org/AntCMS).*