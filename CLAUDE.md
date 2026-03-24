# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A collection of standalone, self-contained HTML files — no build step, no dependencies, no package manager. Each file embeds its own CSS and JavaScript.

## Running the Project

Open any HTML file directly in a browser:
```
open tictactoe.html
open contact-form-snippet.html
```

## Files

- **tictactoe.html** — Two-player in-browser Tic Tac Toe with score tracking.
- **contact-form-snippet.html** — A contact form intended to be pasted into a WordPress.com Custom HTML block. Submits via `fetch()` to a [Formspree](https://formspree.io) endpoint. The placeholder `XXXXXXXX` in the `<form action>` must be replaced with the user's real Formspree form ID before use.

## Code Conventions

- All CSS is scoped inside the file's top-level wrapper element to avoid conflicts when embedded in third-party pages (e.g., `#cf-wrapper` in the contact form).
- JavaScript is written as IIFEs to avoid polluting the global scope.
- No external libraries or CDN links.

## Git Workflow

After every task that creates or modifies files: commit with a descriptive message and push to `origin main`.

GitHub repo: https://github.com/angielooperp/ClaudeCodeTest
