## Go

These settings apply only when `--go` is specified on the command line.

```yaml $(go)
go:
  license-header: MICROSOFT_APACHE_NO_VERSION
  clear-output-folder: true
```

### Tag: package-2020-02-20 and go

These settings apply only when `--tag=package-2020-02-20 --go` is specified on the command line.
Please also specify `--go-sdks-folder=<path to the root directory of your azure-sdk-for-go clone>`.

```yaml $(tag) == 'package-2020-02-20' && $(go)
namespace: Microsoft.Hubtest
output-folder: $(go-sdks-folder)/testonly/Generated
```
