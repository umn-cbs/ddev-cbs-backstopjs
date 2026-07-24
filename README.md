[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/mwaltonen/ddev-cbs-backstopjs/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/mwaltonen/ddev-cbs-backstopjs/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/mwaltonen/ddev-cbs-backstopjs)](https://github.com/mwaltonen/ddev-cbs-backstopjs/commits)
[![release](https://img.shields.io/github/v/release/mwaltonen/ddev-cbs-backstopjs)](https://github.com/mwaltonen/ddev-cbs-backstopjs/releases/latest)

# DDEV Cbs Backstopjs

## Overview

This add-on integrates Cbs Backstopjs into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get mwaltonen/ddev-cbs-backstopjs
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Cbs Backstopjs |
| `ddev logs -s cbs-backstopjs` | Check Cbs Backstopjs logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.cbs-backstopjs --cbs-backstopjs-docker-image="ddev/ddev-utilities:latest"
ddev add-on get mwaltonen/ddev-cbs-backstopjs
ddev restart
```

Make sure to commit the `.ddev/.env.cbs-backstopjs` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `CBS_BACKSTOPJS_DOCKER_IMAGE` | `--cbs-backstopjs-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@mwaltonen](https://github.com/mwaltonen)**
