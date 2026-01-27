# Run scan (brakeman)

Run security scan (brakeman)

## Usage example

```
jobs:
  job-name:
    runs-on: <runner>
    steps:
    - uses: actions/scan/rails/v1@main
      with:
        ruby-version: 

```

## Inputs

|Name|Description|Required|Default value|
|---|---|---|---|
|ruby-version|Ruby version|true||

