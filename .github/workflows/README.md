# Workflows

Table of contents:

* [.github/workflows/go-pr.yml](#Pull-Request-(Go))
* [.github/workflows/go-release.yml](#Release-(Go))

## Pull Request (Go)

File: .github/workflows/go-pr.yml



### Usage example

```
name: My workflow
on:
  push:
    branches:
    - main

jobs:
  my-job:
    uses: .github/workflows/go-pr.yml@main
    with: 
      docker-tag: 
      go-version: 
      run-docker-build: 
      run-lint: 
      run-test: 

```

### Inputs

|Name|Type|Description|Required|
|---|---|---|---|
|docker-tag|string|Docker tag|true|
|go-version|string|Go version|true|
|run-docker-build|boolean|Run docker build (without pushing the image)|true|
|run-lint|boolean|Run lint|true|
|run-test|boolean|Run test|true|

## Release (Go)

File: .github/workflows/go-release.yml



### Usage example

```
name: My workflow
on:
  push:
    branches:
    - main

jobs:
  my-job:
    uses: .github/workflows/go-release.yml@main
    with: 
      go-binary-name: 
      go-main: 
      go-version: 
      release-darwin-amd64: 
      release-darwin-arm64: 
      release-docker: 
      release-linux-amd64: 
      release-win-amd64: 
      version: 

```

### Inputs

|Name|Type|Description|Required|
|---|---|---|---|
|go-binary-name|string|Go binary name|true|
|go-main|string|Go main files|true|
|go-version|string|Go version|true|
|release-darwin-amd64|boolean|Release darwin-amd64|true|
|release-darwin-arm64|boolean|Release darwin-arm64|true|
|release-docker|boolean|Release docker|true|
|release-linux-amd64|boolean|Release linux-amd64|true|
|release-win-amd64|boolean|Release win-amd64|true|
|version|string|Version to release|true|

