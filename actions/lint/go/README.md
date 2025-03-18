# Run linting (Go)

Run go linting

## Usage example

```
jobs:
  job-name:
    runs-on: <runner>
    steps:
    - uses: actions/lint/go@main
      with:
        go-version: 
        lint-version: v1.64

```

## Inputs

|Name|Description|Required|Default value|
|---|---|---|---|
|go-version|Go version|true||
|lint-version|Lint version|false|v1.64|

