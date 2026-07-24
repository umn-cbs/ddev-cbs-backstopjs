# DDEV CBS Backstopjs

## Overview

This add-on integrates CBS Backstopjs into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get umn-cbs/ddev-cbs-backstopjs
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for CBS Backstopjs |
| `ddev logs -s cbs-backstopjs` | Check CBS Backstopjs logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.cbs-backstopjs --cbs-backstopjs-docker-image="ddev/ddev-utilities:latest"
ddev add-on get umn-cbs/ddev-cbs-backstopjs
ddev restart
```

Make sure to commit the `.ddev/.env.cbs-backstopjs` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `CBS_BACKSTOPJS_DOCKER_IMAGE` | `--cbs-backstopjs-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@umn-cbs](https://github.com/umn-cbs)**
