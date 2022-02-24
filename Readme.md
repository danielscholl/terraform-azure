# terraform-azure

![Docker Build and Push](https://github.com/danielscholl/terraform-azure/workflows/Docker%20Build%20and%20Push/badge.svg)

A controlled Alpine docker image with terraform and azure cli.

Build
------

The make script will build the docker image. Arguments can be passed to the script that define the Terraform and Azure CLI Versions.

- Argument 1:  TERRAFORM_VERSION
- Argument 2:  AZURE_VERSION

Default Versions

- TERRAFORM_VERSION=1.1.6
- AZURE_VERSION=2.31.0

__COMMAND__
```
$ make \
    STEP_1_IMAGE="golang:1.17.7-alpine3.15" \
    STEP_2_IMAGE="alpine:3.15" \
    TERRAFORM_VERSION=1.1.6 \
    AZURE_CLI_VERSION=2.31.0 \
    docker-build
```
