# Run tests (Rails)

Run rails tests

## Usage example

```
jobs:
  job-name:
    runs-on: <runner>
    steps:
    - uses: actions/test/rails/v1@main
      with:
        ruby-version: 

```

## Inputs

|Name|Description|Required|Default value|
|---|---|---|---|
|ruby-version|Ruby version|true||

