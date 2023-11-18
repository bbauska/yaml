# yaml
Digital guide to the YAML framework.
In 2005, the web developer Dirk Jesse published the responsive CSS framework YAML under the Creative Commons license CC-BY 2.0, which allowed the basic framework to be used for free both privately and commercially. Operators who want to put their web project online under a different license can also acquire a commercial model that gives them free access to the licensing. The focus of the CSS framework has always been on offering users the biggest possible freedom for the design of barrier-free web applications. The current version of the framework (4.2.1) was made available in 2013, and is supported by various content management systems such as WordPress, TYPO3, or Joomla thanks to corresponding CMS integration templates.


Course Content


Collapse All Sections

1
YAML overview

2 Lessons

Course overview
Introduction to YAML
2
Syntax of YAML

4 Lessons

Overview of syntax in YAML
Overview of data types in YAML
Overview of advanced data types in YAML
Comparison of various data formats
3
Applications of YAML

2 Lessons

Overview of various tools using YAML
Overview of parsers and emitters for YAML



<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
%YAML 1.2
---
YAML: YAML Ain't Markup Language™

What It Is:
  YAML is a human-friendly data serialization
  language for all programming languages.

YAML Resources:
  YAML Specifications:
  - YAML 1.2:
    - Revision 1.2.2      # Oct 1, 2021 *New*
    - Revision 1.2.1      # Oct 1, 2009
    - Revision 1.2.0      # Jul 21, 2009
  - YAML 1.1
  - YAML 1.0

  YAML Matrix Chat:  '#chat:yaml.io'     # Our New Group Chat Room!
  YAML IRC Channel:  libera.chat#yaml    # The old chat
  YAML News:         twitter.com/yamlnews
  YAML Mailing List: yaml-core           # Obsolete, but historical

  YAML on GitHub:                        # github.com/yaml/
    YAML Specs:        yaml-spec/
    YAML 1.2 Grammar:  yaml-grammar/
    YAML Test Suite:   yaml-test-suite/
    YAML Issues:       issues/

  YAML Reference Parsers:
  - Generated Reference Parsers
  - YPaste Interactive Parser

  YAML Test Matrix:   matrix.yaml.io

YAML Frameworks and Tools:
  C/C++:
  - libfyaml      # "C" YAML 1.2 processor (YTS)
  - libyaml       # "C" Fast YAML 1.1 (YTS)
  - libcyaml      # YAML de/serialization of C data (using libyaml)
  - yaml-cpp      # C++ YAML 1.2 implementation

  Crystal:
  - YAML          # YAML 1.1 from the standard library

  C#/.NET:
  - YamlDotNet    # YAML 1.1/(1.2) library + serialization (YTS)
  - yaml-net      # YAML 1.1 library

  D:
  - D-YAML        # YAML 1.1 library w/ official community support (YTS)

  Dart:
  - yaml          # YAML package for Dart

  Delphi:
  - Neslib.Yaml   # YAML 1.1 Delphi binding to libyaml (YTS)

  Elixir:
  - yaml-elixir   # YAML support for the Elixir language

  Erlang:
  - yamerl        # YAML support for the Erlang language

  Golang:
  - Go-yaml       # YAML support for the Go language
  - Go-gypsy      # Simplified YAML parser written in Go
  - goccy/go-yaml # YAML 1.2 implementation in pure Go

  Haskell:
  - HsYAML         # YAML 1.2 implementation in pure Haskell (YTS)
  - YamlReference  # Haskell 1.2 reference parser
  - yaml           # YAML 1.1 Haskell framework (based on libyaml)

  Java:
  - SnakeYAML Engine  # Java 8+ / YAML 1.2
  - SnakeYAML         # Java 5 / YAML 1.1
  - YamlBeans         # To/from JavaBeans. YAML 1.0/1.1
  - eo-yaml           # YAML 1.2 for Java 8. Packaged as a Module (Java 9+)
  - Chronicle-Wire    # Java Implementation

  JavaScript:
  - yaml          # JavaScript parser/stringifier (YAML 1.2, 1.1) (YTS)
  - js-yaml       # Native PyYAML port to JavaScript (Demo)

  Nim:
  - NimYAML       # YAML 1.2 implementation in pure Nim (YTS)

  OCaml:
  - ocaml-yaml    # YAML 1.1/1.2 via libyaml bindings
  - ocaml-syck    # YAML 1.0 via syck bindings

  Perl Modules:
  - YAML          # Pure Perl YAML 1.0 Module
  - YAML::XS      # Binding to libyaml
  - YAML::Syck    # Binding to libsyck
  - YAML::Tiny    # A small YAML subset module
  - YAML::PP      # A YAML 1.2/1.1 processor (YTS)

  PHP:
  - The Yaml Component  # Symfony Yaml Component (YAML 1.2)
  - php-yaml      # libyaml bindings (YAML 1.1)
  - syck          # syck bindings (YAML 1.0)
  - spyc          # yaml loader/dumper (YAML 1.?)

  Python:
  - PyYAML        # YAML 1.1, pure python and libyaml binding
  - ruamel.yaml   # YAML 1.2, update of PyYAML; comments round-trip
  - PySyck        # YAML 1.0, syck binding
  - strictyaml    # Restricted YAML subset

  R:
  - R YAML        # libyaml wrapper

  Raku:
  - YAMLish       # Port of YAMLish to Raku
  - YAML::Parser::LibYAML  # LibYAML wrapper

  Ruby:
  - psych         # libyaml wrapper (in Ruby core for 1.9.2)
  - RbYaml        # YAML 1.1 (PyYAML Port)
  - yaml4r        # YAML 1.0, standard library syck binding

  Rust:
  - yaml-rust     # YAML 1.2 implementation in pure Rust
  - serde-yaml    # YAML de/serialization of structs

  Shell:
  - parse_yaml    # Simple YAML parser for Bash using sed and awk
  - shyaml        # Read YAML files - jq style

  Swift:
  - Yams          # libyaml wrapper

  Others:
  - yamlvim       # YAML dumper/emitter in pure vimscript

Related Projects:
  - Rx            # Multi-Language Schemata Tool for JSON/YAML
  - Kwalify       # Ruby Schemata Tool for JSON/YAML 
  - pyKwalify     # Python Schemata Tool for JSON/YAML
  - yatools.net   # Visual Studio editor for YAML
  - JSON          # Official JSON Website
  - Pygments      # Python language Syntax Colorizer /w YAML support
  - yamllint      # YAML Linter based on PyYAML
  - YAML Diff     # Semantically compare two YAML documents
  - JSON Schema   # YAML-compliant JSON standard for data validation

# Edit This Website
...
