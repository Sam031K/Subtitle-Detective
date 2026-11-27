# Subtitle-Detective
A native Jellyfin plugin that detects subtitle languages, corrects mislabeled subtitle tracks, and standardizes display names without modifying the original media files.
# Subtitle Detective

Subtitle Detective is a native Jellyfin plugin designed to automatically identify, correct, and organize subtitle tracks across movie, television, and anime libraries.

Instead of relying solely on potentially incorrect language metadata, Subtitle Detective analyzes actual subtitle content to determine the language, identify subtitle purpose, and generate clean, consistent display names.

All changes are applied within Jellyfin without modifying or remuxing the original media files.

## Features

- **Automatic Language Detection** — Identifies subtitle languages through content analysis rather than blindly trusting existing metadata.
- **Standardized Subtitle Naming** — Generates consistent and readable subtitle display names.
- **Subtitle Purpose Identification** — Recognizes Full Subtitles, Signs and Songs, Forced Subtitles, SDH, Commentary, and other qualifiers.
- **Text-Based Subtitle Support** — Supports formats such as SRT and ASS.
- **Image-Based Subtitle Support** — Supports PGS and VobSub through OCR-based analysis.
- **Smart Scanning** — Avoids unnecessary repeated analysis of previously processed subtitle tracks.
- **Season-Level Analysis** — Uses supporting evidence from other episodes within the same season when individual results are inconclusive.
- **Manual Review** — Allows users to inspect, approve, or skip uncertain results.
- **Automatic Title Cleanup** — Removes unnecessary release group names, encoder tags, and redundant metadata.
- **Library Management** — Browse and manage subtitle tracks across movies, series, seasons, and individual episodes.
- **Reversible Changes** — Restore original subtitle display names.
- **Non-Destructive Operation** — Original media files remain untouched.
- **Native Jellyfin Integration** — No separate Docker container or companion server required.

## Subtitle Naming Convention

Subtitle Detective follows a consistent naming structure:

`Language – Qualifiers – Format`

Examples:

- English – Full Subtitles – ASS
- English – Signs and Songs – Default – ASS
- Japanese – Full Subtitles – SRT
- Turkish – Forced – SRT
- French – SDH – PGS
- German – Commentary – SRT
- English – ASS

## Project Philosophy

Subtitle metadata should be accurate, consistent, readable, and trustworthy.

Subtitle Detective prioritizes actual content over unreliable metadata, avoids making unsupported language assignments, and provides manual review when automatic detection is inconclusive.

The ultimate goal is to make subtitle management as automatic, accurate, and non-destructive as possible.

## Development Status

Subtitle Detective is under active development. Language detection accuracy, subtitle classification, and support for complex subtitle tracks are continuously being improved. Contributions, bug reports, and suggestions are welcome.
