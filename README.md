# EPUB Cover Fixer for reMarkable

A browser-based tool to automatically detect and fix common EPUB cover display issues for reMarkable devices. Runs entirely in your browser — no data is sent to any server.

## Features

- **Multi-file support**: Process multiple EPUB files simultaneously
- **Drag & drop interface**: Simply drag files or click to browse
- **Real-time analysis**: See issues detected before applying fixes
- **Privacy-focused**: All processing happens locally in your browser

## Issues Detected & Fixed

- **Directory structure**: Converts OEBPS directories to standard EPUB structure
- **Metadata problems**: Adds missing cover image identification in metadata
- **Missing attributes**: Adds `properties="cover-image"` to cover image items
- **Spine configuration**: Adds `linear="no"` to cover pages in reading order
- **File organization**: Moves cover images to `covers/` subdirectory
- **File extensions**: Standardizes `.jpeg` to `.jpg` extensions
- **HTML structure**: Simplifies complex div structures to clean figure/img elements

## Hosted Version

Use my hosted version at https://rm-covers.scottlabs.io/

## Run Yourself

1. Open `index.html` in your browser
2. Drag EPUB files onto the interface or click to browse
3. Click "Analyze All" to detect issues
4. Click "Fix All" to apply corrections
5. Download the corrected EPUB files

Compatible with both EPUB 2.0 and 3.0+ formats.
