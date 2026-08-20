--AntCMS--
Title: Compatible web servers
Author: The AntCMS Team
Description: Learn about what Markdown syntax and features AntCMS supports.
--AntCMS--

# Compatible Web Servers

AntCMS is designed to be flexible across various server environments. Below are the details for supported web servers and deployment options.

---

## Apache, Litespeed, and OpenLitespeed
These servers are compatible with `.htaccess` files and should function automatically with AntCMS.

*   **Note:** If using **OpenLitespeed**, you must reload the service after making changes for the server to recognize the `.htaccess` file.

---

## NGINX
We provide a [pre-configured nginx.conf](https://github.com/AntCMS-org/AntCMS/blob/main/configs/nginx.conf) template for use with NGINX.

*   **Status:** Please note that this configuration is currently provided as a reference and has not yet been fully tested or validated in production environments.

---

## Caddy
AntCMS is proven to work successfully with the Caddy web server.

*   **Standard Configuration:** While standard Caddy behavior for PHP applications is compatible, it does not automatically include features like asset and image compression.
*   **Recommended Configuration:** For full functionality (including proper routing for assets), we provide a [pre-built caddyfile](https://github.com/AntCMS-org/AntCMS/blob/main/configs/caddyfile).

**Important Note:** ETags are currently incompatible with Caddy and are automatically disabled in this environment. Consequently, using Caddy will result in reduced caching capabilities for assets.

---

## Development Servers
The following environments are supported for local development:

*   **PHP Local Development Server:** Useful for quick testing (Note: does not include asset delivery).
*   **DDEV:** AntCMS includes a dedicated configuration for DDEV, allowing you to spin up a fully-functional development instance quickly.