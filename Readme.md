# alpine-terraform-azure

A minimal terraform and azure cli Docker image (~26mb) - [Alpine Linux](https://alpinelinux.org/).

Build
------

The make script will build the docker image. Arguments can be passed to the script that define the Terraform and Azure CLI Versions.

- Argument 1:  TERRAFORM_VERSION
- Argument 2:  AZURE_VERSION

Default Versions

- TERRAFORM_VERSION=0.14.5
- AZURE_VERSION=

__COMMAND__
```
$  make \
    STEP_1_IMAGE="golang:1.14.1-alpine3.11" \
    STEP_2_IMAGE="alpine:3.11" \
    TERRAFORM_VERSION=0.12.20 \
    docker-build
```

Run Example
-------

```
  $
```
