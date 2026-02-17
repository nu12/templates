# Upload (Github)

Upload file to Github release

## Usage example

```
jobs:
  job-name:
    runs-on: <runner>
    steps:
    - uses: actions/github/upload/v1@main
      with:
        release-name: 
        upload-file: 

```

## Inputs

|Name|Description|Required|Default value|
|---|---|---|---|
|release-name|Name of the release|true||
|upload-file|Name of the file to upload|true||

