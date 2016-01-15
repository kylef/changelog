# Changelog Specification

This document is a full specification of the changelog format.

## Filename

Changelogs should be stored in a filename called `CHANGELOG.md`.

## Version

A version is indicated by a subheading followed by the version name.

```markdown
## 1.0.0
```

A released version may contain a date in the ISO8601 standard using UTC.
The date must be contained within round brackets:

```markdown
## 1.0.0 (2016-01-09)
```

A version may also contain a short summary.

```markdown
## 1.0.0 (2016-01-09)

Initial release of Curassow.
```

## Section

Within a version, you may define sections to group individual change entries
together via subheadings. For example, to create a section called "Bug Fixes":

```markdown
### Bug Fixes
```

You MAY define your own sections with any name. It is recommended that you use
the section names defined below so that tooling can understand the semantic
meaning of changes.

- Breaking - Indicates a change that is backwards incompatible and breaks the
  existing behaviour.
- Enhancements - New functionality that is introduced.
- Bug Fixes - Backwards compatible bug fixes.

## Change Entry

A change entry is in the form of a markdown list.

```markdown
* My change
```

Each entry is markdown, so it may contain any form of valid markdown such as
links.

It is recommended that you contain the author of the change along with
any related issues. For example:

```markdown
* Explicitly inform the user to close existing project when switching to
  a workspace for the first time.  
  [Kyle Fuller](https://github.com/kylef)
  [#2996](https://github.com/CocoaPods/CocoaPods/issues/2996)
```

Or, rendered:

> * Explicitly inform the user to close existing project when switching to
>   a workspace for the first time.  
>   [Kyle Fuller](https://github.com/kylef)
>   [#2996](https://github.com/CocoaPods/CocoaPods/issues/2996)
