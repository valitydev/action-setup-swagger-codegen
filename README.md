# `action-setup-swagger-codegen` - **Github Action**

This action installs [swagger-codegen](https://github.com/swagger-api/swagger-codegen) and [valitydev/swagger-generator-erlang](https://github.com/valitydev/swagger-generator-erlang).

## Input

| Name                         | Description                                 | Required | Default |
|------------------------------|---------------------------------------------|----------|---------|
| `codegen-version`            | swagger-codegen version to use              | ✓        |         |
| `generator-version`          | swagger-generator-erlang version to use     | ✓        |         |

## Example Workflow File

```yaml
name: Workflow with swagger-codegen

on: [ master ]

jobs:
  deploy:
    runs-on: ubuntu-latest
      steps:
        uses: valitydev/action-setup-swagger-codegen@v1.0.0
```
