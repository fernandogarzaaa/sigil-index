# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added / Changed
- Site accessibility: sortable headers and badge rows are keyboard-operable (Tab + Enter/Space) with `aria-sort` and visible focus rings; the detail dialog moves focus to Close and restores it on exit; muted text meets WCAG AA contrast in light and dark mode; result count is announced (`aria-live`); detail dialog is full-screen on narrow phones
- Site robustness: if `index.json` cannot be fetched, search and the risk filter now filter the server-rendered rows instead of blanking the table
- Dependabot config for GitHub Actions (weekly)
- SECURITY.md with private reporting contact
- `npm test`: zero-dependency checks of every badge and revocation signature, tamper rejection, and docs freshness (`test/index.test.mjs`); `package.json` with `test` / `build` / `validate` scripts
- README: how to install the `sigil` CLI (`npm i -g sigil-mcp`), local checking commands, and the corrected "site stays current" flow (PR authors rebuild `docs/`)
