# Changelog

All notable changes to Code & Context will be documented in this file.

## [2025-01-06]

### Added

- Custom `/changelog` slash command for Claude to automatically generate changelog entries
  - Analyzes git status and recent commits
  - Formats entries according to project style
  - Supports options like `--commits` and `--since`
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

- Renamed site from "Shared Content Hub" to "Code & Context" to better reflect the site's philosophy and purpose
- Updated main hub page (`index.html`) to link to local `personal.html` instead of external GitHub Pages
- Added instruction in `CLAUDE.local.md` to never automatically remove sacred wording
- Reorganized personal.html content:
  - Moved "Effective Communication", "Thinking Clearly", and "Documentation as Code" from Thoughts to Principles section
  - Renamed "Thoughts" tab to "About" to better represent the "Why This Site" content
- Updated index.html philosophy section wording to "Code is communication. Context adds meaning."
- Added conditional "Back to Home" navigation to submodule pages:
  - Interface Design pages only show navigation when accessed via Code & Context
  - Tech Debt page only shows navigation when accessed via Code & Context
  - Uses JavaScript to detect `/share/content/` in URL path
- Widened Interface Design page container from `max-w-4xl` to `max-w-7xl` for consistency

### Technical Details

- Used Tailwind CSS for styling with custom CSS variables for theming
- Implemented tab switching with vanilla JavaScript
- Created hover effects and transitions for enhanced user experience
- Structured content to match the design pattern from previous "Personal Development" card style
