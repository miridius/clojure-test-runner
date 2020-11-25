# Clojure test runner

 The test runner takes three parameters:
  1. The slug of the exercise (e.g. `two-fer`).
  2. A path to an input directory (with a trailing slash) containing the submitted solution file(s) and any other exercise file(s).
  3. A path to an output directory (with a trailing slash).
  
- A file named `results.json` will be written to the output directory.
- The runner will exit with an exit code of 0 if it has run successfully, regardless of the status of the tests.

``` bash
$ ./bin/run.sh <SLUG> <INPUT> <OUTPUT>
```

To run this project's tests (i.e. test the test runner):

    $ clojure -A:test:runner

Build an uberjar:

    $ clojure -A:uberjar

Run that uberjar:

    $ java -jar clojure-test-runner.jar

## Documentation

The specification of the interface that the test runners must conform to is found in the [track-tooling](https://github.com/exercism/v3-docs/tree/master/anatomy/track-tooling) repo.

## Copyright

All content in this repository is copyright to Exercism and licenced under AGPL
