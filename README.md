# sort_json.py
(c) 2025 by Eric Fitzgerald (github@efitz.net), all rights reserved, Apache 2.0 license

Sort JSON file(s), maintaining hierarchy, and optionally compare with other files.

## Purpose
I wrote this to help me keep multiple localization files in sync.  By sorting but maintaining hierarchy, we can do a line by line comparison.

## Known Limitations
Does not support JSONC or JSON5 - it doesn't know what to do with comments

## Usage
```
Examples:
  config.json                          # Sort config.json
  config.json --diff other.json        # Sort both files and compare other.json with config.json
  config.json --diff *.json            # Sort all JSON files and compare each file in diff with config.json
  config.json --dry-run                # Show what would be done
  config.json --yolo                   # Sort and delete backup files
```
