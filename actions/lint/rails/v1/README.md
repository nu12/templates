# Run linting (Rails)

Run rails linting

## Usage example

```
jobs:
  job-name:
    runs-on: <runner>
    steps:
    - uses: actions/lint/rails/v1@main
      with:
        ruby-version: 

```

## Inputs

|Name|Description|Required|Default value|
|---|---|---|---|
|ruby-version|Ruby version|true||

