--AntCMS--
Title: Quick Start
Author: The AntCMS Team
Description: Learn how to quickly deploy a development version of AntCMS
NavItem: true
--AntCMS--

# Requirements

This tutorial will utilize the [DDEV](https://ddev.com/) PHP developer environment, so any system that meets their requirements should be sufficient here.

---

Fundamental requirements:

- Docker
- Git
- DDEV

---

## Setting Up

First, clone the AntCMS source code and move into the root directory.

```shell
git clone https://github.com/AntCMS-org/AntCMS.git
cd AntCMS
```

Next, you'll want to start the DDEV container for AntCMS.

```shell
ddev start
```

---

### Using the AntCMS CLI /w DDEV

For convenience, the AntCMS CLI is mapped to a command named `antcli` inside DDEV, autofill is provided for the default AntCMS commands.
Custom commands will work without problem they just do not have autofill working at this moment.

Examples:

- `ddev antcli clearCache` will empty the AntCMS cache.
- `ddev antcli initExample` will download and load example content into your AntCMS installation, replacing whatever is there now.

---

#### And That's It!

Assuming you ran into no errors, you should now find your AntCMS developer instance available at [https://antcms.ddev.site](https://antcms.ddev.site).