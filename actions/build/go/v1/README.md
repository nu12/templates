# Build (Go)

Build Go project

## Usage example

```
jobs:
  job-name:
    runs-on: <runner>
    steps:
    - uses: actions/build/go/v1@main
      with:
        go-main: main.go
        go-version: 
        name-extention: 
        name: 

```

## Inputs

|Name|Description|Required|Default value|
|---|---|---|---|
|go-main|Main file of the project|false|main.go|
|go-version|Go version|true||
|name|Name of the binary (output)|true||
|name-extention|Extention of the binary (ex: .exe)|false||

