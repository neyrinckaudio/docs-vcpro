# V-Control Pro Documentation

This repository contains the complete user documentation for V-Control Pro, a macOS/Windows application that connects professional control surfaces to digital audio and video workstation applications.

## About V-Control Pro

V-Control Pro bridges the gap between legacy professional control surfaces (particularly Digidesign/Avid surfaces) and modern DAW applications. It enables users to continue using high-quality hardware controllers that are no longer officially supported, while also providing enhanced control for modern surfaces.

### Supported Control Surfaces

- **Legacy Digidesign/Avid Surfaces**: D-Command, C|24, Control 24, ProControl, Command 8, 003
- **Modern Surfaces**: PreSonus FaderPort series (V2, 8, 16), ioStation 24c
- **iPad Applications**: V-Console, V-Control Pro iPad App

### Supported Applications

- **Audio**: Pro Tools (all versions), Logic Pro, Cubase/Nuendo, Studio One, Ableton Live, Reaper, and many more
- **Video**: DaVinci Resolve, Premiere Pro
- **Game Audio**: FMOD Studio, Wwise

## Documentation Site

This repository uses [MkDocs Material](https://squidfunk.github.io/mkdocs-material/) to generate a comprehensive documentation website covering:

- Installation and setup guides
- Controller-specific configuration instructions  
- DAW/application integration tutorials
- Detailed feature compatibility matrices
- Troubleshooting guides

## Development Setup

### Prerequisites

- Python 3.7+ with pip
- MkDocs and MkDocs Material theme

### Installation

```bash
pip install mkdocs mkdocs-material mkdocs-include-markdown-plugin
```

### Local Development

```bash
# Serve documentation locally with live reload
mkdocs serve

# Build static site
mkdocs build
```

The development server will be available at `http://localhost:8000` with automatic reload when files change.

## Repository Structure

```
docs/                          # Main documentation content
├── feature-chart/            # Controller/DAW compatibility matrices
├── images/                   # Screenshots and diagrams
├── setup/                    # DAW-specific setup guides (HTML)
├── stylesheets/             # Custom CSS
└── js/                      # Custom JavaScript

original-feature-charts/       # Source Excel files for feature data
mkdocs.yml                    # Site configuration and navigation
deploy.sh                     # Automated deployment script
```

## Deployment

The site can be deployed using the included deployment script:

```bash
./deploy.sh
```

This script will:
1. Build the MkDocs site
2. Commit changes to git
3. Push to the remote repository

## Contributing

When adding or updating documentation:

1. Follow the existing Markdown formatting conventions
2. Add new pages to the navigation structure in `mkdocs.yml`
3. Place images in `docs/images/` directory
4. Use the Material for MkDocs extensions for enhanced formatting (admonitions, tabs, etc.)
5. Test locally with `mkdocs serve` before deploying

## Feature Charts

The detailed compatibility matrices are generated from Excel files in `original-feature-charts/`. These show exactly which features work with each controller/DAW combination and are a key reference for users choosing compatible setups.
