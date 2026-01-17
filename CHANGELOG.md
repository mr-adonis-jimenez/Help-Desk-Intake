# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
- Comprehensive documentation suite
- CHANGELOG.md for version tracking
- API documentation for code functions
- Enhanced code comments and JSDoc

## [1.2.0] - 2026-01-17

### Changed
- Consolidated CI workflows for improved efficiency
- Updated linting configurations (ESLint, Stylelint, HTMLHint)
- Fixed security alert #7 by adding explicit permissions to ci.yml workflow

### Fixed
- Removed duplicate checkout step in pages.yml workflow
- Removed accidental pull_request trigger from lighthouse.yml
- Added name attributes to select elements for better accessibility

## [1.1.0] - 2026-01-10

### Added
- Pre-commit configuration for automated code quality checks
- Lighthouse CI integration for performance monitoring
- Consolidated CI workflow combining linting and testing

### Changed
- Refactored CI workflows to reduce redundancy
- Updated stylelint-config-standard from 36.0.1 to 39.0.1

### Security
- Updated dependencies via Dependabot
- Implemented automated security scanning

## [1.0.0] - 2025-12-31

### Added
- Initial release of Help Desk Intake & Ticket Tracker
- Ticket intake form with validation (name, email, category, priority, description)
- Ticket dashboard with status toggle (Open/Closed)
- CSV export functionality for reporting
- Local-first storage using localStorage
- Responsive design for mobile and desktop
- Priority indicators (Low, Medium, High) with color coding
- MIT License
- Security policy (SECURITY.md)
- Contributing guidelines (CONTRIBUTING.md)
- Architecture documentation (ARCHITECTURE.md)
- README with setup and usage instructions

### Technical Features
- Static HTML/CSS/JS application (no backend required)
- Browser-based localStorage for data persistence
- Client-side validation with user-friendly error messages
- UTF-8 BOM support for Excel-compatible CSV export
- Accessible form elements with proper labels
- ESLint, Stylelint, and HTMLHint integration
- GitHub Actions CI/CD pipeline
- GitHub Pages deployment

## Version History Notes

### Data Format
- Tickets are stored in localStorage under key: `hd:tickets:v1`
- Each ticket includes: id, date, name, email, category, priority, description, status
- Status values: "Open" or "Closed"
- Priority values: "Low", "Medium", or "High"

### Browser Compatibility
- Modern browsers with localStorage support required
- Tested on: Chrome, Firefox, Safari, Edge
- Mobile responsive design

[Unreleased]: https://github.com/mr-adonis-jimenez/Help-Desk-Intake/compare/v1.2.0...HEAD
[1.2.0]: https://github.com/mr-adonis-jimenez/Help-Desk-Intake/compare/v1.1.0...v1.2.0
[1.1.0]: https://github.com/mr-adonis-jimenez/Help-Desk-Intake/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/mr-adonis-jimenez/Help-Desk-Intake/releases/tag/v1.0.0
