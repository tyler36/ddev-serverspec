[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/tyler36/ddev-serverspec/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/tyler36/ddev-serverspec/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/tyler36/ddev-serverspec)](https://github.com/tyler36/ddev-serverspec/commits)
[![release](https://img.shields.io/github/v/release/tyler36/ddev-serverspec)](https://github.com/tyler36/ddev-serverspec/releases/latest)

# DDEV Serverspec

## Overview

This add-on integrates [Serverspec](https://serverspec.org/) into your [DDEV](https://ddev.com/) project.

This add-on installs the required serverspec packages inside the web container.

## Installation

```bash
ddev add-on get tyler36/ddev-serverspec
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev serverspec-init` | Scaffold tests |
| `ddev serverspec` | Run serverspec tests |

## Credits

**Contributed and maintained by [@tyler36](https://github.com/tyler36)**
