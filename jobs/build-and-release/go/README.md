# Build (Docker)

Build docker image

## Usage example

```
jobs:
  job-name:
    runs-on: <runner>
    steps:
    - uses: jobs/build-and-release/go@main
      with:
        go-main: main.go
        go-version: 
        name-extention: 
        name: 
        platform: linux-amd64
        release-name: 
        zip-util: zip

```

## Inputs

|Name|Description|Required|Default value|
|---|---|---|---|
|go-main|Files to build package main|false|main.go|
|go-version|Go version|true||
|name|Name of the repo, project, or application|true||
|name-extention|Extention of the binary (ex: .exe)|false||
|platform|Platform name|false|linux-amd64|
|release-name|Release name|true||
|zip-util|Zip utility command|false|zip|

