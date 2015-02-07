# nvm box

[![wercker status](https://app.wercker.com/status/189c21e17f08866388d3601daaaee1f7/m "wercker status")](https://app.wercker.com/project/bykey/189c21e17f08866388d3601daaaee1f7)

Box that runs [nvm](https://github.com/creationix/nvm) to support the usage of multiple node versions.
It installs the latest versions of node __0.8__, __0.9__, __0.10__, __0.11__ and makes __0.10__ the default version when running node.

## Example

```yaml
box: seigyo/nvm
build:
  steps:
    - script:
        name: Set NVM to NodeJS 0.11.x (latest)
        code: |
          nvm use 0.11
    - npm-install
    - npm-test
```

## Changelog

### 0.2.0

- Updated installed version of NVM

### 0.1.0

- Initial release

## License

MIT, see LICENSE
