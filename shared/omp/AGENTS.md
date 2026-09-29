# Subtractive edits

When asked to remove an idea from prose, make the final text read as though that idea was never raised. Remove its negation, contrast, disclaimer, and references to the edit too. Preserve the remaining meaning.

When refactoring or retiring code, finish the cutover: migrate every caller, remove the superseded implementation and references to it, and update affected tests and documentation. Delete guards, fallbacks, wrappers, aliases, and comments whose only purpose was the old path; retain protections required by the surviving behavior or an explicit compatibility contract. Verify the old path is absent and unrelated behavior still works. Keep the edit within the requested scope.

# Corrections

Skip apologies, self-reproach such as "I should have", excuses, and promises to do better.

# Comments and documentation

Do not add comments or documentation by default. Add them when tooling requires them or when they explain a non-obvious API contract, invariant, or safety constraint. Avoid comments that merely restate the code.

# Commits

Before committing, check recent commit messages. Use Conventional Commits by default; in someone else's repository, follow its established convention.

# Defaults

Before setting an explicit option or default, verify its existing value in local source, documentation, or runtime. Omit settings that merely restate defaults.

# Naming

Use complete words for project-controlled names and identifiers. Introduce no abbreviations or shortenings.

Represent namespaces through directory structure rather than file or directory names.

Use the fewest complete words possible for file and directory names, preferring one word. Obtain explicit approval before creating or renaming a file or directory to a name containing more than one word. Hyphenated, underscored, and camel-cased names count as multiple words.

Preserve names required by a language, framework, external API, or tool; those are not project-controlled choices.
