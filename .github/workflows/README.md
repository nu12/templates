# Workflows

Table of contents:

* [.github/workflows/go-pr.v1.yml](#pull-request-go)
* [.github/workflows/go-release.v1.yml](#release-go)
* [.github/workflows/rails-pr.v1.yml](#pull-request-rails)
* [.github/workflows/rails-release.v1.yml](#release-rails)

## Pull Request (Go)

File: .github/workflows/go-pr.v1.yml



### Usage example

```
name: My workflow
on:
  push:
    branches:
    - main

jobs:
  my-job:
    uses: .github/workflows/go-pr.v1.yml@main
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

File: .github/workflows/go-release.v1.yml



### Usage example

```
name: My workflow
on:
  push:
    branches:
    - main

jobs:
  my-job:
    uses: .github/workflows/go-release.v1.yml@main
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

## Pull Request (Rails)

File: .github/workflows/rails-pr.v1.yml



### Usage example

```
name: My workflow
on:
  push:
    branches:
    - main

jobs:
  my-job:
    uses: .github/workflows/rails-pr.v1.yml@main
    with:
      docker-tag: 
      ruby-version: 
      run-docker-build: 
      run-lint: 
      run-scan: 
      run-test: 

```

### Inputs

|Name|Type|Description|Required|
|---|---|---|---|
|docker-tag|string|Docker tag|true|
|ruby-version|string|Ruby version|true|
|run-docker-build|boolean|Run docker build (without pushing the image)|true|
|run-lint|boolean|Run lint|true|
|run-scan|boolean|Run scan (brakeman)|true|
|run-test|boolean|Run test|true|

## Release (Rails)

File: .github/workflows/rails-release.v1.yml



### Usage example

```
name: My workflow
on:
  push:
    branches:
    - main

jobs:
  my-job:
    uses: .github/workflows/rails-release.v1.yml@main

```

