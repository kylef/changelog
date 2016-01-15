# Changelog

A formal specification for changelog files and entries.

## Quick Links

- [Specification](Specification.md)

## Rationale and Goals

The primary goal around the changelog specification is to formalise a structure
for changelog files to bring consistency across projects.

A formal specification around changelogs may also allow automation via tools.
Tools can understand semantics around changes, whether a change is breaking, an
enhancement or a bug fix and automatically determine the next appropriate
[semantic version](http://semver.org) number. Along with dealing with any
manual tasks around changelog management.

## Examples

A small example changelog entry:

```markdown
## 0.2.0

### Enhancements

* Adds support for versions of Swift included in Xcode.
* Added `swiftenv --help`.
```

Or rendered as markdown:

> ## 0.2.0
> ### Enhancements
> * Adds support for versions of Swift included in Xcode.
> * Added `swiftenv --help`.

### Examples Elsewhere

You can find examples of changelogs in the wild in the following projects:

- [swiftenv](https://github.com/kylef/swiftenv/blob/master/CHANGELOG.md)
- [CocoaPods](https://github.com/CocoaPods/CocoaPods/blob/master/CHANGELOG.md)
- [Xcodeproj](https://github.com/CocoaPods/Xcodeproj/blob/master/CHANGELOG.md)
- [Jekyll](https://github.com/jekyll/jekyll/blob/master/History.markdown)

### Parsers & Generators

Interested in programmatically reading or manipulating your changelog?

- [Golang: parkr/changelog](https://github.com/parkr/changelog)
