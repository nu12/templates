# Zip

Create zip file

## Usage example

```
jobs:
  job-name:
    runs-on: <runner>
    steps:
    - uses: actions/utils/zip/v1@main
      with:
        file-to-zip: 
        output-file: 
        util: zip

```

## Inputs

|Name|Description|Required|Default value|
|---|---|---|---|
|file-to-zip|Name of the release|true||
|output-file|Name of the file to upload|true||
|util|Command to use for zipping|false|zip|

