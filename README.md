# Chef Circle CI Orb

This repository contains Chef-related orb maintained for our own needs.

Support is very limited, currently orb is applicable for ubuntu only.

## Commands

### setup-cdk

Installs Chef Development Kit.

The only parameter is `version`, which is optional.

### setup

Currently just a `setup-cdk` alias, with `cdk_version` parameter instead
of `version`.

### share

Shares cookbook on Supermarket. Expects knife to be installed, i.e.
setup command should be called separately before share. 

Parameters:

| name                     | description               | default                     |
|:-------------------------|:--------------------------|:----------------------------|
| cookbook                 | Cookbook name             |                             |
| supermarket_user         |                           |                             |
| location                 | Cookbook parent directory | ..                          |
| category                 | Cookbook category         | Other                       |
| supermarket_url          |                           | https://supermarket.chef.io |
| supermarket_key_variable | Environment variable that holds base64-encoded supermarket key | SUPERMARKET_KEY | 
