# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.1.0] - 2022-02-17
### Changed
- Updated minimum WordPress version to `5.7`: https://codex.wordpress.org/Supported_Versions.
- Updated minimum PHP version to `7.4`: https://www.php.net/supported-versions.

## [1.0.0] - 2021-06-25
### Added
- Added `PHPCompatibilityWP` rule.
- Added `VariableAnalysis` rule.
- Added `WordPress` rule.
- Added `WordPressVIPMinimum` rule.
- Added `WordPress-VIP-Go` rule.
- Excluded `WordPress.Files.FileName.InvalidClassFileName` sniff.
- Excluded `WordPress.Files.FileName.NotHyphenatedLowercase` sniff.
- Added relative exclude pattern `^bower_components/*` for the `bower_components` folder.
- Added relative exclude pattern `^node_modules/*` for the `node_modules` folder.
- Added relative exclude pattern `^vendor/*` for the `vendor` folder.
- Added relative exclude pattern `^vendor-bin/*` for the `vendor-bin` folder.
- Added relative exclude pattern `^wordpress/*` for the `wordpress` folder.
- Added relative exclude pattern `^wp-content/*` for the `wp-content` folder.

[Unreleased]: https://github.com/pronamic/wp-coding-standards/compare/1.1.0...HEAD
[1.1.0]: https://github.com/pronamic/wp-coding-standards/compare/1.0.0...1.1.0
[1.0.0]: https://github.com/pronamic/wp-coding-standards/releases/tag/1.0.0
