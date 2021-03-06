---
title: Known Limitations
page_title: Known Limitations | RadClientExportManager for ASP.NET AJAX Documentation
description: Known Limitations
slug: clientexportmanager/functionality/known-limitations
tags: known,limitations
published: True
position: 3
---

# Known Limitations



## Known Limitations

The **RadClientExportManager** control's known limitations are listed below:

* no rendering of shadow DOM

* no CSS box-shadow, text-shadow, gradients

* only **solid** border-style

* the content of the following elements is not rendered: `<iframe>`, `<svg>`, `<input>`, `<textarea>`, `<select>`. A `<canvas>` will be rendered as an image, but only if it's "non-tainted" (does not display images from another domain). An .svg image can be exported if its URL is set in the "src" attribute of an `<img>` element.

* images hosted on different domains might not be rendered, unless permissive [Cross-Origin HTTP headers](https://developer.mozilla.org/en-US/docs/Web/HTML/CORS_enabled_image) are provided by the server. Similarly, fonts might not be possible to load cross-domain.

* when the generated document is opened with Acrobat Reader and you try to use the **Save As** option from the file menu an error is thrown. "The document could not be saved. There was a problem reading(23)". The solution is to open Acrobat Reader options (Edit → Preferences) and in the "Documents" section uncheck “Save As optimizes for Fast Web View”, which is enabled by default. After this, **Save As** will work without errors.



# See Also
