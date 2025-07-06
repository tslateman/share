# Changelog

All notable changes to the Shared Content Hub will be documented in this file.

## [2025-01-06]

### Added

- Created `personal.html` with card-based layout for personal development content
  - Implemented tabbed navigation (Core Values, Principles, Thoughts, Virtues)
  - Added three main value categories: Self, Social, and Impact
  - Included dark/light theme toggle functionality
  - Made design responsive for mobile and desktop
- Added "A Note on Honesty" section acknowledging AI assistance in site creation
- Documented wordsmithing examples in `CLAUDE.local.md` as "sacred wording"
  - Original choppy text: "Define good. The answer often depends. Context is king."
  - Selected improvement: "Good means different things in different moments. Context shapes every judgment we make."

### Changed

- Updated main hub page (`index.html`) to link to local `personal.html` instead of external GitHub Pages
- Added instruction in `CLAUDE.local.md` to never automatically remove sacred wording

### Technical Details

- Used Tailwind CSS for styling with custom CSS variables for theming
- Implemented tab switching with vanilla JavaScript
- Created hover effects and transitions for enhanced user experience
- Structured content to match the design pattern from previous "Personal Development" card style
