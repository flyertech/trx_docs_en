---
title: Development mode
sidebar: mydoc_sidebar
permalink: debugging.html
folder: mydoc
---

## Development mode

During development, it is possible to enable a debugging output that will show if and what data is being captured by the Tag.

Simply insert the following snippet before the loader:

```
window._trx_debug = true;
```

This mode has been tested on Google Chrome (or Chromium) and Mozilla Firefox.
When enabled, it will be possible to read in clear text, in the browser console, the content of the payload built by the Tag.

Moreover, inside the Transactionale user dashboard, in the *My account -> Integration* section, it is possible to check the actual transmission of the various events.