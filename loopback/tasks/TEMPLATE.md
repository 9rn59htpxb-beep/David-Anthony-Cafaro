# Task: [Short Title]

Write a short title that describes what you want done, e.g. "Fix login bug" or "Add dark mode".

## Summary

Write one or two sentences describing what needs to change and why.

## Affected Repository

- **Repo:** `9rn59htpxb-beep/` — add the repo name after the slash
- **Branch:** — leave blank to use the default branch, or write the branch name
- **Files (if known):** — list any specific files, or leave blank if unsure

## Type of Change

Check the box that best fits by replacing `[ ]` with `[x]`:

- [ ] Bug fix
- [ ] New feature
- [ ] Refactor / cleanup
- [ ] Documentation
- [ ] Dependency update
- [ ] Other: 

## Acceptance Criteria

List what must be true for this task to be considered done. Add more lines if needed.

1. 
2. 

## Steps

List the high-level steps needed. Fill this in before starting work. Add or remove lines as needed.

- [ ] 
- [ ] 
- [ ] Open pull request
- [ ] Owner review and merge

## Notes

Add any constraints, references, or context the agent should know. Leave blank if none.

## Status

Replace the word that matches the current state and delete the others:

`open` | `in-progress` | `blocked` | `done`

---

## Example (filled-in task)

# Task: Fix broken link on home page

## Summary

The "Contact Us" link on the home page returns a 404 error. Update it to point to the correct URL.

## Affected Repository

- **Repo:** `9rn59htpxb-beep/David-Anthony-Cafaro`
- **Branch:** main
- **Files (if known):** `src/pages/Home.tsx`

## Type of Change

- [x] Bug fix

## Acceptance Criteria

1. Clicking "Contact Us" on the home page loads the contact page without errors.
2. No other links on the page are broken.

## Steps

- [x] Identify the incorrect link in `Home.tsx`
- [x] Update the href to `/contact`
- [ ] Open pull request
- [ ] Owner review and merge

## Notes

The old URL was `/kontact` (typo). No design changes needed.

## Status

`in-progress`
