# pads-haskell
The pads haskell repository contains the code for the Haskell binding for PADS.  For more information about the project, see the
pads website (www.padsproj.org).

# Building

`pads-haskell` currently requires GHC 7.10.3. This project provides an
appropriate [Stack][1] configuration file.

## Setup

To install an appropriate GHC tool chain:

```bash
$ stack setup
```

## Build

To build `pads-haskell`:

```bash
$ stack build
```

# Testing

To run the automated testing infrastructure:

```bash
stack test pads-haskell:examples
```

Or to run individual tests:

```bash
stack repl
λ> :l Examples.First
...
λ> test
Cases: 89  Tried: 89  Errors: 0  Failures: 0
Counts {cases = 89, tried = 89, errors = 0, failures = 0}
(0.11 secs, 0 bytes)
```

[1]: https://www.stackage.org/
