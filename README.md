# Evan Sultanik, Ph.D.
[![Twitter Link](https://img.shields.io/twitter/follow/ESultanik?style=social)](https://twitter.com/ESultanik)
[![website](https://img.shields.io/badge/website-sultanik.com-lightgray)](https://www.sultanik.com/)
<span style="float:right">[![CC BY NC SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]</span>











<img style="float:right" src="https://github-readme-stats.vercel.app/api?username=ESultanik&count_private=true&show_icons=true&theme=chartreuse-dark&include_all_commits=true">

Evan is a principal computer security researcher based in Philadelphia working at [Trail of Bits](https://github.com/trailofbits/).
He has a couple dozen academic publications, but most of them are related to distributed systems and combinatorial optimization,
not security.
He is also an editor of and frequent contributor to the offensive computer security journal [Proof of Concept or GTFO](https://www.sultanik.com/pocorgtfo).

[Evan’s woefully out-of-date résumé](https://www.sultanik.com/files/ESultanikResume.pdf) is a PDF that is also a ZIP
as well as an Nintendo Entertainment System ROM! That’s right: [Evan’s résumé PDF](https://www.sultanik.com/files/ESultanikResume.pdf)
is a valid NES ROM that you can emulate! Check the footnotes on the first page. If you don't have an NES emulator handy,
you can actually [emuluate the PDF in your browser](https://www.sultanik.com/nesresume/).
Evan also has an [even more woefully out-of-date academic _curriculum vitæ_.](https://www.sultanik.com/files/ESultanikCV.pdf)

Aside from when writing in a biographical format, Evan does not usually refer to himself in the third person.

The following are some of my selected projects.

## Program Analysis 🔎

Automated program instrumentation and bug-finding. This section is for general program analysis tools. Tools related to
to Blockchain technology and smart contracts are in their own section, below.

### PolyTracker

<span style="float:right">![co%E2%80%91creator](https://img.shields.io/badge/-co%E2%80%91creator-brightgreen?cacheSeconds=604800) </span> <span style="float:right">![maintainer](https://img.shields.io/badge/-maintainer-brightgreen?cacheSeconds=604800) </span>
[![GitHub](https://img.shields.io/badge/repo--brightgreen?style=social&logo=github)](https://github.com/trailofbits/polytracker)
![GitHub Stars](https://img.shields.io/github/stars/trailofbits/polytracker?style=social)
[![PyPI Downloads](https://img.shields.io/pypi/dm/polytracker?label=PyPI%20Downloads)](/project/polytracker/)
[![License](https://img.shields.io/github/license/trailofbits/polytracker)](https://github.com/trailofbits/polytracker/blob/master/LICENSE)

An LLVM-based universal taint and data-flow analysis instrumentation framework. Can track up to 2<sup>32</sup> input 
bytes.

### Manticore

<span style="float:right">![contributor](https://img.shields.io/badge/-contributor-brightgreen?cacheSeconds=604800) </span>
[![GitHub](https://img.shields.io/badge/repo--brightgreen?style=social&logo=github)](https://github.com/trailofbits/manticore)
![GitHub Stars](https://img.shields.io/github/stars/trailofbits/manticore?style=social)
[![PyPI Downloads](https://img.shields.io/pypi/dm/manticore?label=PyPI%20Downloads)](/project/manticore/)
[![License](https://img.shields.io/github/license/trailofbits/manticore)](https://github.com/trailofbits/manticore/blob/master/LICENSE)

Symbolic execution engine for x86, ARM, and EVM.

### Fickling

<span style="float:right">![creator](https://img.shields.io/badge/-creator-brightgreen?cacheSeconds=604800) </span> <span style="float:right">![maintainer](https://img.shields.io/badge/-maintainer-brightgreen?cacheSeconds=604800) </span>
[![GitHub](https://img.shields.io/badge/repo--brightgreen?style=social&logo=github)](https://github.com/trailofbits/fickling)
![GitHub Stars](https://img.shields.io/github/stars/trailofbits/fickling?style=social)
[![PyPI Downloads](https://img.shields.io/pypi/dm/fickling?label=PyPI%20Downloads)](/project/fickling/)
[![License](https://img.shields.io/github/license/trailofbits/fickling)](https://github.com/trailofbits/fickling/blob/master/LICENSE)

Fickling is a decompiler, static analyzer, and bytecode rewriter for Python
[pickle](https://docs.python.org/3/library/pickle.html) object serializations.

Pickled Python objects are in fact bytecode that is interpreted by a stack-based virtual machine
built into Python called the "Pickle Machine". Fickling can take pickled data streams and decompile them into
human-readable Python code that, when executed, will deserialize to the original serialized object.

I do not prescribe any meaning to the “F” in Fickling; it could stand for “fickle,” … or something else.
Divining its meaning is a personal journey in discretion and is left as an exercise to the reader.

Learn more about it in our [blog post](https://blog.trailofbits.com/2021/03/15/never-a-dill-moment-exploiting-machine-learning-pickle-files/)
and [DEF CON 2021 talk](https://www.youtube.com/watch?v=bZ0m_H_dEJI).

## Funky Files 📄

A lot of my recent work has been on developing examples of funky files that exploit buggy file formats and parsers (see
the footnotes on the first page of [my résumé](https://www.sultanik.com/files/ESultanikResume.pdf), for example), as 
well as tools to make file formats and parsers safer.

### PolyFile

<span style="float:right">![creator](https://img.shields.io/badge/-creator-brightgreen?cacheSeconds=604800) </span> <span style="float:right">![maintainer](https://img.shields.io/badge/-maintainer-brightgreen?cacheSeconds=604800) </span>
[![GitHub](https://img.shields.io/badge/repo--brightgreen?style=social&logo=github)](https://github.com/trailofbits/polyfile)
![GitHub Stars](https://img.shields.io/github/stars/trailofbits/polyfile?style=social)
[![PyPI Downloads](https://img.shields.io/pypi/dm/polyfile?label=PyPI%20Downloads)](/project/polyfile/)
[![License](https://img.shields.io/github/license/trailofbits/polyfile)](https://github.com/trailofbits/polyfile/blob/master/LICENSE)

A cleanroom, pure-Python implementation of libmagic that can identify files, is smart about polyglots (files that are
multiple types at the same time), can output an interactive HTML-based hex viewer, and recursively enumerate the
contents of a file (similar to `binwalk`).

### A PDF Git Repository Polyglot

<span style="float:right">![creator](https://img.shields.io/badge/-creator-brightgreen?cacheSeconds=604800) </span>

I created a [PDF that is a git repository](https://github.com/ESultanik/PDFGitPolyglot) that, when cloned, contains its LaTeX 
source code and a copy of itself. The PDF contains an article describing how I did it.

## Utilities 🛠

I enjoy building generic command line utilities and libraries.

### Graphtage

<span style="float:right">![creator](https://img.shields.io/badge/-creator-brightgreen?cacheSeconds=604800) </span> <span style="float:right">![maintainer](https://img.shields.io/badge/-maintainer-brightgreen?cacheSeconds=604800) </span>
[![GitHub](https://img.shields.io/badge/repo--brightgreen?style=social&logo=github)](https://github.com/trailofbits/graphtage)
![GitHub Stars](https://img.shields.io/github/stars/trailofbits/graphtage?style=social)
[![PyPI Downloads](https://img.shields.io/pypi/dm/graphtage?label=PyPI%20Downloads)](/project/graphtage/)
[![License](https://img.shields.io/github/license/trailofbits/graphtage)](https://github.com/trailofbits/graphtage/blob/master/LICENSE)

Graphtage is a command-line utility and underlying library for semantically comparing and merging tree-like structures,
such as JSON, XML, HTML, YAML, plist, and CSS files. Its name is a portmanteau of “graph” and “graftage”—the latter
being the horticultural practice of joining two trees together such that they grow as one.

### It-Depends

<span style="float:right">![co%E2%80%91creator](https://img.shields.io/badge/-co%E2%80%91creator-brightgreen?cacheSeconds=604800) </span> <span style="float:right">![maintainer](https://img.shields.io/badge/-maintainer-brightgreen?cacheSeconds=604800) </span>
[![GitHub](https://img.shields.io/badge/repo--brightgreen?style=social&logo=github)](https://github.com/trailofbits/it-depends)
![GitHub Stars](https://img.shields.io/github/stars/trailofbits/it-depends?style=social)
[![PyPI Downloads](https://img.shields.io/pypi/dm/it-depends?label=PyPI%20Downloads)](/project/it-depends/)
[![License](https://img.shields.io/github/license/trailofbits/it-depends)](https://github.com/trailofbits/it-depends/blob/master/LICENSE)

It-Depends is a tool to automatically build a dependency graph and Software Bill of Materials (SBOM) for packages and 
arbitrary source code repositories. You can use it to enumerate all third party dependencies for a software package, map 
those dependencies to known security vulnerabilities, as well as compare the similarity between two packages based on 
their dependencies.

### Notify When Done (nwd)

<span style="float:right">![creator](https://img.shields.io/badge/-creator-brightgreen?cacheSeconds=604800) </span> <span style="float:right">![maintainer](https://img.shields.io/badge/-maintainer-brightgreen?cacheSeconds=604800) </span>
[![GitHub](https://img.shields.io/badge/repo--brightgreen?style=social&logo=github)](https://github.com/esultanik/nwd)
![GitHub Stars](https://img.shields.io/github/stars/esultanik/nwd?style=social)
[![PyPI Downloads](https://img.shields.io/pypi/dm/nwd?label=PyPI%20Downloads)](/project/nwd/)
[![License](https://img.shields.io/github/license/esultanik/nwd)](https://github.com/esultanik/nwd/blob/master/LICENSE)

Notify When Done (`nwd`) is a utility for triggering alerts when a process finishes. Kicking off a long-running compile? 
NWD can post a popup notification when it's done. Starting a job on a remote server? `nwd` can send you an E-mail when 
it’s done. Want to run a custom script once another finishes? `nwd` can facilitate that, too.

### Biggest

<span style="float:right">![creator](https://img.shields.io/badge/-creator-brightgreen?cacheSeconds=604800) </span> <span style="float:right">![maintainer](https://img.shields.io/badge/-maintainer-brightgreen?cacheSeconds=604800) </span>
[![GitHub](https://img.shields.io/badge/repo--brightgreen?style=social&logo=github)](https://github.com/esultanik/nwd)
![GitHub Stars](https://img.shields.io/github/stars/esultanik/nwd?style=social)
[![PyPI Downloads](https://img.shields.io/pypi/dm/nwd?label=PyPI%20Downloads)](/project/nwd/)
[![License](https://img.shields.io/github/license/esultanik/nwd)](https://github.com/esultanik/nwd/blob/master/LICENSE)

A utility for finding the largest directories and/or files in a given directory hierarchy. Biggest supports pretty 
printed and colorized output to the terminal.

## Cryptography 🔐

Despite dabbling in cryptography, I am not a cryptographer. Do not use this code to secure your secrets. 

### Lenticrypt

<span style="float:right">![creator](https://img.shields.io/badge/-creator-brightgreen?cacheSeconds=604800) </span> <span style="float:right">![maintainer](https://img.shields.io/badge/-maintainer-brightgreen?cacheSeconds=604800) </span>
[![GitHub](https://img.shields.io/badge/repo--brightgreen?style=social&logo=github)](https://github.com/esultanik/lenticrypt)
![GitHub Stars](https://img.shields.io/github/stars/esultanik/lenticrypt?style=social)
[![PyPI Downloads](https://img.shields.io/pypi/dm/lenticrypt?label=PyPI%20Downloads)](/project/lenticrypt/)
[![License](https://img.shields.io/github/license/esultanik/lenticrypt)](https://github.com/esultanik/lenticrypt/blob/master/LICENSE)

A proof-of-concept cryptosystem that provides provable plausibly deniable encryption.
Lenticrypt can generate a single ciphertext file such that _different_ plaintexts are generated depending on which key 
is used for decryption.

## Blockchain ⛓

“Crypto” 👏 Means 👏 Cryp 👏 to 👏 gra 👏 phy!

I no longer own any cryptocurrency. I know too much about how the sausage is made.

The most ethical way I can contribute to that ecosystem is to build tools that at least make it safer for those who are 
willing to transact with it. The following are those tools.

### Etheno

<span style="float:right">![creator](https://img.shields.io/badge/-creator-brightgreen?cacheSeconds=604800) </span> <span style="float:right">![maintainer](https://img.shields.io/badge/-maintainer-brightgreen?cacheSeconds=604800) </span>
[![GitHub](https://img.shields.io/badge/repo--brightgreen?style=social&logo=github)](https://github.com/crytic/etheno)
![GitHub Stars](https://img.shields.io/github/stars/crytic/etheno?style=social)
[![PyPI Downloads](https://img.shields.io/pypi/dm/etheno?label=PyPI%20Downloads)](/project/etheno/)
[![License](https://img.shields.io/github/license/crytic/etheno)](https://github.com/crytic/etheno/blob/master/LICENSE)

Etheno is the Ethereum testing Swiss Army knife. It’s a JSON RPC multiplexer, analysis tool wrapper, and test 
integration tool. It eliminates the complexity of setting up analysis tools like Manticore and Echidna on large, 
multi-contract projects. In particular, custom Manticore analysis scripts require less code, are simpler to write, and 
integrate with Truffle.

### solc-select

<span style="float:right">![creator](https://img.shields.io/badge/-creator-brightgreen?cacheSeconds=604800) </span>
[![GitHub](https://img.shields.io/badge/repo--brightgreen?style=social&logo=github)](https://github.com/crytic/solc-select)
![GitHub Stars](https://img.shields.io/github/stars/crytic/solc-select?style=social)
[![PyPI Downloads](https://img.shields.io/pypi/dm/solc-select?label=PyPI%20Downloads)](/project/solc-select/)
[![License](https://img.shields.io/github/license/crytic/solc-select)](https://github.com/crytic/solc-select/blob/master/LICENSE)

I am the creator of the original version of solc-select: A tool to quickly switch between Solidity compiler versions.

### Slither

<span style="float:right">![contributor](https://img.shields.io/badge/-contributor-brightgreen?cacheSeconds=604800) </span>
[![GitHub](https://img.shields.io/badge/repo--brightgreen?style=social&logo=github)](https://github.com/crytic/slither)
![GitHub Stars](https://img.shields.io/github/stars/crytic/slither?style=social)
[![PyPI Downloads](https://img.shields.io/pypi/dm/slither?label=PyPI%20Downloads)](/project/slither-analyzer/)
[![License](https://img.shields.io/github/license/crytic/slither)](https://github.com/crytic/slither/blob/master/LICENSE)

I am a contributor to Slither, a Solidity static analysis framework. It runs a suite of vulnerability detectors, prints 
visual information about contract details, and provides an API to easily write custom analyses. Slither enables 
developers to find vulnerabilities, enhance their code comprehension, and quickly prototype custom analyses.

### Ethereum Security Toolbox

<span style="float:right">![creator](https://img.shields.io/badge/-creator-brightgreen?cacheSeconds=604800) </span> <span style="float:right">![maintainer](https://img.shields.io/badge/-maintainer-brightgreen?cacheSeconds=604800) </span>
[![GitHub](https://img.shields.io/badge/repo--brightgreen?style=social&logo=github)](https://github.com/crytic/eth-security-toolbox)
![GitHub Stars](https://img.shields.io/github/stars/crytic/eth-security-toolbox?style=social)
[![License](https://img.shields.io/github/license/crytic/eth-security-toolbox)](https://github.com/crytic/eth-security-toolbox/blob/master/LICENSE)
[![Docker Pulls](https://img.shields.io/docker/pulls/trailofbits/eth-security-toolbox)](https://hub.docker.com/r/trailofbits/eth-security-toolbox)


### Echidna

<span style="float:right">![contributor](https://img.shields.io/badge/-contributor-brightgreen?cacheSeconds=604800) </span>
[![GitHub](https://img.shields.io/badge/repo--brightgreen?style=social&logo=github)](https://github.com/crytic/echidna)
![GitHub Stars](https://img.shields.io/github/stars/crytic/echidna?style=social)
[![License](https://img.shields.io/github/license/crytic/echidna)](https://github.com/crytic/echidna/blob/master/LICENSE)

I am a contributor to Echidna, a fuzzer/property-based tester of Ethereum smarts contracts. It uses sophisticated 
grammar-based fuzzing campaigns based on a contract ABI to falsify user-defined predicates or Solidity assertions.

[cc-by-nc-sa]: https://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY%20NC%20SA%204.0-lightgrey.svg
