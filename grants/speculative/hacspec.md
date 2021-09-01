# Project Name

The name of the project is: hacspec

## Project overview

hacspec is a functional domain specific language embedded in Rust with a set of tools that is designed for specifying cryptographic mechanisms.

This grant application is supposed to fund stabilizing the language definition and typechecker as well as the standard library.

### General

> In 5 lines, what is your project about?

The goal of hacspec is convenient tooling to write executable specifications and reference implementations that can be easily replaced with optimized native Rust code in order to bridge the gap between Rust cryptography and existing formal verification tools.

hacspec is a functional domain specific language embedded in Rust with a set of tools.

As a language for specifying cryptographic primitives and protocols it aims in particular at the Achilles heel of formal verification: the specifications.

In order to check that code is in hacspec and connect it to existing verification tools a typecheker is provided. The typechecker allows to develop and plug in language backends to compile hacspec code to formal languages such as F*, Coq, etc.

> Why Concordium shall support your project?

hacspec will make it significantly easier to verify correctness and security properties of cryptographic mechanisms, especially in Rust. The hacspec project has been collaborating with Bas Spitters from the COBRA project for a while now. Their team started to develop a Coq backend for the typehecker.

> How will your project integrate with Concordium?

Bas Spitters and his students implemented [BLS12-381 in hacspec](https://github.com/hacspec/hacspec/tree/master/examples/bls12-381) already and started contributing a [Coq backend](https://github.com/hacspec/hacspec/pull/123) to the typechecker. Their team is committed to building and extending the Coq/fiat-crypto backends for hacspec such that hacspec can be used at Concordium to verify correctness and security properties.

> Why you/your team are interested to build and develop this project?

We believe that the hacspec language and tooling can contribute significantly to the safety of cryptographic systems. As a low barrier entry point with multiple backends it can play a vital role in making formal methods a commonly used tool in the toolbox of (cryptography) engineers, just like testing or fuzzing.

### Description

> We work based on a "reverse-engineering" approach. We kindly ask you to:

> Define the final product, we like teams who dream a little bit here

We envision that hacspec will be part of a fully-fledged verification system for cryptographic mechanisms in Rust that enables ubiquitous use of formal methods throughout the design and development process of any such mechanism.

hacspec should be *the* entry point for everyone writing specifications for cryptographic mechanisms, or verifying security or code properties of implementations of such mechanisms.

> Describe in a reverse mode, what are the steps you aim to follow to reach your goal

The first step is to stabilize all parts of the hacspec project. In parallel more and more consumers and backends are added, and more specifications are written to demonstrate the capabilities of hacspec.

> Describe the current problems/issues you are encoutering

The core of the project consists of two distinct main parts. We have proof of concept implementations of both. This grant is supposed to help stabilize them.

**Language:** The hacspec language and typechecker.

**Standard Library:** The hacspec standard library that can be used in hacspecs.

The typechecker and existing backends have been written by individual PhD students so far and need to be cleaned up in order to make them maintainable and extensible. Because the typechecker is written in Rust as well in order to keep the entry barrier as low as possible the code is more complex and verbose than in other languages such as OCaml. Using the typechecker also takes noticeable time on non-trivial specifications. Improving performance is another challenge for the typechecker.

Defining the scope and APIs of the standard library is challenging. It must be expressive enough to make it easy for spec authors to write their specifications. At the same time it should be as small as possible to make it easier for new backends to plug in to hacspec. (Each backend needs to implement the standard library in the respective language.)

> Define how Concordium could help you

hacspec has been developed without any sort of funding so far. The funding will be necessary to stabilize the project and actually make it usable for others.

Concordium and COBRA can further be a significant user of hacspec and help guide the direction of the language as well as drive adoption. With Concordium being well embedded in the Rust, formal methods, as well as cryptography community. This network can help hacspec to build its community.

### Submission

- Website: [https://hacspec.org/](https://hacspec.org/)
- Github repository with PoC: [https://github.com/hacspec/hacspec/](https://github.com/hacspec/hacspec/)
- Project high-level presentation: [https://github.com/hacspec/hacspec/blob/master/presentation_slides.pdf](https://github.com/hacspec/hacspec/blob/master/presentation_slides.pdf)
- Technical report with specification and architecture: [https://hal.inria.fr/hal-03176482](https://hal.inria.fr/hal-03176482)

### Benchmark

> Please name the projects you are competing with:

**Cryptol**

The [Cryptol language](https://cryptol.net/) by [Galois](https://galois.com/) is a language to specify cryptography and can be used together with the [Software Analysis Workbench](https://saw.galois.com/) (SAW) to perform formal verification. There exists a Rust integration for SAW with [crux-mir](https://github.com/GaloisInc/crucible/tree/master/crux-mir). The cryptol language however is heavily influenced by haskell and therefore poses a pretty high entry bar — something hacspec explicitly wants to avoid.

**Other Rust Tools**

There are a number of tools in the Rust ecosystem that serve as frontends to verification toolchains such as [KLEE](https://klee.github.io/), [Prusti](https://github.com/viperproject/prusti-dev/), [Electrolysis](https://github.com/Kha/electrolysis), [SMACK](https://smackers.github.io/), [RustHorn](https://github.com/hopv/rust-horn) or [Creusot](https://github.com/xldenis/creusot). However, they are not focused on cryptographic mechanisms and have different focus areas, such as verifying full Rust programs. Further, most of these tools are very academic or not properly maintained.

### Team

- Franziskus Kiefer

    [https://www.franziskuskiefer.de/](https://www.franziskuskiefer.de/)

    [https://github.com/franziskuskiefer](https://github.com/franziskuskiefer)

    - Background

        Franziskus is a security and cryptography engineer and researcher based in Berlin. In his most recent role he was leading the security engineering efforts at [Wire](https://wire.com/), an end-to-end encrypted messaging and collaboration application.

        Previously, Franziskus was working on [Mozilla’s](https://mozilla.org/) cryptography library [NSS](https://en.wikipedia.org/wiki/Network_Security_Services) and [Firefox](https://firefox.com/) after finishing his PhD on password based cryptography at the University of Surrey. He is interested in everything around applied cryptography, in particular authentication and key exchange protocols, [formally verifiable specifications](http://hacspec.org/) and implementations of cryptographic primitives, and privacy preserving data collection and computation. He is also the initiator and co-organiser of the [Berlin Crypto Meetup](https://berlin-crypto.github.io/).

        A full list of my publications is available from the [publications page](https://www.franziskuskiefer.de/publications/).

- Karthik Bhargavan

    [https://prosecco.gforge.inria.fr/personal/karthik/](https://prosecco.gforge.inria.fr/personal/karthik/)

    [https://github.com/karthikbhargavan](https://github.com/karthikbhargavan)

    - Background

        Karthik is a researcher (directeur de recherche) at [Inria](http://www.inria.fr/), where he leads the [Prosecco project](http://prosecco.inria.fr/) ("Programming Securely with Cryptography") at [INRIA Paris](http://inria.fr/rocquencourt). He is a fellow (chaire) at the [Prairie](https://prairie-institute.fr/) research institute. He also teaches part-time at the [Master Parisien de Recherche en Informatique (MPRI)](https://wikimpri.dptinfo.ens-cachan.fr/doku.php).

        His research concerns the design and implementation of new program verification techniques that would enable formal analyses of real-world security applications. His recent work focuses on using dependent type systems, such as [F*](http://fstar-lang.org/). to investigate the (in)security of cryptographic protocols, such as [TLS](https://mitls.org/), and to build verified cryptographic libraries, such as [HACL*](https://github.com/project-everest/hacl-star). A full list of my publications is available from the [publications page](https://prosecco.gforge.inria.fr/personal/karthik/pubs.php).

        Karthik has recently been involved in the design, analysis, and standardization of [TLS 1.3](https://tools.ietf.org/html/rfc8446) and [Messaging Layer Security](https://datatracker.ietf.org/wg/mls/about/) at the IETF.

- We might get someone else on board to work on this under guidance of Franziskus and Karthik.

### Website

[https://hacspec.org/](https://hacspec.org/)

### Legal

> If relevant, what's the structure you're going to use in order to develop and commercialise your project? Please provide as much as possible details.

There is no plan to commercialize the project itself. hacspec is a community project that will be governed and maintained by an R&D company (in the process of being incorporated right now) run by Karthik Bhargavan and Franziskus Kiefer. It is and will continue to be developed under a permissive open source license (MIT right now). At the company hacspec will be used to analyse cryptographic mechanisms in commercial projects.

## Development

> This is the most important part of the application. This section shall explain in detail, the milestones of your project. These milestones will appear in the grant agreement.

### Overview

- Total Estimated Duration: 26 weeks (6 months)
- Full-Time Equivalent (FTE): 1
- Total Costs: $100k

The source code is developed under MIT license.

1. Standard Library Documentation (ED: 2 weeks, FTE: 1)

    Write documentation for the standard library functions.
    The documentation in rustdoc will make usage of the standard library easier as well as serve as a web presence of the library with example usages.

2. Test Standard Library (ED: 5 weeks, FTE: 1)
    
    Ensure all standard library functions are properly tested.
    Test coverage of the existing code is pretty low such that spec authors run into a lot of issues. Before publishing a first stable version of the library it is mandatory to ensure correctness of all provided functions.

3. Standard Library Stabilization (ED: 6 weeks, FTE: 1)

    Clean up and finalize v1.0 of the hacspec standard library.
    The library right now has a lot of unused code as well as unnecessary functionality. At the same time experimenting with specification has shown that some things like iterating over arrays isn't well supported right now. This milestone will clean up the existing code and extend the functionality where necessary, resulting in a first usable and stable version of the library.

4. Typechecker Documentation (ED: 2 weeks, FTE: 1)

    Document the typechecker implementation and the APIs for compiler backends.
    The documentation in rustdoc will ensure that it is easy to add new backends and allows maintenance and extension of the typechecker itself.

5. Test Typechecker (ED: 5 weeks, FTE: 1)

    Ensure that the typechecker is correct and all language features are being tested.
    The typechecker is crucial to ensure that specifications are valid hacspec code. Extensive testing is necessary to ensure that it works as expected.

6. Typechecker Stabilization (ED: 6 weeks, FTE: 1)

    Finalize v1.0 of the hacspec typechecker.
    It is important for the backend API to be stable such that (3rd party) language compilers don't break when improving the typechecker. In this milestone these APIs will be stabilized and the typechecker code will be refactored for maintainability and performance.

### Community and marketing

> As a part of the program, we kindly are asking you to produce content that explains your project. It could be videos, blog posts or press hits. This is a mandatory requirement to get a grant.

The project will inform academic papers that will be accompanied by blog posts.

There will be extensive documentation on how to use the different parts of the project as well as blog posts explaining progress and the project.

The website of the project will be extended with documentation and blog posts to explain and showcase all parts of the project.

### What's next?

> Please add here what ever makes sense for your future activities.

hacspec is a tool that we want to use to verify modern cryptography such as multi party computation, post-quantum cryptography, or zero-knowledge systems. We hope that hacspec can play a role in making formal methods more prevalent when implementing and specifying cryptographic mechanisms when the community around the language builds up over time and more cryptographers, engineers and formal methods folks use it.

The project will further be the starting point for a verification system in Rust that puts formal methods closer to the engineers and cryptographers writing the code and specifications.

In order to fund this we will be looking for long-term commitements from hacspec users.
