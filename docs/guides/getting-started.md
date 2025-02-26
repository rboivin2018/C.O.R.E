---
layout: page
title: Getting Started
permalink: /guides/getting-started
---

# Getting Started Guide

This guide will help you set up and start using the Robotics Platform.

## Prerequisites

- Python 3.8+
- Git
- C++ development environment (for certain modules)

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/robotics-platform.git
cd robotics-platform

# Set up a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

## Basic Configuration

The platform uses YAML configuration files located in the `config` directory:

```bash
# Create your robot configuration
cp config/examples/drone.yaml config/my_drone.yaml
```

Edit `my_drone.yaml` to match your hardware specifications.

## Running Your First Robot

```bash
# Start the core system
python -m robotics.core --config=config/my_drone.yaml
```

## Next Steps

- [Configuring Sensors](configuring-sensors)
- [Creating Custom Controllers](custom-controllers)
- [Integrating New Hardware](hardware-integration)
