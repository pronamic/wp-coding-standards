# Pronamic WordPress Coding Standards

Pronamic WordPress Coding Standards for PHP_CodeSniffer.

## Versions

We try to provide support for the last 3 major releases of PHP and WordPress in our projects.

### PHP

- `8.3`
- `8.2`
- `8.1`

https://www.php.net/supported-versions.php

### WordPress

- `6.5`
- `6.4`
- `6.3`

https://codex.wordpress.org/WordPress_Versions

### Other

- https://make.wordpress.org/core/handbook/best-practices/browser-support/
- https://make.wordpress.org/core/handbook/references/php-compatibility-and-wordpress-versions/

## PHP_CodeSniffer

https://github.com/PHPCSStandards/PHP_CodeSniffer

### Arguments

https://github.com/PHPCSStandards/PHP_CodeSniffer/wiki/Usage

#### `colors`

By default use colors in output.

```xml
<arg name="colors" />
```

#### `extensions`

By default only check files with `php` extension:

```xml
<arg name="extensions" value="php" />
```

#### `parallel`

By default use `8` parallel processes.

```xml
<arg name="parallel" value="8" />
```

https://github.com/squizlabs/PHP_CodeSniffer/issues/1732

#### `sp`

By default show sniff codes in all reports.
By default show progress of the run.

```xml
<arg value="sp" />
```

## Rules

### PHPCompatibilityWP

https://github.com/PHPCompatibility/PHPCompatibilityWP

By default this package test PHP `8.1` and higher via the following setting:

```xml
<config name="testVersion" value="8.1-"/>
```

### PHPCompatibility

https://github.com/PHPCompatibility/PHPCompatibility

Required through `PHPCompatibilityWP`.

### WordPress

https://github.com/WordPress/WordPress-Coding-Standards

By default the minimum WordPress version to check is set to `6.3` via the following setting:

```xml
<config name="minimum_supported_wp_version" value="6.3" />
```

https://github.com/WordPress/WordPress-Coding-Standards/wiki/Customizable-sniff-properties#minimum-wp-version-to-check-for-usage-of-deprecated-functions-classes-and-function-parameters

### WordPressVIPMinimum

https://github.com/Automattic/VIP-Coding-Standards

### WordPress-VIP-Go

https://github.com/Automattic/VIP-Coding-Standards

### VariableAnalysis

https://github.com/sirbrillig/phpcs-variable-analysis

## Exclusions

### `WordPress.Files.FileName.InvalidClassFileName`

According to the WordPress PHP Coding Standards:

> Class file names should be based on the class name with `class-` prepended and the underscores in the class name replaced with hyphens, for example `WP_Error` becomes:
>
> ```
> class-wp-error.php
> ```

_Source:_ https://make.wordpress.org/core/handbook/best-practices/coding-standards/php/#naming-conventions

This sniff will check on this naming convention:

```
Class file names should be based on the class name with "class-" prepended. Expected class-test.php, but found Test.php.
```

We often use the [PSR-4](https://www.php-fig.org/psr/psr-4/) autoloading mechanism and therefore deviate from it.

### `WordPress.Files.FileName.NotHyphenatedLowercase`

According to the WordPress PHP Coding Standards:

> Files should be named descriptively using lowercase letters. Hyphens should separate words.
>
> ```
> my-plugin-name.php
> ```

_Source:_ https://make.wordpress.org/core/handbook/best-practices/coding-standards/php/#naming-conventions

```
Filenames should be all lowercase with hyphens as word separators. Expected test.php, but found Test.php.
```

We often use the [PSR-4](https://www.php-fig.org/psr/psr-4/) autoloading mechanism and therefore deviate from it.

### `Universal.Arrays.DisallowShortArraySyntax`

According to the WordPress PHP Coding Standards:

> Using long array syntax ( `array( 1, 2, 3 )` ) for declaring arrays is generally more readable than short array syntax ( `[ 1, 2, 3 ]` ), particularly for those with vision difficulties. Additionally, it’s much more descriptive for beginners.
> 
> Arrays must be declared using long array syntax.

_Source:_ https://developer.wordpress.org/coding-standards/wordpress-coding-standards/php/#declaring-arrays

[![Pronamic - Work with us](https://github.com/pronamic/brand-resources/blob/main/banners/pronamic-work-with-us-leaderboard-728x90%404x.png)](https://www.pronamic.eu/contact/)
