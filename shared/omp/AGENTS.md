# Subtractive edits

Finish every cutover: migrate producers, callers, consumers, tests, and affected documentation. Delete the retired implementation and every reference to it, including wrappers, aliases, fallbacks, dead guards, disabled code, deprecation markers, and tombstone comments. Do not hide or bypass obsolete code instead of deleting it. Verify the old path is absent, the replacement works, and unrelated behavior still works.

When removing an idea from prose, remove its negations, contrasts, disclaimers, and references to the removal. Preserve the remaining meaning; the text must read as though the idea was never raised.

# Corrections

Skip apologies, self-reproach, excuses, and promises to improve. Report facts and the authorized correction concisely.

# Comments and documentation

Write self-documenting code. Comments are exceptional: tooling requirements or genuinely non-obvious contracts, invariants, and safety constraints. Preserve required documentation, including comments consumed by tooling. Update affected documentation without creating unsolicited documentation files.

# Checks

Never accommodate an implementation by adding suppressions, weakening checks or assertions, skipping tests, or removing validation, security, error handling, or data-loss protections. Surface conflicting requirements and report remaining exemptions.

Exercise changed behavior; add meaningful regression coverage for non-trivial logic. Remove temporary scaffolding. Distinguish source inspection from executable verification and report actual results and limitations.

# Commits

Check recent commit messages. Use Conventional Commits by default; follow the established convention in someone else's repository.

Separate actual changes by coherent, independently revertible purpose. Stage only the intended files or hunks, including necessary tests and documentation. Review staged content before committing; leave unrelated changes unstaged. A session is not automatically one commit.

# Defaults

Verify existing defaults in source, documentation, or runtime before specifying values. Omit settings that merely restate defaults.

# Naming

Use complete words for project-controlled names and identifiers; introduce no abbreviations or shortenings.

Represent namespaces through directory structure.

Use the fewest complete words for file and directory names, preferring one word. Obtain explicit approval before creating or renaming a file or directory to a multiword name. Hyphenated, underscored, and camel-cased names count as multiple words.

Preserve names required by a language, framework, external API, or tool.
