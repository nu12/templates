# Setup (Go)

Setup Go

## Usage example

```
jobs:
  job-name:
    runs-on: <runner>
    steps:
    - uses: actions/setup/go/v1@main
      with:
        go-version: 

```

## Inputs

|Name|Description|Required|Default value|
|---|---|---|---|
|go-version|Go version|true||

