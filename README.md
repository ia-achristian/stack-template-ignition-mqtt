# Project Template

This project template is designed as a base repository for any Ignition MQTT project. It includes a basic structure for a project to be customized and built upon. For starters, this readme should be updated with pertinent information for the project.

The stack consists of four services:

- `distributor`: An Ignition Gateway with the CirrusLink MQTT Distributor module
- `engine`: An Ignition Gateway with the CirrusLink MQTT Engine module, and a connection to the Distributor
- `transmission`: An Ignition Gateway with the CirrusLink MQTT Transmission module, and a connection to the Distributor
- `transmission-edge`: An Ignition Edge Gateway with the CirrusLink MQTT Transmission module, and a connection to the Distributor

With the exception of the `distributor` service, which acts as the MQTT broker for the stack, any of the other three services can be removed without affecting other components of the stack.

The password for the default MQTT user `admin` in this stack is `password` (different from the MQTT modules' default).

> [!WARNING]
> Do not use default passwords in production!

## Creating a README

- The contents of this readme should be updated with information about the project.
- See [Make a README](https://www.makeareadme.com/) for tips on creating a good README, and specifically [what to include](https://www.makeareadme.com/#suggestions-for-a-good-readme).

## Quick links

- [Setup Guide](https://github.com/inductive-automation/docs-common/blob/main/docs/setup-guide.md): Instructions for setting up the project for the first time.
- [Quickstart Guide](https://github.com/inductive-automation/docs-common/blob/main/docs/quickstart-guide.md): Instructions for making changes to the project after initial setup.
- Sub-directory READMEs: Additional information for how to use specific directories in the project can be found in the READMEs of those directories.

## Linting Checks

This project has some linting checks that are run automatically on pull requests. You can see more information about these checks in the [docs-common repository](https://github.com/inductive-automation/common-workflows).
