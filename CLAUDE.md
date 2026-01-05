# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

```bash
# Setup
npm install                    # Install dependencies

# Build
npm run build                  # Build the project
npm run build:prod             # Build for production

# Testing
npm test                       # Run all tests
npm test -- path/to/test.js    # Run a single test file
npm test -- --watch            # Run tests in watch mode

# Linting and Formatting
npm run lint                   # Run linter
npm run lint:fix               # Fix linting issues
npm run format                 # Format code

# Running
npm run dev                    # Start development server
npm start                      # Start production server
```

## Architecture

### High-Level Structure
[Describe major directories and their purposes, e.g.:
- `src/core/` - Core business logic and domain models
- `src/api/` - API routes and controllers
- `src/services/` - External service integrations]

### Key Patterns
[Document architectural decisions that require understanding multiple files, e.g.:
- Uses repository pattern for data access
- Event-driven architecture with message queue
- Dependency injection via constructor parameters]

### Data Flow
[Explain how data moves through the system, e.g.:
- HTTP requests → Routes → Controllers → Services → Database
- WebSocket connections handled by EventEmitter pattern
- State management using Redux with async thunks]

### Important Conventions
[Note project-specific practices, e.g.:
- All database queries must use parameterized statements
- API responses follow JSend specification
- Feature flags checked via FeatureService.isEnabled()]
