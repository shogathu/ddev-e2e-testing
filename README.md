# DDEV E2e Testing

## Overview

This add-on integrates E2e Testing into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get shogathu/e2e-testing
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for E2e Testing |
| `ddev logs -s e2e-testing` | Check E2e Testing logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.e2e-testing --e2e-testing-docker-image="ddev/ddev-utilities:latest"
ddev add-on get shogathu/e2e-testing
ddev restart
```

Make sure to commit the `.ddev/.env.e2e-testing` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `E2E_TESTING_DOCKER_IMAGE` | `--e2e-testing-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@shogathu](https://github.com/shogathu)**
