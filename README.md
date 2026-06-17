# Formalising Independence and Causality in Reversible Concurrent Calculi

## Overview

This repository contains a formalisation of reversible concurrent calculi in [Beluga](https://complogic.cs.mcgill.ca/beluga/index.html).

It extends and refines the [formalisation of CCSK<sup>P</sup>](https://github.com/CinRC/A-Beluga-Formalization-of-CCSKP) presented in [*A Formalization of the Reversible Concurrent Calculus CCSK<sup>P</sup> in Beluga*](https://doi.org/10.4204/EPTCS.425.5) with additional results from [*Independence and Causality in the Reversible Concurrent Setting*](https://doi.org/10.1007/978-3-031-97063-4_2).

[![Code Type Reconstruction](https://github.com/CinRC/Formalising-Independence-and-Causality-in-Reversible-Concurrent-Calculi/actions/workflows/main.yml/badge.svg)](https://github.com/CinRC/Formalising-Independence-and-Causality-in-Reversible-Concurrent-Calculi/actions/workflows/main.yml)
[![Example Tests](https://github.com/CinRC/Formalising-Independence-and-Causality-in-Reversible-Concurrent-Calculi/actions/workflows/test.yml/badge.svg)](https://github.com/CinRC/Formalising-Independence-and-Causality-in-Reversible-Concurrent-Calculi/actions/workflows/test.yml)

## Usage instructions

Once Beluga is installed (cf. [the installation instructions](#installation-instructions)), it suffices to run

```console
beluga run/code.cfg 
```

to type-check and verify the formalisation. The expected output, after ±15 seconds, is the following:

<details>
<summary>View expected output</summary>

```console
## Type Reconstruction begin: run/../code/shared/definitions.bel ##
## Type Reconstruction done:  run/../code/shared/definitions.bel ##
## Type Reconstruction begin: run/../code/shared/unique.bel ##
## Type Reconstruction done:  run/../code/shared/unique.bel ##
## Type Reconstruction begin: run/../code/shared/basic-properties.bel ##
## Type Reconstruction done:  run/../code/shared/basic-properties.bel ##
## Type Reconstruction begin: run/../code/ccsk/definitions.bel ##
## Type Reconstruction done:  run/../code/ccsk/definitions.bel ##
## Type Reconstruction begin: run/../code/ccsk/basic-properties.bel ##
## Type Reconstruction done:  run/../code/ccsk/basic-properties.bel ##
## Type Reconstruction begin: run/../code/ccsk/unique-step.bel ##
## Type Reconstruction done:  run/../code/ccsk/unique-step.bel ##
## Type Reconstruction begin: run/../code/ccskp/definitions.bel ##
## Type Reconstruction done:  run/../code/ccskp/definitions.bel ##
## Type Reconstruction begin: run/../code/ccskp/unique.bel ##
## Type Reconstruction done:  run/../code/ccskp/unique.bel ##
## Type Reconstruction begin: run/../code/ccskp/basic-properties.bel ##
## Type Reconstruction done:  run/../code/ccskp/basic-properties.bel ##
## Type Reconstruction begin: run/../code/ccskp/lemmas-connectedness-one.bel ##
## Type Reconstruction done:  run/../code/ccskp/lemmas-connectedness-one.bel ##
## Type Reconstruction begin: run/../code/ccskp/connectedness-relationship-one.bel ##
## Type Reconstruction done:  run/../code/ccskp/connectedness-relationship-one.bel ##
## Type Reconstruction begin: run/../code/ccskp/lemmas-connectedness-two.bel ##
## Type Reconstruction done:  run/../code/ccskp/lemmas-connectedness-two.bel ##
## Type Reconstruction begin: run/../code/ccskp/connectedness-relationship-two.bel ##
## Type Reconstruction done:  run/../code/ccskp/connectedness-relationship-two.bel ##
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
## Type Reconstruction begin: run/../code/ccskp/axioms/defs-and-properties.bel ##
## Type Reconstruction done:  run/../code/ccskp/axioms/defs-and-properties.bel ##
## Type Reconstruction begin: run/../code/ccskp/axioms/events.bel ##
## Type Reconstruction done:  run/../code/ccskp/axioms/events.bel ##
## Type Reconstruction begin: run/../code/ccskp/axioms/bti.bel ##
## Type Reconstruction done:  run/../code/ccskp/axioms/bti.bel ##
## Type Reconstruction begin: run/../code/ccskp/axioms/sp.bel ##
## Type Reconstruction done:  run/../code/ccskp/axioms/sp.bel ##
## Type Reconstruction begin: run/../code/ccskp/axioms/wf.bel ##
## Type Reconstruction done:  run/../code/ccskp/axioms/wf.bel ##
## Type Reconstruction begin: run/../code/ccskp/axioms/pci.bel ##
## Type Reconstruction done:  run/../code/ccskp/axioms/pci.bel ##
## Type Reconstruction begin: run/../code/ccskp/axioms/id.bel ##
## Type Reconstruction done:  run/../code/ccskp/axioms/id.bel ##
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
## Type Reconstruction begin: run/../code/ccsk/complementarity.bel ##
## Type Reconstruction done:  run/../code/ccsk/complementarity.bel ##
## Type Reconstruction begin: run/../code/ccsk/axioms/defs-and-properties.bel ##
## Type Reconstruction done:  run/../code/ccsk/axioms/defs-and-properties.bel ##
## Type Reconstruction begin: run/../code/ccsk/axioms/events.bel ##
## Type Reconstruction done:  run/../code/ccsk/axioms/events.bel ##
## Type Reconstruction begin: run/../code/bijection/lemmas-lifting.bel ##
## Type Reconstruction done:  run/../code/bijection/lemmas-lifting.bel ##
## Type Reconstruction begin: run/../code/ccsk/axioms/bti.bel ##
## Type Reconstruction done:  run/../code/ccsk/axioms/bti.bel ##
## Type Reconstruction begin: run/../code/ccsk/axioms/sp.bel ##
## Type Reconstruction done:  run/../code/ccsk/axioms/sp.bel ##
## Type Reconstruction begin: run/../code/ccsk/axioms/wf.bel ##
## Type Reconstruction done:  run/../code/ccsk/axioms/wf.bel ##
## Type Reconstruction begin: run/../code/ccsk/axioms/pci.bel ##
## Type Reconstruction done:  run/../code/ccsk/axioms/pci.bel ##
## Type Reconstruction begin: run/../code/ccsk/axioms/id.bel ##
## Type Reconstruction done:  run/../code/ccsk/axioms/id.bel ##
## Type Reconstruction begin: run/../code/ccsk/axioms/ire.bel ##
## Type Reconstruction done:  run/../code/ccsk/axioms/ire.bel ##
## Type Reconstruction begin: run/../code/ccsk/axioms/cire.bel ##
## Type Reconstruction done:  run/../code/ccsk/axioms/cire.bel ##
## Type Reconstruction begin: run/../code/ccsk/axioms/rpi.bel ##
## Type Reconstruction done:  run/../code/ccsk/axioms/rpi.bel ##
## Type Reconstruction begin: run/../code/ccsk/axioms/ed.bel ##
## Type Reconstruction done:  run/../code/ccsk/axioms/ed.bel ##
```

</details>

Tests can be run using, e.g.,

```console
beluga run/ex-processes.cfg 
```

For this particular set of examples, the expected result is, after ±1 second,

<details>
<summary>View expected output</summary>

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

</details>

If Makefile is installed, then the previous commands can be replaced by

```console
make code
```

and 

```console
make test
```

The latter will perform the type reconstruction of all the tests, and is expected to take ±8 seconds.

The totality declarations following each recursive function declaration ensure that all functions are total and that every recursive call is made on a decreasing argument, guaranteeing the correctness of the proofs. The optional `--coverage` pragma can be added to the .bel files to check these conditions.

## Installation instructions

This mechanization is compatible with [Beluga](https://complogic.cs.mcgill.ca/beluga/) version 1.1.1 and above, and optionally uses [GNU Make](https://www.gnu.org/software/make/) version 4.0 and above to facilitate compilation.
To install Beluga or compile it from source, please refer to [their documentation](https://beluga-lang.readthedocs.io/en/latest/getting-started.html#installation) or [installation guide](https://github.com/Beluga-lang/Beluga/blob/master/INSTALL).

In short, once [opam](https://opam.ocaml.org/doc/Install.html) version 2.1.4 and above is installed, simply execute

```shell
opam install beluga.1.1.1
```

## Repository structure

- `run\`: Contains the `.cfg` files requires to compile …
  + `code.cfg`: … the actual formalisation (in `code/` folder)
  + `ex-processes.cfg`: … test examples on processes (in `examples/` folder)
  + `ex-proof-labels.cfg`: … test examples on proof labels (in `examples/` folder)
  + `ex-transitions.cfg`: … test examples on transitions (in `examples/` folder)
  + `ex-causality-relations.cfg`: … test examples on connectedness, dependence and independence (in `examples/` folder)
- `code\`: Contains the Beluga formalisation of …
  + `shared\`: … shared …
    * `definitions.bel`: … definitions
    * `unique.bel`: … proofs of uniqueness of the derivation of predicates
    * `basic-properties.bel`: … properties of keys
  + `ccsk\`: … CCSK …
    * `definitions.bel`: … definitions
    * `basic-properties.bel`: … basic properties (e.g. loop lemma, symmetry of transitions and paths)
    * `unique-step.bel`: … uniqueness of the derivation of transitions
    * `complementarity.bel`: … complementarity of dependence and independence
    * `axioms\`: … axioms, in particular …
      - `defs-and-properties.bel`: … definitions and auxiliary lemmas for the axioms
      - `events.bel`: … definition and properties of equivalent transitions
      - `bti.bel`: … BTI (backward transitions are independent)
      - `sp.bel`: … SP (square property)
      - `wf.bel`: … WF (well-foundedness)
      - `pci.bel`: … PCI (propagation of coinitial independence)
      - `id.bel`: … ID (independence of diamonds)
      - `ire.bel`: … IRE (independence respects events)
      - `cire.bel`: … CIRE (coinitial independence respects events)
      - `rpi.bel`: … RPI (reversing preserves independence)
      - `ed.bel`: … ED (event determinism)
  + `ccskp\`: … CCSKP …
    * `definitions.bel`: … definitions
    * `unique.bel`: … uniqueness of the derivation of predicates
    * `basic-properties.bel`: … basic properties (e.g. loop lemma, symmetry of transitions and paths)
    * `lemmas-connectedness-one.bel`: … auxiliary lemmas for Proposition 4.4 (1)
    * `connectedness-relationship-one.bel`: … Proposition 4.4 (1)
    * `lemmas-connectedness-two.bel`: … auxiliary lemmas for Proposition 4.4 (2)
    * `connectedness-relationship-two.bel`: … Proposition 4.4 (2)
    * `complementarity.bel`: … complementarity of dependence and independence
    * `unique-step.bel`: … uniqueness of the derivation of transitions
    * `lemmas-bijection.bel`: … auxiliary lemmas for the CCSK-CCSKP bijection
    * `axioms\`: … axioms, in particular …
      - `defs-and-properties.bel`: … definitions and auxiliary lemmas for the axioms
      - `events.bel`: … definition and properties of equivalent transitions
      - `bti.bel`: … BTI (backward transitions are independent)
      - `sp.bel`: … SP (square property)
      - `wf.bel`: … WF (well-foundedness)
      - `pci.bel`: … PCI (propagation of coinitial independence)
      - `id.bel`: … ID (independence of diamonds)
      - `fld.bel`: … FLD (forward label determinism)
      - `ire.bel`: … IRE (independence respects events)
      - `cire.bel`: … CIRE (coinitial independence respects events)
      - `rpi.bel`: … RPI (reversing preserves independence)
      - `ed.bel`: … ED (event determinism)
  + `bijection\`: … the proof of the bijection between CCSK and CCSKP, in particular …
    * `definitions.bel`: … definitions of the forget and enrich functions (as relations)
    * `functionality.bel`: … functionality of forget and enrich
    * `totality.bel`: … totality of forget and enrich
    * `bijection.bel`: … forget and enrich are mutual inverses
    * `lemmas-lifting.bel`: … properties that can be lifted from one LTS to the other
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
    * `connectedness.bel`: … connected proof labels
    * `dependence.bel`: … dependent proof labels
    * `independence.bel`: … independent proof labels

The `.github\workflows\` repository contains workflows used to build automatically the code and run the tests.
The `beluga_cloc_config.txt` file is a configuration file for [cloc](https://github.com/AlDanial/cloc) to count lines of code.

### Line count

Thanks to [cloc](https://github.com/AlDanial/cloc) and [our configuration file](beluga_cloc_config.txt), 

```console
cloc --md --read-lang-def=beluga_cloc_config.txt --by-file code/
cloc --read-lang-def=beluga_cloc_config.txt --by-file examples/
```

or 

```console
make count
```

can be used to count the lines of code (comments excluded):

<!--
Add the --md flag to the commands above to obtain a markdown-formatted table.
-->

<details>
<summary>View line count</summary>

File|blank|comment|code
:-------|-------:|-------:|-------:
code/ccsk/axioms/defs-and-properties.bel|34|48|1908
code/ccskp/axioms/sp.bel|42|73|977
code/ccskp/axioms/defs-and-properties.bel|61|86|719
code/ccskp/connectedness-relationship-one.bel|3|6|689
code/ccskp/connectedness-relationship-two.bel|14|31|567
code/ccskp/unique-step.bel|31|29|528
code/ccskp/lemmas-bijection.bel|33|44|417
code/ccskp/complementarity.bel|32|30|409
code/bijection/totality.bel|21|26|298
code/ccskp/axioms/bti.bel|18|36|296
code/ccskp/lemmas-connectedness-one.bel|24|27|293
code/ccskp/definitions.bel|54|71|274
code/ccsk/unique-step.bel|10|12|195
code/bijection/lemmas-lifting.bel|16|46|155
code/ccskp/axioms/fld.bel|6|15|147
code/ccskp/lemmas-connectedness-two.bel|12|21|141
code/bijection/bijection.bel|23|19|114
code/ccskp/basic-properties.bel|15|16|112
code/bijection/functionality.bel|16|27|100
code/ccskp/axioms/events.bel|16|32|93
code/ccskp/unique.bel|10|15|92
code/ccskp/axioms/wf.bel|10|17|79
code/shared/unique.bel|9|10|69
code/ccsk/definitions.bel|14|12|67
code/ccsk/axioms/bti.bel|5|10|58
code/ccskp/axioms/id.bel|3|11|54
code/shared/definitions.bel|13|14|54
code/ccsk/axioms/id.bel|3|11|53
code/ccsk/basic-properties.bel|5|5|45
code/bijection/definitions.bel|11|12|44
code/shared/basic-properties.bel|7|10|44
code/ccsk/complementarity.bel|8|15|43
code/ccsk/axioms/events.bel|4|18|25
code/ccsk/axioms/sp.bel|2|5|23
code/ccsk/axioms/pci.bel|1|14|19
code/ccsk/axioms/ed.bel|1|3|17
code/ccsk/axioms/wf.bel|3|4|17
code/ccsk/axioms/cire.bel|1|4|11
code/ccsk/axioms/ire.bel|1|4|9
code/ccsk/axioms/rpi.bel|1|3|9
code/ccskp/axioms/pci.bel|1|5|8
code/ccskp/axioms/ire.bel|1|4|7
code/ccskp/axioms/cire.bel|1|4|6
code/ccskp/axioms/rpi.bel|1|3|6
code/ccskp/axioms/ed.bel|1|3|5
--------|--------|--------|--------
SUM:|598|911|9296

File|blank|comment|code
:-------|-------:|-------:|-------:
examples/transitions/stuck-keyed-ccskp.bel|18|13|85
examples/transitions/stuck-keyed-ccsk.bel|14|8|56
examples/transitions/forward-transitions-ccskp.bel|16|18|48
examples/transitions/stuck-std-ccskp.bel|9|7|46
examples/transitions/forward-transitions-ccsk.bel|16|18|45
examples/proof-labels/not-valid.bel|8|7|28
examples/transitions/backward-transitions-ccskp.bel|9|11|26
examples/transitions/backward-transitions-ccsk.bel|9|11|24
examples/transitions/stuck-std-ccsk.bel|4|4|19
examples/transitions/events.bel|0|3|17
examples/processes/standard.bel|8|9|15
examples/causality-relations/independence.bel|6|5|14
examples/causality-relations/connectedness.bel|6|5|12
examples/causality-relations/dependence.bel|6|5|12
examples/proof-labels/valid.bel|13|12|12
examples/processes/keyed.bel|6|7|6
examples/processes/stuck-keyed.bel|5|6|6
examples/processes/stuck-std.bel|3|4|3
--------|--------|--------|--------
SUM:|156|153|474

</details>