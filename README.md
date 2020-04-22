#Node cookbook

description
This cookbook installed mongodb from source.
It creates its own apt package and then installs it.
The recipe also creates the config files and then service file with dynamic input of variables.

## list of what is installed
- Mongodb

## Options and setting variables

Changes are made in the attribute file.
Changing the port

## Commands

```
chef exec rspec
```
```
kitchen test
```
```
KITCHEN_YAML=kitchen_cloud.yml kitchen test
```
