# translation-tools
Tools for exporting and importing translations

This is built on this package:
https://jy95.github.io/i18n-tools/

# Setup
1. Install package:

`npm i -g @jy95/i18n-tools`

2. You will need to modify the contents of this package to indicate the absolute path to these files on your system.

(If anyone else would like to add support for this to be dynamic, be my guest)

# To Export

`npx @jy95/i18n-tools export to_xlsx --settings ~/Code/translation-tools/opdash/export/settings.json`

# To Import

`npx @jy95/i18n-tools import from_xlsx --settings ~/Code/translation-tools/opdash/import/settings.json`
