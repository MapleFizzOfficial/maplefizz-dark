# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.1.1] - 2025

### Fixed
- **Token Colors**: Fixed INI file string token scopes (`string.quoted.single.ini`, `string.quoted.double.ini`) to properly override general `string` scope
- **Scope Ordering**: Reordered token color rules to ensure more specific scopes take precedence over general ones
- **Syntax Highlighting**: Corrected INI file string foreground color to `#C0C0C0` (was previously overridden by user settings)

### Changed
- **Token Rules**: Moved INI-specific token rules before general string rules in `tokenColors` array for proper precedence

## [0.1.0] - 2025

### Added
- **Core Theme**: Initial release of MapleFizz Dark theme
- **Color Palette**: Implemented signature MapleFizz candy-plum palette
  - Background: `#121016` (deep mauve charcoal)
  - Primary Accent: `#6A103B` (maple plum)
  - Secondary Accent: `#FF2F92` (vibrant candy pink)
  - Highlight: `#DCF763` (warm yellow)
  - Foreground: `#E5E5E8` (soft white text)
- **UI Components**: Complete styling for all VS Code UI elements
  - Editor surfaces, sidebars, panels, tabs
  - Activity bar, status bar, breadcrumbs
  - Hover widgets, suggest widgets, peek views
  - Terminal ANSI colors
- **Syntax Highlighting**: Comprehensive token color rules for:
  - JavaScript/TypeScript
  - HTML/CSS/SCSS
  - Markdown
  - JSON
  - INI files
  - Regex patterns
- **Git Integration**: Git decoration colors for untracked, modified, deleted, and conflicting resources
- **Diagnostics**: Error, warning, and info foreground colors with overview ruler support

### Changed
- **Base Tone**: Replaced harsh blacks with rich mauve charcoal `#221C26`
- **Contrast**: Improved readability with refined text luminance and smoother focus transitions
- **Interactivity**: Enhanced hover and selection states using brand pink `#FF2F92`
- **Line Highlight**: Added subtle plum glow (`#22132640`) for active line visibility

### Fixed
- **Version Compatibility**: Resolved version mismatch with Cursor/VS Code (requires `^1.99.3`)
- **Search Terms**: Added additional keywords for better discoverability (fixes [#2](https://github.com/MapleFizzOfficial/maplefizz-dark/issues/2))
- **Badge Contrast**: Corrected badge foreground/background contrast
- **Status Bar**: Fixed folderless status bar visibility

---

[Unreleased]: https://github.com/MapleFizzOfficial/maplefizz-dark/compare/v0.1.1...HEAD
[0.1.1]: https://github.com/MapleFizzOfficial/maplefizz-dark/compare/v0.1.0...v0.1.1
[0.1.0]: https://github.com/MapleFizzOfficial/maplefizz-dark/releases/tag/v0.1.0