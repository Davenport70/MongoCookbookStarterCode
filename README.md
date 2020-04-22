#Mongo cookbook

## What is Chef?

Chef is a configuration management tool that allows you to provision code and create a secure, tested environment. Chef uses cookbooks which include provisioned recipes that install required packages. This means that when you create an AMI it comes with a standardised, provisioned environment.

## How to use the cookbook?

The cookbook is simple to use. Some commands you will need to ensure your cookbook is working. These commands will run your tests both locally and in AWS.

## Commands

Running a unit test
```
chef exec rspec
```
Testing Locally
```
kitchen test
```
Testing in AWS
```
KITCHEN_YAML=kitchen_cloud.yml kitchen test
```

## Pre-requisites

- chef

## list of what is installed
- Mongodb

## Options and setting variables

Changes are made in the attribute file.
Changing the port

```
default['mongo']['port'] = <new_value_here>
```
