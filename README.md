# PG Test Suite

This repository contains a test suite for implementations of [Property Graph Exchange Format (PG)](https://pg-format.github.io/):

## PG Format parsing

File `pg-format-valid.json` contains an array of test cases with keys:

- `pg` - the [PG Format](https://pg-format.github.io/specification/#pg-format) source to be parsed
- `about` (optional) - an informal description of the test case
- `graph` (optional) - the expected graph in [PG-JSON](https://pg-format.github.io/specification/#pg-json)
- `formatted` (optional) - pretty printed result of the source

File `pg-format-invalid.json` contains an object mapping invalid PG Format documents to informal descriptions of the test case.

## Examples

Directory `examples` contains sample documents in PG Format (`*.pg`) and PG-JSON (`*.json`). Applications are expected to parse each `NAME.pg` into the graph given in file `NAME.json`.
