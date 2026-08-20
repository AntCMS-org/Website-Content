--AntCMS--
Title: Image Compression
Author: The AntCMS Team
Description: Learn about automated image compression functionally in AntCMS.
--AntCMS--

# Image Compression

AntCMS provides built-in functionality to automatically compress images upon delivery. 

### How it Works

This feature is automatically enabled when:
1. The **GD PHP extension** is installed on your server.
2. Asset delivery is handled directly by AntCMS (rather than exclusively by the web server).

To ensure performance, images are compressed and the result is stored in the AntCMS cache to be re-used upon future requests; **your original files remain untouched.**

---

## Supported Formats

AntCMS automatically detects and compresses the following formats:
*   JPEG / JPG
*   PNG
*   WEBP

## Default Settings

By default, all supported images are processed using a quality level of **85%**. This provides an ideal balance between visual fidelity and file size, though this value may be changed via the config file.

---

## Custom Quality Overrides

If you require a specific quality level for a particular image rather than the global default, you can override it by appending a `imageQuality` GET parameter to your asset URL.

| Level | Value | Example URL |
| :--- | :--- | :--- |
| **Very High** | 95% | `/assets/image.jpg?imageQuality=veryhigh` |
| **High** | 80% | `/assets/image.jpg?imageQuality=high` |
| **Medium** | 65% | `/assets/image.jpg?imageQuality=medium` |
| **Low** | 25% | `/assets/image.jpg?imageQuality=low` |
| **Very Low** | 0% | `/assets/image.jpg?imageQuality=verylow` |

---

## Visual Comparison

*Note: The following images demonstrate the effect of different quality parameters.*

### Default (85%, configurable)

![Default quality](/assets/exampleImage.jpg)

### Very High (95%)

![Very high quality preset](/assets/exampleImage.jpg?imageQuality=veryhigh)

### High (80%)

![High quality preset](/assets/exampleImage.jpg?imageQuality=high)

### Medium (65%)

![Medium quality preset](/assets/exampleImage.jpg?imageQuality=medium)

### Low (25%)

![Low quality preset](/assets/exampleImage.jpg?imageQuality=low)

### Very Low (0%)

![Very low quality preset](/assets/exampleImage.jpg?imageQuality=verylow)