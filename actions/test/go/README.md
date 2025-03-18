# Run tests (Go)

Run go tests

## Usage example

```
jobs:
  job-name:
    runs-on: <runner>
    steps:
    - uses: actions/test/go@main
      with:
        go-version: 

```

## Inputs

|Name|Description|Required|Default value|
|---|---|---|---|
|go-version|Go version|true||

