# Changelog Command

Generate a changelog entry for recent changes. This command will:
1. Check git status for uncommitted changes
2. Review recent commits if specified
3. Format changes according to the changelog structure
4. Add proper date formatting
5. Follow the existing changelog style with sections for Added, Changed, Fixed, etc.

## Usage
- `/changelog` - Generate entry for current uncommitted changes
- `/changelog --commits 5` - Include last 5 commits in the changelog entry
- `/changelog --since yesterday` - Include commits since yesterday

## Changelog Format
The command will follow this structure:
```markdown
## [YYYY-MM-DD]

### Added

- New features or files

### Changed

- Modifications to existing functionality

### Fixed

- Bug fixes

### Technical Details

- Implementation notes
```

## Instructions
When executed:
1. First run `git status` to see current changes
2. Run `git diff` to understand what changed
3. If commits requested, run `git log --oneline -n [number]` or `git log --since="[date]"`
4. Analyze the changes and categorize them appropriately
5. Write clear, concise bullet points focusing on the "what" and "why"
6. Add blank lines after section headings for readability
7. Present the formatted changelog entry for the user to review
8. Ask if they want to append it to CHANGELOG.md or copy to clipboard