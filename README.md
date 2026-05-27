# Formalizing Independence and Causality in Reversible Concurrent Calculi

## Overview

This repository contains a formalization of reversible concurrent calculi in [Beluga](https://complogic.cs.mcgill.ca/beluga/index.html).

It extends and refines the [formalization of CCSKP in Beluga](https://github.com/CinRC/A-Beluga-Formalization-of-CCSKP) presented in [*A Formalization of the Reversible Concurrent Calculus CCSKP in Beluga*](https://cgi.cse.unsw.edu.au/~eptcs/paper.cgi?ICE2025.5) with additional results from [*Independence and Causality in the Reversible Concurrent Setting.*](https://doi.org/10.1007/978-3-031-97063-4_2).

[![Code Type Reconstruction](https://github.com/CinRC/Formalizing-Independence-and-Causality-in-Reversible-Concurrent-Calculi/actions/workflows/main.yml/badge.svg)](https://github.com/CinRC/Formalizing-Independence-and-Causality-in-Reversible-Concurrent-Calculi/actions/workflows/main.yml)
[![Example Tests](https://github.com/CinRC/Formalizing-Independence-and-Causality-in-Reversible-Concurrent-Calculi/actions/workflows/test.yml/badge.svg)](https://github.com/CinRC/Formalizing-Independence-and-Causality-in-Reversible-Concurrent-Calculi/actions/workflows/test.yml)

## Usage instructions

Once Beluga is installed (cf. [the installation instructions](#installation-instructions)), it suffices to run

```console
beluga run/code.cfg 
```

to perform the type reconstruction of the formalization. Expected result, after ±15 seconds, is

```console
## Type Reconstruction begin: run/../code/shared/definitions.bel ##
## Type Reconstruction done:  run/../code/shared/definitions.bel ##
## Type Reconstruction begin: run/../code/shared/unique.bel ##
## Type Reconstruction done:  run/../code/shared/unique.bel ##
## Type Reconstruction begin: run/../code/shared/basic-properties.bel ##
## Type Reconstruction done:  run/../code/shared/basic-properties.bel ##
## Type Reconstruction begin: run/../code/ccsk/definitions.bel ##
## Type Reconstruction done:  run/../code/ccsk/definitions.bel ##
## Type Reconstruction begin: run/../code/ccsk/unique-step.bel ##
## Type Reconstruction done:  run/../code/ccsk/unique-step.bel ##
## Type Reconstruction begin: run/../code/ccskp/definitions.bel ##
## Type Reconstruction done:  run/../code/ccskp/definitions.bel ##
## Type Reconstruction begin: run/../code/ccskp/unique.bel ##
## Type Reconstruction done:  run/../code/ccskp/unique.bel ##
## Type Reconstruction begin: run/../code/ccskp/basic-properties.bel ##
## Type Reconstruction done:  run/../code/ccskp/basic-properties.bel ##
## Type Reconstruction begin: run/../code/ccskp/lemmas-connectivity-one.bel ##
## Type Reconstruction done:  run/../code/ccskp/lemmas-connectivity-one.bel ##
## Type Reconstruction begin: run/../code/ccskp/connectivity-relationship-one.bel ##
## Type Reconstruction done:  run/../code/ccskp/connectivity-relationship-one.bel ##
## Type Reconstruction begin: run/../code/ccskp/lemmas-connectivity-two.bel ##
## Type Reconstruction done:  run/../code/ccskp/lemmas-connectivity-two.bel ##
## Type Reconstruction begin: run/../code/ccskp/connectivity-relationship-two.bel ##
## Type Reconstruction done:  run/../code/ccskp/connectivity-relationship-two.bel ##
## Type Reconstruction begin: run/../code/ccskp/complementarity.bel ##
## Type Reconstruction done:  run/../code/ccskp/complementarity.bel ##
## Type Reconstruction begin: run/../code/ccskp/unique-step.bel ##
## Type Reconstruction done:  run/../code/ccskp/unique-step.bel ##
## Type Reconstruction begin: run/../code/ccskp/lemmas-bijection.bel ##
## Type Reconstruction done:  run/../code/ccskp/lemmas-bijection.bel ##
## Type Reconstruction begin: run/../code/bijection/definitions.bel ##
## Type Reconstruction done:  run/../code/bijection/definitions.bel ##
## Type Reconstruction begin: run/../code/bijection/functionality.bel ##
## Type Reconstruction done:  run/../code/bijection/functionality.bel ##
## Type Reconstruction begin: run/../code/bijection/totality.bel ##
## Type Reconstruction done:  run/../code/bijection/totality.bel ##
## Type Reconstruction begin: run/../code/bijection/bijection.bel ##
## Type Reconstruction done:  run/../code/bijection/bijection.bel ##
## Type Reconstruction begin: run/../code/ccskp/axioms/transitions-properties.bel ##
## Type Reconstruction done:  run/../code/ccskp/axioms/transitions-properties.bel ##
## Type Reconstruction begin: run/../code/ccskp/axioms/bti.bel ##
## Type Reconstruction done:  run/../code/ccskp/axioms/bti.bel ##
## Type Reconstruction begin: run/../code/ccskp/axioms/sp.bel ##
## Type Reconstruction done:  run/../code/ccskp/axioms/sp.bel ##
## Type Reconstruction begin: run/../code/ccskp/axioms/wf.bel ##
## Type Reconstruction done:  run/../code/ccskp/axioms/wf.bel ##
## Type Reconstruction begin: run/../code/ccskp/axioms/pci.bel ##
## Type Reconstruction done:  run/../code/ccskp/axioms/pci.bel ##
## Type Reconstruction begin: run/../code/ccskp/axioms/fld.bel ##
## Type Reconstruction done:  run/../code/ccskp/axioms/fld.bel ##
## Type Reconstruction begin: run/../code/ccskp/axioms/ire.bel ##
## Type Reconstruction done:  run/../code/ccskp/axioms/ire.bel ##
## Type Reconstruction begin: run/../code/ccskp/axioms/cire.bel ##
## Type Reconstruction done:  run/../code/ccskp/axioms/cire.bel ##
## Type Reconstruction begin: run/../code/ccskp/axioms/rpi.bel ##
## Type Reconstruction done:  run/../code/ccskp/axioms/rpi.bel ##
## Type Reconstruction begin: run/../code/ccskp/axioms/ed.bel ##
## Type Reconstruction done:  run/../code/ccskp/axioms/ed.bel ##
## Type Reconstruction begin: run/../code/ccsk/axioms/transitions-properties.bel ##
## Type Reconstruction done:  run/../code/ccsk/axioms/transitions-properties.bel ##
```

Tests can be run using e.g.

```console
beluga run/ex-processes.cfg 
```

For this particular set of examples, expected result is, after ±1 second,

```console
## Type Reconstruction begin: run/../code/shared/definitions.bel ##
## Type Reconstruction done:  run/../code/shared/definitions.bel ##
## Type Reconstruction begin: run/../examples/processes/standard.bel ##
## Type Reconstruction done:  run/../examples/processes/standard.bel ##
## Type Reconstruction begin: run/../examples/processes/stuck-std.bel ##
## Type Reconstruction done:  run/../examples/processes/stuck-std.bel ##
## Type Reconstruction begin: run/../examples/processes/keyed.bel ##
## Type Reconstruction done:  run/../examples/processes/keyed.bel ##
## Type Reconstruction begin: run/../examples/processes/stuck-keyed.bel ##
## Type Reconstruction done:  run/../examples/processes/stuck-keyed.bel ##
```

If Makefile is installed, then the previous commands can be replaced by

```console
make code
```

and 

```console
make test
```

will perform the type reconstruction of all the tests, and is expected to take ±8 seconds.

## Installation instructions

This mechanization is compatible with [Beluga](https://complogic.cs.mcgill.ca/beluga/) version 1.1.1 and above, and optionally uses [GNU Make](https://www.gnu.org/software/make/) version 4.0 and above to facilitate compilation.
To install Beluga or compile it from source, please refer to [their documentation](https://beluga-lang.readthedocs.io/en/latest/getting-started.html#installation) or [installation guide](https://github.com/Beluga-lang/Beluga/blob/master/INSTALL).

In short, once [opam](https://opam.ocaml.org/doc/Install.html) version 2.1.4 and above is installed, simply execute

```shell
opam install beluga
```

Optionally, for improved beli mode [rlwrap](https://github.com/hanslub42/rlwrap) can also be installed.

## Repository structure

- `run\`: Contains the `.cfg` files requires to compile …
  + `code.cfg`: … the actual formalization (in `code/` folder)
  + `ex-processes.cfg`: … test examples on processes (in `examples` folder)
  + `ex-proof-labels.cfg`: … test examples on proof labels (in `examples` folder)
  + `ex-transitions.cfg`: … test examples on transitions (in `examples` folder)
  + `ex-causality-relations.cfg`: … test examples on connectivity, dependence and independence (in `examples` folder)
- `code\`: Contains the Beluga formalization of …
  + `shared\`: … shared …
    * `definitions.bel`: … definitions
    * `unique.bel`: … proofs of uniqueness of the derivation of predicates
    * `basic-properties.bel`: … properties of keys
  + `ccsk\`: … CCSK …
    * `definitions.bel`: … definitions
    * `unique-step.bel`: … uniqueness of the derivation of transitions
    * `axioms\`: … axioms, in particular …
      - `transitions-properties.bel`: … definitions and auxiliary lemmas for the axioms
  + `ccskp\`: … CCSKP …
    * `definitions.bel`: … definitions
    * `unique.bel`: … uniqueness of the derivation of predicates
    * `basic-properties.bel`: … basic properties (e.g. loop lemma, symmetry of transitions and paths)
    * `lemmas-connectivity-one.bel`: … auxiliary lemmas for Proposition 4.4 (1)
    * `connectivity-relationship-one.bel`: … Proposition 4.4 (1)
    * `lemmas-connectivity-two.bel`: … auxiliary lemmas for Proposition 4.4 (2)
    * `connectivity-relationship-two.bel`: … Proposition 4.4 (2)
    * `complementarity.bel`: … complementarity of dependence and independence
    * `unique-step.bel`: … uniqueness of the derivation of transitions
    * `lemmas-bijection.bel`: … auxiliary lemmas for the CCSK-CCSKP bijection
    * `axioms\`: … axioms, in particular …
      - `transitions-properties.bel`: … definitions and auxiliary lemmas for the axioms
      - `bti.bel`: … BTI (backward transitions are independent)
      - `sp.bel`: … SP (square property)
      - `wf.bel`: … WF (well-foundedness)
      - `pci.bel`: … PCI (propagation of coinitial independence)
      - `fld.bel`: … FLD (forward label determinism) and BLD (backward label determinism)
      - `ire.bel`: … IRE (independence respects events)
      - `cire.bel`: … CIRE (coinitial independence respects events)
      - `rpi.bel`: … RPI (reversing preserves independence)
      - `ed.bel`: … ED (event determinism)
  + `bijection\`: … the proof of the bijection between CCSK and CCSKP, in particular …
    * `definitions.bel`: … definitions of the forget and enrich functions (as relations)
    * `functionality.bel`: … functionality of forget and enrich
    * `totality.bel`: … totality of forget and enrich
    * `bijection.bel`: … forget and enrich are mutual inverses

- `examples\`: Contains examples serving as tests for…
  + `processes\`: … processes that …
    * `standard.bel`: … are standard
    * `keyed.bel`: … contain keys
    * `stuck-std.bel`: … are standard and stuck
    * `stuck-keyed.bel`: … contain keys and are stuck
  + `proof-labels\`: … proof labels that …
    * `valid.bel`: … are valid
    * `not-valid.bel`: … are not valid
  + `transitions\`: … transitions, in particular …
    * `forward-transitions-ccsk.bel`: … forward transitions in CCSK
    * `backward-transitions-ccsk.bel`: … backward transitions in CCSK
    * `stuck-std-ccsk.bel`: … proofs that some standard processes are stuck in CCSK
    * `stuck-keyed-ccsk.bel`: … proofs that some processes containing keys are stuck in CCSK
    * `forward-transitions-ccskp.bel`: … forward transitions in CCSKP
    * `backward-transitions-ccskp.bel`: … backward transitions in CCSKP
    * `stuck-std-ccskp.bel`: … proofs that some standard processes are stuck in CCSKP
    * `stuck-keyed-ccskp.bel`: … proofs that some processes containing keys are stuck in CCSKP
    * `events.bel`: … transitions representing the same event
  + `causality-relations\`: … causality relations on proof labels, in particular …
    * `connectivity.bel`: … connected proof labels
    * `dependence.bel`: … dependent proof labels
    * `independence.bel`: … independent proof labels

The `.github\workflows\` repository contains workflows used to build automatically the code and run the tests.
The `beluga_cloc_config.txt` file is a configuration file for [cloc](https://github.com/AlDanial/cloc) to count lines of code.
