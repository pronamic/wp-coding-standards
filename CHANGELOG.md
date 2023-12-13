# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [2.1.0] - 2023-12-13
- Updated to `PHPCSStandards/PHP_CodeSniffer` version `3.8`: https://github.com/PHPCSStandards/PHP_CodeSniffer/releases/tag/3.8.0.
- Increased minimum WordPress version to `6.2`.
- Increased minimum PHP version to `8.1`.

## [2.0.2] - 2023-11-02
- Added `<rule ref="Generic.Arrays.DisallowLongArraySyntax" />`.

## [2.0.1] - 2023-09-11
- Changed config `minimum_supported_version` to `minimum_wp_version`: https://github.com/WordPress/WordPress-Coding-Standards/wiki/Customizable-sniff-properties.

## [2.0.0] - 2023-09-05
- Update to WordPress coding standards version `3.0.0`: https://github.com/WordPress/WordPress-Coding-Standards/releases/tag/3.0.0.
- Update to WordPress VIP coding standards version `3.0.0`: https://github.com/Automattic/VIP-Coding-Standards/releases/tag/3.0.0
- Increased minimum WordPress version to `6.1`.
- Increased minimum PHP version to `8.0`.

## [1.3.1] - 2023-01-31
- For now allow PHP `7.4`.

## [1.3.0] - 2022-12-01
### Changed
- Updated minimum WordPress version to `5.9`: https://codex.wordpress.org/Supported_Versions.
- Updated minimum PHP version to `8.0`: https://www.php.net/supported-versions.

### Fixed
- Error trim(): Passing null to parameter #1 ($string) of type string is deprecated on PHP 8.1. [#1](https://github.com/pronamic/wp-coding-standards/issues/1)

## [1.2.0] - 2022-04-12
### Changed
- We deviate from the WordPress Coding Standards and switch to the short array syntax.

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

[Unreleased]: https://github.com/pronamic/wp-coding-standards/compare/2.0.3...HEAD
[2.0.3]: https://github.com/pronamic/wp-coding-standards/compare/2.0.2...2.0.3
[2.0.2]: https://github.com/pronamic/wp-coding-standards/compare/2.0.1...2.0.2
[2.0.1]: https://github.com/pronamic/wp-coding-standards/compare/2.0.0...2.0.1
[2.0.0]: https://github.com/pronamic/wp-coding-standards/compare/1.3.0...2.0.0
[1.3.0]: https://github.com/pronamic/wp-coding-standards/compare/1.2.0...1.3.0
[1.2.0]: https://github.com/pronamic/wp-coding-standards/compare/1.1.0...1.2.0
[1.1.0]: https://github.com/pronamic/wp-coding-standards/compare/1.0.0...1.1.0
[1.0.0]: https://github.com/pronamic/wp-coding-standards/releases/tag/1.0.0
