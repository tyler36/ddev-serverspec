[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/tyler36/ddev-serverspec/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/tyler36/ddev-serverspec/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/tyler36/ddev-serverspec)](https://github.com/tyler36/ddev-serverspec/commits)
[![release](https://img.shields.io/github/v/release/tyler36/ddev-serverspec)](https://github.com/tyler36/ddev-serverspec/releases/latest)

# DDEV Serverspec

## Overview

This add-on integrates Serverspec into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get tyler36/ddev-serverspec
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Serverspec |
| `ddev logs -s serverspec` | Check Serverspec logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.serverspec --serverspec-docker-image="ddev/ddev-utilities:latest"
ddev add-on get tyler36/ddev-serverspec
ddev restart
```

Make sure to commit the `.ddev/.env.serverspec` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `SERVERSPEC_DOCKER_IMAGE` | `--serverspec-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@tyler36](https://github.com/tyler36)**
