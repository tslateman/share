# Code & Context

A centralized repository for shared content on personal development, interface design, and technical debt management.

## Overview

This repository serves as a home base for various knowledge resources and documentation, bringing together content from:
- Personal principles and values
- Programming interface design best practices
- Technical debt management strategies

## Structure

```
├── index.html                          # Main hub landing page
├── content/
│   ├── personal/                       # Git submodule: git@github.com:tslateman/site.git
│   │   └── *.md files                 # Values, principles, and thoughts
│   ├── interface-design/              # Git submodule: https://github.com/tslateman/interface-design
│   │   └── index.html                 # SCORE framework and best practices
│   └── tech-debt/                     # Git submodule: git@github.com:tslateman/tech-debt
│       └── index.html                 # Articles and management strategies
└── assets/                            # Shared assets (CSS, JS, images)
    ├── css/
    ├── js/
    └── images/
```

## Git Submodules

This repository uses git submodules to sync content from external repositories:

- **personal**: git@github.com:tslateman/site.git (deployed at https://tslateman.github.io/site/)
- **interface-design**: https://github.com/tslateman/interface-design
- **tech-debt**: git@github.com:tslateman/tech-debt

### Working with Submodules

When cloning this repository for the first time:
```bash
git clone --recursive https://github.com/tslateman/share.git
```

If you've already cloned without submodules:
```bash
git submodule init
git submodule update
```

To update submodules to their latest versions:
```bash
git submodule update --remote
```

## Content Areas

### Personal
Explores values, principles, and practices for effective work and life, including:
- Core values and guiding principles
- Thoughts on communication and clear thinking
- Documentation as code philosophy
- Virtues from Marcus Aurelius and programming

### Interface Design
Comprehensive guide to building better programming interfaces:
- The SCORE(D) framework
- Core design principles
- Common anti-patterns
- AI and intelligent interfaces
- Team adoption strategies

### Technical Debt
Resources for understanding and managing technical debt:
- Types of technical debt
- Measurement and tracking strategies
- Best practices for prevention and management
- AI's impact on technical debt

## Usage

Simply open `index.html` in a web browser to access the main hub. From there, you can navigate to the different content areas.

## Contributing

This is a personal knowledge repository, but suggestions and improvements are welcome through issues or pull requests.

## License

See LICENSE file for details.
