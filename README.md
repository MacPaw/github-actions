# Reusable GitHub Actions & Workflows

<p align="center">
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/githubactions/githubactions-original.svg" width=250, height=400>
</p>

## Repository contains reusable GitHub Actions workflows

This repository provides production-ready, reusable GitHub Actions workflows for Symfony PHP projects, consolidating best practices from MacPaw's public repositories.

### Workflows

All reusable workflows are located in `.github/workflows` folder

- [symfony-php-reusable.yml](.github/workflows/symfony-php-reusable.yml) - Comprehensive Symfony PHP quality checks and testing workflow
  - 🔍 **Code Quality** - PHPStan, PHPCS, PHP-CS-Fixer, Rector, Infection
  - 🧪 **Multi-Version Testing** - PHP 7.4-8.4, Symfony 4.4-7.3
  - 📊 **Code Coverage** - Xdebug + Codecov integration
  - 🎯 **Custom Matrix Exclusions** - Flexible version compatibility
  - 🔧 **Custom Config Files** - Custom configuration paths for all quality tools
  - ⚙️ **Configurable Thresholds** - Custom Infection MSI thresholds
  - ⚡ **Performance Optimized** - Parallel execution, intelligent caching
  - [📚 Detailed Documentation](docs/workflows/symfony-php-reusable.md)

- [release-reusable.yml](.github/workflows/release-reusable.yml) - Fully automated release workflow using semantic-release
  - 🤖 **Fully Automated** - No manual version bumping or changelog writing required
  - ✅ **Semantic Versioning** - Automatic version calculation from commit messages
  - 🏷️ **Auto Tag & Release** - Automatically creates tags and GitHub releases
  - 📝 **Auto-Generated Changelogs** - Beautiful, categorized release notes
  - 🎯 **Conventional Commits** - Based on conventional commit standards
  - 🔀 **Multi-Branch Support** - main/master, next, beta, alpha, maintenance branches
  - 🛡️ **Safe & Idempotent** - Won't create duplicate releases
  - 🧪 **Dry Run Mode** - Test releases without publishing
  - 🔑 **Secure Authentication** - Uses GH_TOKEN repository secret for release operations
  - [📚 Detailed Documentation](docs/workflows/release.md)

### Documentation

- [Symfony PHP Reusable Workflow](docs/workflows/symfony-php-reusable.md) - Complete workflow documentation with:
  - 📥 All input parameters and configuration options
  - 🚀 Multiple usage examples (basic, minimal, full, extended matrix)
  - 🔄 Workflow diagram and process details
  - 🎯 Matrix strategy and custom exclusions
  - 🛠️ Advanced features and optimizations
  - 🚨 Prerequisites and required configuration files
  - 🔧 Troubleshooting guide
  - 📊 Analysis of MacPaw's Symfony repositories
  - 📈 Best practices and recommendations

- [Release Workflow](docs/workflows/release.md) - Complete semantic-release documentation with:
  - 🤖 Fully automated release process using semantic-release
  - 📝 Conventional commits specification and examples
  - 🏷️ Automatic version calculation (feat → minor, fix → patch, BREAKING → major)
  - 🚀 Multiple usage examples (feature, bugfix, breaking changes, pre-releases)
  - 🔀 Multi-branch release channels (main, beta, alpha, maintenance)
  - 📊 Auto-generated categorized changelogs
  - 🧪 Dry run mode for testing releases
  - 🔑 GH_TOKEN secret configuration and setup guide
  - 🔐 GitHub App token support for organizations
  - 🎯 Fine-grained Personal Access Token (PAT) instructions
  - ⚙️ Configuration via .releaserc.json
  - 🔧 Comprehensive troubleshooting guide
  - 📋 Best practices for conventional commits
  - 🛠️ Advanced configuration and customization examples
  - 🔄 Migration guide from manual releases

### Contributing

Contributions are welcome! When adding new features:

1. Test across multiple PHP/Symfony version combinations
2. Update documentation to reflect changes
3. Maintain backward compatibility
4. Add usage examples
5. Update analysis documentation if adding new tools

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Security

For information about reporting security vulnerabilities, please see our [Security Policy](SECURITY.md).

### Resources

- [MacPaw GitHub Organization](https://github.com/MacPaw/)
- [GitHub Actions Documentation](https://docs.github.com/en/actions)
- [Symfony PHP Package reusable workflow](docs/workflows/symfony-php-reusable.md)
- [Release workflow](docs/workflows/release.md)
- [Repository Analysis](ANALYSIS.md)
