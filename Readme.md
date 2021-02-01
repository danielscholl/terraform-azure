# terraform-azure

![Docker Build and Push](https://github.com/danielscholl/terraform-azure/workflows/Docker%20Build%20and%20Push/badge.svg)

A controlled Alpine docker image with terraform and azure cli.

Build
------

The make script will build the docker image. Arguments can be passed to the script that define the Terraform and Azure CLI Versions.

- Argument 1:  TERRAFORM_VERSION
- Argument 2:  AZURE_VERSION

Default Versions

- TERRAFORM_VERSION=0.14.5
- AZURE_VERSION=2.16.0

__COMMAND__
```
$ make \
    STEP_1_IMAGE="golang:1.15.6-alpine3.12" \
    STEP_2_IMAGE="alpine:3.12" \
    TERRAFORM_VERSION=0.14.5 \
    AZURE_CLI_VERSION=2.16.0 \
    docker-build
```

---
Project modeled after work done by [@bryannice](https://github.com/bryannice)
