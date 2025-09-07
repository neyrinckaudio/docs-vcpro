# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a MkDocs Material documentation site for V-Control Pro, a macOS/Windows application that connects control surfaces to digital audio and video workstation applications. The documentation covers setup, configuration, and feature compatibility for various control surfaces (legacy Digidesign/Avid surfaces, PreSonus FaderPort series) with different DAW applications.

## Build Commands

- **Build documentation site**: `mkdocs build`
- **Serve locally for development**: `mkdocs serve`
- **Deploy**: `./deploy.sh` (builds, commits, and pushes changes automatically)

## Repository Structure

- `docs/` - Main documentation content in Markdown format
- `docs/feature-chart/` - Compatibility matrices between controllers and DAWs
- `docs/setup/` - HTML setup files for various DAW integrations  
- `docs/images/` - Screenshots and diagrams
- `original-feature-charts/` - Source Excel files for feature compatibility data
- `mkdocs.yml` - MkDocs configuration with navigation structure and theme settings
- `deploy.sh` - Automated build and deployment script

## Content Architecture

The documentation is organized into major sections:
1. **Getting Started** - Installation, requirements, quick start
2. **Surface Setup** - Controller-specific configuration guides
3. **DAW/Application Setup** - Software-specific integration guides
4. **Feature Charts** - Detailed compatibility matrices showing which features work with which controller/DAW combinations

## Key Files

- `mkdocs.yml` - Defines the complete site navigation structure and Material theme configuration
- `docs/index.md` - Homepage introducing V-Control Pro and its supported surfaces
- `docs/feature-charts.md` - Index page linking to all compatibility matrices
- Feature chart files follow naming pattern: `{controller}-{daw}.md` (e.g., `c24-logic.md`)

## MkDocs Configuration

Uses Material theme with:
- Navigation tabs enabled
- TOC integration
- Include-markdown plugin for content reuse
- Custom CSS (`docs/stylesheets/extra.css`)
- Browser compatibility JavaScript (`docs/js/unsupported-browser.js`)

## Documentation Standards

- All content is in Markdown format
- Images stored in `docs/images/`
- Feature charts are generated from Excel files in `original-feature-charts/`
- Uses Material for MkDocs extensions (admonition, tabbed content, etc.)

### Content Guidelines

**Writing Style:**
- Use clear, concise language appropriate for technical users
- Structure content with logical flow from basic to advanced topics
- Include step-by-step procedures for complex tasks
- Use consistent formatting (numbered lists for procedures, bullet points for features/options)

**Troubleshooting Documentation:**
- Always start with a Quick Checklist for immediate help
- Organize by logical troubleshooting flow: update → licensing → connection → OS-specific → DAW-specific
- Use tabbed content (=== "Platform") for OS-specific instructions
- Include visual indicators (✓ ✗) to show connection status
- Cross-reference related setup guides
- End with "Still Need Help?" section for escalation

**MkDocs Material Features to Use:**
- Admonitions (!!! info, !!! warning, !!! note) for important callouts
- Tabbed content for platform-specific instructions
- Anchor links with descriptive IDs for easy navigation
- Code blocks with proper syntax highlighting
- Cross-references to related documentation sections

## Important Files

- `docs/troubleshooting.md` - Comprehensive troubleshooting guide with quick checklist and step-by-step procedures
- `docs/controllers-overview.md` - Controller setup reference
- `docs/v-control-pro-licensing.md` - Licensing information and procedures