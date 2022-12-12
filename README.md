# Files difference calculator


### Hexlet tests and linter status:
[![hexlet-check](https://github.com/Vasily7277/frontend-project-46/actions/workflows/hexlet-check.yml/badge.svg)](https://github.com/Vasily7277/frontend-project-46/actions/workflows/hexlet-check.yml)
[![linter & jest](https://github.com/Vasily7277/frontend-project-46/actions/workflows/linter&jest.yml/badge.svg)](https://github.com/Vasily7277/frontend-project-46/actions/workflows/linter&jest.yml)
[![Maintainability](https://api.codeclimate.com/v1/badges/7cb2e37150d0257c9bba/maintainability)](https://codeclimate.com/github/Vasily7277/frontend-project-46/maintainability)
[![Test Coverage](https://api.codeclimate.com/v1/badges/7cb2e37150d0257c9bba/test_coverage)](https://codeclimate.com/github/Vasily7277/frontend-project-46/test_coverage)


## Description
Difference Calculator is a program that determines the difference between two data structures. 

## Program features:
- Support for input formats: json, yaml, yml.
- Output reports in the form of stylish, plain or json.
"Difference checker" requires [Node.js](https://nodejs.org/) v18+ to run.

Copy repository and install the dependencies.

```sh
git clone https://github.com/Vasily7277/frontend-project-46
cd frontend-project-46/
make install
```

For help, you can use the --help (-h) command:

```sh
gendiff --help
```

### Compare flat .json files with *plain* structure (example of the 3rd step):

[![asciicast](https://asciinema.org/a/YXB8zMwvaPsTQUUFl8kCy6hJn.svg)](https://asciinema.org/a/YXB8zMwvaPsTQUUFl8kCy6hJn)

```sh
gendiff __fixtures__/file1.json __fixtures__/file2.json
```

### Compare flat .yaml files with *plain* structure (example of the 5th step):

[![asciicast](https://asciinema.org/a/qhR8ItKkATxbgSFhcEwZBBb89.svg)](https://asciinema.org/a/qhR8ItKkATxbgSFhcEwZBBb89)

```sh
gendiff __fixtures__/file1.yml __fixtures__/file2.yml 
```

### Compare .json files with *nested* structure and with default STYLYSH format (example of the 6th step):

[![asciicast](https://asciinema.org/a/BjectNRs9zHdNmzXgM3GZxWaD.svg)](https://asciinema.org/a/BjectNRs9zHdNmzXgM3GZxWaD)

```sh
gendiff __fixtures__/file1.json __fixtures__/file2.json 
```

### Compare files with *nested* structure and with PLAIN format (example of the 7th step):

[![asciicast](https://asciinema.org/a/LXUREwp5B2eKs7zTXIskn3i1V.svg)](https://asciinema.org/a/LXUREwp5B2eKs7zTXIskn3i1V)

```sh
gendiff -f plain __fixtures__/file1.json __fixtures__/file2.json
gendiff -f plain __fixtures__/file1.yml __fixtures__/file2.yml
```

### Compare files with *nested* structure and with JSON format (example of the 8th step):

[![asciicast](https://asciinema.org/a/sfCf5hOKnfMdQAOUz8LjV7FoV.svg)](https://asciinema.org/a/sfCf5hOKnfMdQAOUz8LjV7FoV)

```sh
gendiff -f json __fixtures__/file1.yml __fixtures__/file2.yml
gendiff -f json __fixtures__/file1.json __fixtures__/file2.json  
```