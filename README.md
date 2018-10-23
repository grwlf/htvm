HTVM
====

*Under construction*

This project is an experimental Haskell binding fot [TVM](https://tvm.ai)
Machine Learning framework. The project is under development at the moment.

Expected features are:

* DSL part produce C++ sources of the Machine Learing model by the means of
  Monadic interface.
* Compile part provides funtions to compile DSL source into dynamic library
* Runtime performs evaluation of the model using Haskell-to-C FFI.


In future, the C++ may should be replaced with explicit AST generation.

Install
-------

We use development environment specified in [Nix](https://nixos.org/nix)
language. Nix package manager and tools are expected to be installed on the
system. To enter the environment, type:

    $ nix-shell

in the project's main folder. Nix should open development shell with proper
Haskell packages installed. From this shell, one can run Cabal, Ghc and other
Haskell tools as usual:

    (nix-shell) $ cabal configure
    (nix-shell) $ cabal build
    (nix-shell) $ cabal repl htvm

Log
===

#### 22.10.2018
* Started to implement Printer

#### 17.10.2018
* Demo exposes DSL which compiles somehow

#### 15.10.2018
* Write this README.md
