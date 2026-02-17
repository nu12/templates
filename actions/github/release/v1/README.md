# Release (Github)

Github release

## Usage example

```
jobs:
  job-name:
    runs-on: <runner>
    steps:
    - uses: actions/github/release/v1@main
      with:
        version: 

```

## Inputs

|Name|Description|Required|Default value|
|---|---|---|---|
|version|Release version number|true||

