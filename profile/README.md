# Invokable

## Support Discussions
Support is provided through sponsor-only [Discussions](https://github.com/orgs/invokable/discussions).  

## Package Versioning and Support Policy

### Semantic Versioning (SemVer)

All packages under the Invokable organization follow [Semantic Versioning](https://semver.org/) principles:

- **MAJOR** version (`X.0.0`): Incremented for incompatible API changes
- **MINOR** version (`0.X.0`): Incremented for backward-compatible functionality additions
- **PATCH** version (`0.0.X`): Incremented for backward-compatible bug fixes

### PHP and Laravel Version Support

Invokable packages align their PHP version support with Laravel's official support schedule. You can find the current Laravel version support status at [Laravel Releases](https://laravel.com/docs/releases).

- Laravel follows PHP's [official support schedule](https://www.php.net/supported-versions.php)
- Only actively supported PHP versions are maintained in the latest Laravel version
- When PHP versions reach end-of-life, support is dropped in subsequent Laravel releases

### Version Increment Policy for Dropping Support

When dropping support for older PHP or Laravel versions, we increment the **MINOR** version by `1`. For example:

- Current version: `1.2.0` (supports PHP 8.0+)
- After dropping PHP 8.0 support: `1.3.0` (supports PHP 8.1+)

This approach ensures that:
1. Older Laravel projects can still install compatible versions via Composer's version constraints
2. Projects using newer PHP/Laravel versions receive the latest features and improvements
3. Breaking changes are properly signaled without unnecessarily incrementing the major version
