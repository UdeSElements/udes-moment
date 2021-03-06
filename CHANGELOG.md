# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased - 3.0.0]
### Deleted (not done)
- Remove the `isMomentReady` property of UdeS.MomentImportMixin, witch is replaced
  by the `timestampMoment` property.
- Remove the deprecated `__dispatchEvent` function along with the 
`udes-moment-language-changed` event.


## [2.2.1] - 2018-09-07
### Changed
- Return an empty string when the date is invalid.

## [2.2.0] - 2018-05-04
### Added
- Add the `moment` function into the `UdeS.MomentMixin`.


## [2.1.1, 2.1.2, 2.1.3] - 2017-09-22
### Changed
- Update documentation for www.webcomponents.org.
- Use eslint-config-udes and add the pre-commit hook.
- Interval dates are now trimmed.


## [2.1.0] - 2017-09-20
### Added
- Add the `udes-moment-format-table` demo.
- Add the `UdeS.MomentMixin` and the `udes-moment-interval` component.
- Add the first version of package.json.
- Add the ESLint configuration.
- Add this CHANGELOG.md.

### Changed
- Deprecate the property `isMomentReady`, `__dispatchEvent` function  and the 
  `udes-moment-language-changed` event for the next major version.
- Fix the bug where the same language script was inserted at multiple times 
  inside the document.
- Fix the documentation and ESLint errors.
- Fix the devDependencies for the demo by adding the `paper-button` element.


## [2.0.0] - 2017-09-14 15:12:08
### Added
- First Polymer 2 version.
