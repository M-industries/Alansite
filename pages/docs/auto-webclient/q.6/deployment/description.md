---
layout: doc
origin: auto-webclient
language: deployment
version: q.6
type: description
---

1. TOC
{:toc}

Images to be supplied to the client to customize its appearance:
- **favicon.ico**:         bookmark icon (required)
- **logo.png**:            94x94 logo to be displayed at login
- **logo-sideways.png**:   38x76 logo for the application sidebar

Note that logo's are resized to fit and should be supplied at 2x the specified
resolution or larger to be crsip on high dpi displays.

- **config.json**          Configuration options for the client.
 An example:

```json
{
	"include data in error log": true // include (potentially sensitive) data in error reports.
}
```
```js
support data deployment
	/'logo.png'   ( = optional )
	/'logo-sideways.png' ( = optional )
	/'favicon.ico'   ( = required )
	/'config.json' ( = optional )
	/'reports' (
		/ *
			/'type.txt'      ( = required )
			/'template.xlsx' ( = required )
			/'sys.tag'       ( = optional )
	)
conversions
```
