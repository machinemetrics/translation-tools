# translation-tools
Tools for exporting and importing translations

This is built on this package:
https://jy95.github.io/i18n-tools/

# Setup
1. Install i18-tools:

`npm i -g @jy95/i18n-tools`

2. All settings here in `translation-tools` require absolute paths. I currently have these hard-coded to the paths on my own file system.  You'll need to comb through them and update to your own paths. If anyone else would like to add support for this to be dynamic, be my guest!

# To Export

`npx @jy95/i18n-tools export to_xlsx --settings ~/Code/translation-tools/opdash/export/settings.json`

This outputs an excel file into `translation-tools/opdash`.

# To Import

`npx @jy95/i18n-tools import from_xlsx --settings ~/Code/translation-tools/opdash/import/settings.json`

This outputs new en.json, fr.json, etc, files _directly into the locales directory in _~/Code/OperatorView_

**Note**: importing will currently be incorrect as it uses the keySeparator `.`, so divides on periods in our keys.  In op dash we use `|`.  I filed an issue for them to add support.... we'll see what they do and if not I can fork it or create a PR for that functionality.
