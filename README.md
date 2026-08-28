<p align="center">
  <a href="https://github.com/axolotl-pm/setup-php-action/actions"><img alt="setup-php-action status" src="https://github.com/axolotl-pm/setup-php-action/workflows/build-test/badge.svg"></a>
</p>

# setup-php-action

This action installs PHP and Composer for [Axolotl-PM](https://github.com/axolotl-pm/PocketMine-MP) from [axolotl-pm/PHP-Binaries releases](https://github.com/axolotl-pm/PHP-Binaries/releases).

This is used internally for Axolotl-PM's own CIs, and can also be used by plugins using GitHub Actions.

Currently only supported on Linux, but MacOS and Windows support is planned for the future.

## Inputs
| Name | Required | Possible values | Description |
|:-----|:--------:|:----------------|:------------|
| `php-version` | YES | Any version available in [`axolotl-pm/PHP-Binaries`](https://github.com/axolotl-pm/PHP-Binaries) (currently `8.1` through `8.5`) | PHP version, must be a full `major.minor.patch` |
| `install-path` | YES | Folder path | Path to install the binary into (e.g. `./bin`) |
| `pm-version-major` | NO | `5` | Major version of [Axolotl-PM](https://github.com/axolotl-pm/PocketMine-MP) to build extensions for |
