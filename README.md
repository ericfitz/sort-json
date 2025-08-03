# sort_json.py

(c) 2025 by Eric Fitzgerald (github@efitz.net), all rights reserved, Apache 2.0 license

Sort JSON file(s), maintaining hierarchy, and optionally compare with other files.

Backups are automatically created before overwriting files; the backups are stored in $TMPDIR

## Requirements

- Requires Python 3.6+ (uses f-strings)
- Uses only standard library modules; no extra packages needed

## Purpose

I wrote this to help me keep multiple localization files in sync. By sorting but maintaining hierarchy, we can do a line by line comparison.

## Known Limitations

Does not support JSONC or JSON5 - it doesn't know what to do with comments

## Usage
```
Examples:
  python3 sort_json.py config.json                      # Sort config.json
  python3 sort_json.py config.json --diff other.json    # Sort both files and compare other.json with config.json
  python3 sort_json.py config.json --diff *.json        # Sort all JSON files and compare each file in diff with config.json
  python3 sort_json.py config.json --dry-run            # Show what would be done
```
