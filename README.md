# Pronamic WordPress WordPress Coding Standards

Pronamic WordPress WordPress Coding Standards for PHP_CodeSniffer.

## PHP_CodeSniffer

https://github.com/squizlabs/PHP_CodeSniffer

### Arguments

https://github.com/squizlabs/PHP_CodeSniffer/wiki/Usage

#### `colors`

By default use colors in output.

```xml
<arg name="colors"/>
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

By default this package test PHP 5.6 and higher via the following setting:

```xml
<config name="testVersion" value="5.6-"/>
```

### PHPCompatibility

https://github.com/PHPCompatibility/PHPCompatibility

Required through `PHPCompatibilityWP`.

### WordPress

https://github.com/WordPress/WordPress-Coding-Standards

By default the minimum WordPress version to check is set to `4.7` via the following setting:

```xml
<config name="minimum_supported_wp_version" value="4.7" />
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

We often use the [PSR-4](https://www.php-fig.org/psr/psr-4/) autoloading mechanism and therefore deviate from it.
