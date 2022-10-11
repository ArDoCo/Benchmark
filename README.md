[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6966831.svg)](https://doi.org/10.5281/zenodo.6966831)

# Benchmark
This repository contains a benchmark for traceability link recovery (TLR) between textual Software Architecture Documentation (SAD) and Software Architecture Models (SAM).

Each project of the benchmark is structured as follows:

* The README of each project contains some information about the used languages and lines of code created with [cloc](https://github.com/AlDanial/cloc).
* The folder `pcm` contains a Palladio Component Model (PCM) of the system. It has at least the repository view (components) of the system.
* The folder `uml` contains a Papyrus UML model. It is created from the PCM Repository using [PCM2UML](https://github.com/InFormALin/PCM2UML).
* The text file(s) in the project folder contains the SAD of the projects as plain text.
* The file `goldstandard.csv` contains the traceability links between SAD and SAM. It links the model elements by id with the sentences by their number (index starting at 1).

## Using the benchmark
In order to provide an easy approach to use the benchmark, we provide an example TLR approach called [Simple Tracelink Discovery (STD)](https://github.com/ArDoCo/SimpleTracelinkDiscovery/) that uses this benchmark in its [evaluation](https://github.com/ArDoCo/SimpleTracelinkDiscovery/tree/main/src/test/java/io/github/ardoco/simpletracelinkdiscovery/eval).
Therefore, the benchmark is linked to the STD repository via a [git subtree](https://github.com/ArDoCo/SimpleTracelinkDiscovery/tree/main/src/test/resources/benchmark).

## References
> **Note**
>
> Our LICENSE does only apply to the PCM models and the Gold Standards (CSV files). The texts are licensed w.r.t. to the actual projects.

### BigBlueButton
BigBlueButton (BBB) is a non-scientific application that provides a web conferencing system with the focus on creating a "global teaching platform".
The [documentation of BBB](https://docs.bigbluebutton.org/2.4/architecture.html) is licensed under LGPL.
Therefore, the text we extracted from their documentation is licensed according to the [license of BBB](https://bigbluebutton.org/open-source-project/open-source-license/) under LGPL.

### MediaStore
MediaStore is a "model application built after the iTunes Store".
Its architecture was used for exemplary performance analyses on software architecture models.
The text we extracted from their documentation originates from the publication [Modeling and Simulating Software Architectures: The Palladio Approach](https://books.google.de/books?id=g6BSDQAAQBAJ).

### Teammates
TEAMMATES is an open-source "online tool for manageing peer evaluations and other feedback paths of your students".
The documentation of TEAMMATES is part of their [repository](https://github.com/TEAMMATES/teammates).
Therefore, the text we extracted from their documentation is licensed according to the [license of TEAMMATES](https://github.com/TEAMMATES/teammates/blob/master/LICENSE) under GPL-2.0.

### Teastore
Teastore is a scientific application that is used as a "micro-service reference test application".
The [documentation](https://web.archive.org/web/20201102180945/https://github.com/DescartesResearch/teastore/wiki/Services) of Teastore was part of their [repository](https://github.com/DescartesResearch/teastore).
Therefore, the text we extracted from their documentation is licensed according to the [license of Teastore](https://github.com/DescartesResearch/TeaStore/blob/master/README.md) under Apache-2.0.

### JabRef
JabRef is a tool to manage citations and references in your bibliographies. It has features to collect, organize, cite, and share research work.

The [documentation](https://github.com/JabRef/jabref/blob/main/docs/getting-into-the-code/high-level-documentation.md) of JabRef is part of their [repository](https://github.com/JabRef/jabref/).
Therefore, the text we extracted from their documentation is licensed according to the [license of JabRef](https://github.com/JabRef/jabref/blob/main/LICENSE.md), i.e., MIT.
