# Build (Docker)

Build docker image

## Usage example

```
jobs:
  job-name:
    runs-on: <runner>
    steps:
    - uses: actions/build/docker/v1@main
      with:
        context: .
        dockerfile: Dockerfile
        name: ${{ github.repository }}
        platforms: linux/amd64,linux/arm64
        push: true
        registry-password: 
        registry-username: ${{ github.actor }}
        registry: ghcr.io
        tag: 

```

## Inputs

|Name|Description|Required|Default value|
|---|---|---|---|
|context|Build context|false|.|
|dockerfile|Dockerfile path|false|Dockerfile|
|name|Name of the image|false|${{ github.repository }}|
|platforms|Platform to build for|false|linux/amd64,linux/arm64|
|push|Push the image|false|true|
|registry|Docker registry|false|ghcr.io|
|registry-password|Docker registry password|false||
|registry-username|Docker registry username|false|${{ github.actor }}|
|tag|Docker tag|true||

