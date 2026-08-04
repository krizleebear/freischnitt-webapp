# Changelog

All notable changes to the **freischnitt** web application will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.0.0] - 2026-08-04

### Added
- **Guillotine Cutting Optimizer:** 2D sheet metal & woodworking cut optimization supporting kerf width, grain orientation, and multi-material projects.
- **Interactive Cut Visualizer:** Responsive A4/Desktop sheet diagram with blade cut dimensions, part color-coding, page flipping controls, and zoom.
- **Piece List Editor:** Inline table editing, duplicate piece actions, quick row delete, and keyboard shortcuts (`Enter` to save, `Esc` to cancel).
- **Mobile Workshop Mode:** Numpad measurement input, piece card stepper controls, mobile navigation drawer, and touch-optimized responsive layout.
- **Export & Print Capabilities:** One-click JSON project export/import, A4 vector SVG diagram download, high-resolution PDF export, and dedicated print layout.
- **Legal Compliance & Privacy:**
  - Anti-Spam Impressum & DSGVO privacy policy modal (§ 5 DDG, § 18 MStV) with obfuscated contact data.
  - In-app Open Source License modal displaying CC BY-NC-ND 4.0 application terms and MIT/ISC/Apache-2.0 third-party copyright notices.
- **Standalone Single-File HTML Distribution:** Production build bundled into a single, self-contained `index.html` file using `vite-plugin-singlefile` for offline & portable usage.
- **Brand Identity:** Official custom vector logo (`logo_freischnitt.svg`) with high-DPI SVG/PNG favicons and touch icons.

### Changed
- Refactored asset URLs to use relative paths (`./`) for seamless compatibility with GitHub Pages subpath hosting.
- Enhanced release pipeline to automatically strip sourcemaps (`.map`) and run Playwright E2E browser test verification on minified production builds.

### Fixed
- Prevented accidental double-tap viewport zooming on mobile touch devices.
- Fixed canvas layout math and header button positioning during mobile soft-keyboard invocation.
