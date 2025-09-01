[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/tyler36/ddev-openai-edge-tts/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/tyler36/ddev-openai-edge-tts/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/tyler36/ddev-openai-edge-tts)](https://github.com/tyler36/ddev-openai-edge-tts/commits)
[![release](https://img.shields.io/github/v/release/tyler36/ddev-openai-edge-tts)](https://github.com/tyler36/ddev-openai-edge-tts/releases/latest)

# DDEV Openai Edge Tts

## Overview

This add-on integrates Openai Edge Tts into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get tyler36/ddev-openai-edge-tts
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Openai Edge Tts |
| `ddev logs -s openai-edge-tts` | Check Openai Edge Tts logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.openai-edge-tts --openai-edge-tts-docker-image="ddev/ddev-utilities:latest"
ddev add-on get tyler36/ddev-openai-edge-tts
ddev restart
```

Make sure to commit the `.ddev/.env.openai-edge-tts` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `OPENAI_EDGE_TTS_DOCKER_IMAGE` | `--openai-edge-tts-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@tyler36](https://github.com/tyler36)**
