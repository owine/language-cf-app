# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a simple single-page web application that generates custom language preference formats for Sonarr/Radarr media management applications. The entire application is contained in a single HTML file (`index.html`) with embedded CSS and JavaScript.

## Application Architecture

The application consists of:
- A web interface for selecting and ordering preferred languages
- JavaScript functions that generate JSON custom format specifications
- A scoring system that assigns higher scores to more preferred languages (position-based: first choice gets highest score)

## Key Functions

- `addLanguageField()` - Dynamically adds new language selection dropdowns
- `generateFormat()` - Creates the JSON custom format specification based on selected languages
- `getLanguageName()` - Maps language codes to human-readable names

## Development

Since this is a static HTML application with no build process:
- Open `index.html` directly in a web browser to test
- No package manager, build tools, or dependencies required
- All code is self-contained in the single HTML file

## Custom Format Output

The application generates JSON in the format expected by Sonarr/Radarr custom formats, with specifications that include language codes and preference scores calculated based on user-defined priority order.