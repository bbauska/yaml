# What is YAML?
YAML is a data serialization language for storing information in a human-readable form. It originally stood for “Yet Another Markup Language” but has since been changed to “YAML Ain’t Markup Language” to distinguish itself as different from a true markup language.

It is similar to XML and JSON files but uses a more minimalist syntax even while maintaining similar capabilities. YAML is commonly used to create configuration files in Infrastructure as Code (IoC) programs or to manage containers in the DevOps development pipeline.

More recently, YAML has been used to create automation protocols that can execute a series of commands listed in a YAML file. This means your systems can be more independent and responsive without additional developer attention.

As more and more companies embrace DevOps and virtualization, YAML is quickly becoming a must-have skill for modern developer positions. YAML is also easy to incorporate with existing technologies through the support of popular technologies like Python using PyYAML library, Docker, or Ansible.
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
In this chapter, you will learn the basic syntax of YAML.

## YAML basics
YAML is used to store lists or sequences of elements and key-value pairs or mappings.

  - List (also known as Sequence) is an ordered collection of items. A sequence is represented using square brackets ([]). Each item within the sequence is separated with a new line followed by comma (, ) character. An item can be of any type like strings, numbers or maps etc.

  - Key value pairs (also known as Mapping) is an unordered collection of key/value pairs. But, the keys are not unique because they are allowed to have duplicate values. Each element within a mapping is separated with new line followed by colon(:) character.
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### Key value pairs
A key-value pair is a data structure consisting of a key and a value. The key is used to identify the value, and the value can be any type of data.
<image>
Key-value pairs are represented using the following syntax:
<image>
where <key> represents name and <value> represents data separated by : (the space is mandatory).

Key-value pair example:
<image>
The following is the graphical representation of the key value pair:

![image](https://github.com/bbauska/yaml/assets/41387907/6bfabd62-ed2e-4ac7-a69b-f8c23d823494)

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
### List
A list is a simple data structure consisting of zero or more ordered items. In other words, a list is an ordered collection of data.
![visualization of list or sequence](https://github.com/bbauska/yaml/assets/41387907/5766947a-f6e4-4882-b28a-0429d76a71ac)

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

## Summary
  - Items of a list in YAML are represented by preceding it with - (hyphen).
  - Key value pairs in YAML are represented as <key>:<value>.
  - YAML is case sensitive.
  - YAML uses spaces and indentations to define document structure.
  - To define a YAML file we use either .yml or .yaml as file extension.
  - Different documents in YAML can be separated using three dashes (---).
  - You use three dots (...) to mark the end of a document without starting a new one.
  - A document in block style uses spaces to structure the document.
  - Flow style makes YAML an extension of JSON. Flow style is a little less human-readable than block style, however it provides more compactness to the document.
  - Any text after # not enclosed in ''(quotes) or "" (double quotes) is considered a comment.
  - YAML does not support block or multi-line comments.
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
## YAML vs JSON vs XML
### YAML (.yml):
  - Human-readable code
  - Minimalist syntax
  - Solely designed for data
  - Similar inline style to JSON (is a superset of JSON)
  - Allows comments
  - Strings without quotation marks
  - Considered the “cleaner” JSON
  - Advanced features (extensible data types, relational anchors, and mapping types preserving key order)

### <b>Use Case:</b>
YAML is best for data-heavy apps that use DevOps pipelines or VMs. It’s also helpful for when other developers on your team will work with this data often and therefore need it to be more readable.

### Salient Features of YAML
Here are some of the best features YAML has to offer.

### Multi-document support
You can have multiple YAML documents in a single YAML file to make file organization or data parsing easier.

The separation between each document is marked by three dashes (---)
<image>

### Built-in commenting
YAML allows you to add comments to files using the hash symbol (#) similar to Python comments.

<image>

### Readable syntax
YAML files use an indentation system similar to Python to show the structure of your program. You’re required to use spaces to create indentation rather than tabs to avoid confusion.

It also cuts much of the “noise” formatting found in JSON and XML files such as quotation marks, brackets, and braces.

Together, these formatting specifications increase the readability of YAML files beyond XML and JSON.
<yaml example>

<json example>

## Implicit and Explicit Typing
YAML offers versatility in typing by auto-detecting data types while also supporting explicit typing options. To tag data as a certain type, simply include !![typeName] before the value.
<image>

### No executable commands
As a data-representation format, YAML does not contain executables. It’s therefore very safe to exchange YAML files with external parties.

YAML must be integrated with other languages, like Perl or Java, to add executables.

## YAML Syntax
YAML has a few basic concepts that make up the majority of data.


### Key-value pairs
In general, most things in a YAML file are a form of key-value pair where the key represents the pair’s name and the value represents the data linked to that name. Key-value pairs are the basis for all other YAML constructions.
<image>

### Scalars and mapping
Scalars represent a single stored value. Scalars are assigned to key names using mapping. You define a mapping with a name, colon, and space, then a value for it to hold.

YAML supports common types like integer and floating-point numeric values, as well as non-numeric types Boolean and String.

Each can be represented in different ways, like hexadecimal, octal, or exponent. There are also special types for mathematical concepts like infinity, -infinity, and Not a Number (NAN)
<image>

### String
Strings are a collection of characters that represent a sentence or phrase. You either use | to print each string as a new line or > to print it as a paragraph.

Strings in YAML do not need to be in double-quotes.
<image>

### Sequence
Sequences are data structures similar to a list or array that hold multiple values under the same key. They’re defined using a block or inline flow style.

Block style uses spaces to structure the document. It’s easier to read but is less compact compared to flow style.
<image-1>

Flow style allows you to write sequences inline using square brackets, similar to an array declaration in a programming language like Python or JavaScript. Flow style is more compact but harder to read at a glance.
<image-2>

### Dictionaries
Dictionaries are collections of key-value pairs all nested under the same subgroup. They’re helpful to divide data into logical categories for later use.

Dictionaries are defined like mappings in that you enter the dictionary name, a colon, and a space followed by 1 or more indented key-value pairs.

<blockquote>
  Dictionaries can contain more complex structures as well, such as sequences. Nesting sequences is a good trick to represent complex relational data.
</blockquote>

## Advanced concepts to learn next
Congratulations on taking your first step toward learning YAML. While often overlooked, YAML is a simple and effective tool to pick up for your DevOps toolkit.

### Some next advanced topics to look at are:

  * Anchors
  * Templates
  * YAML with external tools (Docker, Ansible, etc.)
  * Advanced sequence/mapping types
  * Advanced data types (timestamp, null, etc.)

To help you pick up YAML fast, Educative has created the course <a href="https://www.educative.io/courses/introduction-to-yaml">Introduction to YAML</a>. This mini-course covers all YAML syntax in-depth from simple mappings to advanced anchoring techniques.

After less than an hour, you’ll have cracked all the essential YAML skills and earned a YAML certification for your DevOps resume.

Happy learning!
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
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
<script>if (window.location.protocol === "http:" && window.location.hostname === "yaml.org") { window.location.href = window.location.href.replace( "http:", "https:"); }</script>

<title>The Official YAML Web Site</title>

<link rel="stylesheet" type="text/css"
  href="css/screen.css" />

<link rel="icon" href="/favicon.svg" />

<pre class="content">
<span class="ydir">%YAML 1.2</span>
<span class="ydoc">---</span>
<span class="ykey">YAML</span><span class="ysep">:</span> YAML Ain't Markup Language™

<span class="ykey">What It Is</span><span class="ysep">:</span>
  YAML is a human-friendly data serialization
  language for all programming languages.

<span class="ykey">YAML Resources</span><span class="ysep">:</span>
  <span class="ykey">YAML Specifications</span><span class="ysep">:</span>
  - <span class="ykey">YAML 1.2</span><span class="ysep">:</span>
    - <a href="/spec/1.2.2/">Revision 1.2.2</a>      <span class="ycom"># Oct 1, 2021 <a href="https://yaml.com/blog/2021-10/new-yaml-spec/">*New*</a></span>
    - <a href="/spec/1.2.1/">Revision 1.2.1</a>      <span class="ycom"># Oct 1, 2009</span>
    - <a href="/spec/1.2.0/">Revision 1.2.0</a>      <span class="ycom"># Jul 21, 2009</span>
  - <a href="/spec/1.1">YAML 1.1</a>
  - <a href="/spec/1.0">YAML 1.0</a>

  <span class="ykey">YAML Matrix Chat</span><span class="ysep">:</span>  '<a href="https://matrix.to/#/#chat:yaml.io">#chat:yaml.io</a>'     <span class="ycom"># Our New Group Chat Room!</span>
  <span class="ykey">YAML IRC Channel</span><span class="ysep">:</span>  <a href="https://web.libera.chat/?channels#yaml">libera.chat#yaml</a>    <span class="ycom"># The old chat</span>
  <span class="ykey">YAML News</span><span class="ysep">:</span>         <a href="https://twitter.com/yamlnews">twitter.com/yamlnews</a>
  <span class="ykey">YAML Mailing List</span><span class="ysep">:</span> <a href="https://lists.sourceforge.net/lists/listinfo/yaml-core">yaml-core</a>           <span class="ycom"># Obsolete, but historical</span>

  <span class="ykey">YAML on GitHub</span><span class="ysep">:</span>                        <span class="ycom">#</span> <a href="https://github.com/yaml/">github.com/yaml/</a>
    <span class="ykey">YAML Specs</span><span class="ysep">:</span>        <a href="https://github.com/yaml/yaml-spec">yaml-spec/</a>
    <span class="ykey">YAML 1.2 Grammar</span><span class="ysep">:</span>  <a href="https://github.com/yaml/yaml-grammar">yaml-grammar/</a>
    <span class="ykey">YAML Test Suite</span><span class="ysep">:</span>   <a href="https://github.com/yaml/yaml-test-suite" name="yts">yaml-test-suite/</a>
    <span class="ykey">YAML Issues</span><span class="ysep">:</span>       <a href="https://github.com/yaml/yaml/issues">issues/</a>

  <span class="ykey">YAML Reference Parsers</span><span class="ysep">:</span>
  - <a href="https://github.com/yaml/yaml-reference-parser">Generated Reference Parsers</a>
  - <a href="http://ben-kiki.org/ypaste">YPaste Interactive Parser</a>

  <span class="ykey">YAML Test Matrix</span><span class="ysep">:</span>   <a href="https://matrix.yaml.io/">matrix.yaml.io</a>
<!--  <span class="ykey">YAML Docker Runtimes</span><span class="ysep">:</span> <a href="https://github.com/yaml/yaml-runtimes">/yaml-runtimes</a>
  <span class="ykey">YAML Cookbook (Ruby)</span><span class="ysep">:</span> <a href="YAML_for_ruby.html">YAML_for_ruby.html</a> --><!-- http://yaml4r.sourceforge.net/cookbook/ --><!--
-->
<span class="ykey">YAML Frameworks and Tools</span><span class="ysep">:</span>
  <span class="ykey">C/C++</span><span class="ysep">:</span>
  - <a href="https://github.com/pantoniou/libfyaml"               >libfyaml</a>      <span class="ycom"># "C" YAML 1.2 processor (<a href="#yts" title="Uses YAML Test Suite">YTS</a></span>)
  - <a href="http://pyyaml.org/wiki/LibYAML"                      >libyaml</a>       <span class="ycom"># "C" Fast YAML 1.1 (<a href="#yts" title="Uses YAML Test Suite">YTS</a></span>)
  - <a href="https://github.com/tlsa/libcyaml"                    >libcyaml</a>      <span class="ycom"># YAML de/serialization of C data (using libyaml)</span>
  - <a href="https://github.com/jbeder/yaml-cpp/"                 >yaml-cpp</a>      <span class="ycom"># C++ YAML 1.2 implementation</span>

  <span class="ykey">Crystal</span><span class="ysep">:</span>
  - <a href="https://crystal-lang.org/api/latest/YAML.html"       >YAML</a>          <span class="ycom"># YAML 1.1 from the standard library</span>

  <span class="ykey">C#/.NET</span><span class="ysep">:</span>
  - <a href="https://github.com/aaubry/YamlDotNet"                >YamlDotNet</a>    <span class="ycom"># YAML 1.1/(1.2) library + serialization (<a href="#yts" title="Uses YAML Test Suite">YTS</a></span>)
  - <a href="http://yaml-net-parser.sourceforge.net/"             >yaml-net</a>      <span class="ycom"># YAML 1.1 library</span>

  <span class="ykey">D</span><span class="ysep">:</span>
  - <a href="https://github.com/dlang-community/D-YAML"           >D-YAML</a>        <span class="ycom"># YAML 1.1 library w/ official community support (<a href="#yts" title="Uses YAML Test Suite">YTS</a></span>)

  <span class="ykey">Dart</span><span class="ysep"    >:</span>
  - <a href="https://pub.dartlang.org/packages/yaml"              >yaml</a>          <span class="ycom"># YAML package for Dart</span>

  <span class="ykey">Delphi</span><span class="ysep">:</span>
  - <a href="https://github.com/neslib/Neslib.Yaml"               >Neslib.Yaml</a>   <span class="ycom"># YAML 1.1 Delphi binding to libyaml (<a href="#yts" title="Uses YAML Test Suite">YTS</a></span>)

  <span class="ykey">Elixir</span><span class="ysep">:</span>
  - <a href="https://github.com/KamilLelonek/yaml-elixir"         >yaml-elixir</a>   <span class="ycom"># YAML support for the Elixir language</span>

  <span class="ykey">Erlang</span><span class="ysep">:</span>
  - <a href="https://github.com/yakaz/yamerl"                     >yamerl</a>        <span class="ycom"># YAML support for the Erlang language</span>

  <span class="ykey">Golang</span><span class="ysep">:</span>
  - <a href="https://github.com/go-yaml/yaml"                     >Go-yaml</a>       <span class="ycom"># YAML support for the Go language</span>
  - <a href="https://github.com/kylelemons/go-gypsy"              >Go-gypsy</a>      <span class="ycom"># Simplified YAML parser written in Go</span>
  - <a href="https://github.com/goccy/go-yaml"                    >goccy/go-yaml</a> <span class="ycom"># YAML 1.2 implementation in pure Go</span>

  <span class="ykey">Haskell</span><span class="ysep">:</span>
  - <a href="https://hackage.haskell.org/package/HsYAML"          >HsYAML</a>         <span class="ycom"># YAML 1.2 implementation in pure Haskell (<a href="#yts" title="Uses YAML Test Suite">YTS</a></span>)
  - <a href="https://hackage.haskell.org/package/YamlReference"   >YamlReference</a>  <span class="ycom"># Haskell 1.2 reference parser</span>
  - <a href="https://hackage.haskell.org/package/yaml"            >yaml</a>           <span class="ycom"># YAML 1.1 Haskell framework (based on libyaml)</span>

  <span class="ykey">Java</span><span class="ysep">:</span>
  - <a href="https://bitbucket.org/snakeyaml/snakeyaml-engine"    >SnakeYAML Engine</a>  <span class="ycom"># Java 8+ / YAML 1.2</span>
  - <a href="https://bitbucket.org/snakeyaml/snakeyaml"           >SnakeYAML</a>         <span class="ycom"># Java 5 / YAML 1.1</span>
  - <a href="https://github.com/EsotericSoftware/yamlbeans"       >YamlBeans</a>         <span class="ycom"># To/from JavaBeans. YAML 1.0/1.1</span>
  - <a href="https://github.com/decorators-squad/eo-yaml"         >eo-yaml</a>           <span class="ycom"># YAML 1.2 for Java 8. Packaged as a Module (Java 9+)</span>
  - <a href="https://github.com/OpenHFT/Chronicle-Wire"           >Chronicle-Wire</a>    <span class="ycom"># Java Implementation</span>

  <span class="ykey">JavaScript</span><span class="ysep">:</span>
  - <a href="https://github.com/eemeli/yaml"                      >yaml</a>          <span class="ycom"># JavaScript parser/stringifier (YAML 1.2, 1.1) (<a href="#yts" title="Uses YAML Test Suite">YTS</a></span>)
  - <a href="https://github.com/nodeca/js-yaml"                   >js-yaml</a>       <span class="ycom"># Native PyYAML port to JavaScript (<a href="https://nodeca.github.io/js-yaml/">Demo</a></span>)

  <span class="ykey">Nim</span><span class="ysep">:</span>
  - <a href="https://nimyaml.org"                                 >NimYAML</a>       <span class="ycom"># YAML 1.2 implementation in pure Nim (<a href="#yts" title="Uses YAML Test Suite">YTS</a></span>)

  <span class="ykey">OCaml</span><span class="ysep">:</span>
  - <a href="https://github.com/avsm/ocaml-yaml"                  >ocaml-yaml</a>    <span class="ycom"># YAML 1.1/1.2 via libyaml bindings</span>
  - <a href="http://ocaml-syck.sourceforge.net"                   >ocaml-syck</a>    <span class="ycom"># YAML 1.0 via syck bindings</span>

  <span class="ykey">Perl Modules</span><span class="ysep">:</span>
  - <a href="https://metacpan.org/release/YAML"                   >YAML</a>          <span class="ycom"># Pure Perl YAML 1.0 Module</span>
  - <a href="https://metacpan.org/release/YAML-LibYAML"           >YAML::XS</a>      <span class="ycom"># Binding to libyaml</span>
  - <a href="https://metacpan.org/release/YAML-Syck"              >YAML::Syck</a>    <span class="ycom"># Binding to libsyck</span>
  - <a href="https://metacpan.org/release/YAML-Tiny"              >YAML::Tiny</a>    <span class="ycom"># A small YAML subset module</span>
  - <a href="https://metacpan.org/release/YAML-PP"                >YAML::PP</a>      <span class="ycom"># A YAML 1.2/1.1 processor (<a href="#yts" title="Uses YAML Test Suite">YTS</a></span>)

  <span class="ykey">PHP</span><span class="ysep">:</span>
  - <a href="https://symfony.com/doc/current/components/yaml.html">The Yaml Component</a>  <span class="ycom"># Symfony Yaml Component (YAML 1.2)</span>
  - <a href="http://pecl.php.net/package/yaml"                    >php-yaml</a>      <span class="ycom"># libyaml bindings (YAML 1.1)</span>
  - <a href="http://pecl.php.net/package/syck"                    >syck</a>          <span class="ycom"># syck bindings (YAML 1.0)</span>
  - <a href="https://github.com/mustangostang/spyc"               >spyc</a>          <span class="ycom"># yaml loader/dumper (YAML 1.?)</span>

  <span class="ykey">Python</span><span class="ysep">:</span>
  - <a href="http://pyyaml.org"                                   >PyYAML</a>        <span class="ycom"># YAML 1.1, pure python and libyaml binding</span>
  - <a href="https://pypi.python.org/pypi/ruamel.yaml"            >ruamel.yaml</a>   <span class="ycom"># YAML 1.2, update of PyYAML; comments round-trip</span>
  - <a href="https://github.com/yaml/pysyck"                      >PySyck</a>        <span class="ycom"># YAML 1.0, syck binding</span>
  - <a href="https://pypi.org/project/strictyaml/"                >strictyaml</a>    <span class="ycom"># Restricted YAML subset</span>

  <span class="ykey">R</span><span class="ysep">:</span>
  - <a href="https://github.com/viking/r-yaml"                    >R YAML</a>        <span class="ycom"># libyaml wrapper</span>

  <span class="ykey">Raku</span><span class="ysep">:</span>
  - <a href="https://github.com/Leont/yamlish"                    >YAMLish</a>       <span class="ycom"># Port of YAMLish to Raku</span>
  - <a href="https://github.com/tony-o/perl6-libyaml"             >YAML::Parser::LibYAML</a>  <span class="ycom"># LibYAML wrapper</span>

  <span class="ykey">Ruby</span><span class="ysep">:</span>
  - <a href="http://github.com/tenderlove/psych"                  >psych</a>         <span class="ycom"># libyaml wrapper (in Ruby core for 1.9.2)</span>
  - <a href="https://rubygems.org/gems/RbYAML/versions/0.2.0"     >RbYaml</a>        <span class="ycom"># YAML 1.1 (PyYAML Port)</span>
  - <a href="http://yaml4r.sourceforge.net/doc/"                  >yaml4r</a>        <span class="ycom"># YAML 1.0, standard library syck binding</span>

  <span class="ykey">Rust</span><span class="ysep">:</span>
  - <a href="https://github.com/chyh1990/yaml-rust"               >yaml-rust</a>     <span class="ycom"># YAML 1.2 implementation in pure Rust</span>
  - <a href="https://github.com/dtolnay/serde-yaml"               >serde-yaml</a>    <span class="ycom"># YAML de/serialization of structs</span>

  <span class="ykey">Shell</span><span class="ysep">:</span>
  - <a href="https://github.com/mrbaseman/parse_yaml"             >parse_yaml</a>    <span class="ycom"># Simple YAML parser for Bash using sed and awk</span>
  - <a href="https://pypi.org/project/shyaml/"                    >shyaml</a>        <span class="ycom"># Read YAML files - jq style</span>

  <span class="ykey">Swift</span><span class="ysep">:</span>
  - <a href="https://github.com/jpsim/Yams"                       >Yams</a>          <span class="ycom"># libyaml wrapper</span>

  <span class="ykey">Others</span><span class="ysep">:</span>
  - <a href="http://www.vim.org/scripts/script.php?script_id=3191">yamlvim</a>       <span class="ycom"># YAML dumper/emitter in pure vimscript</span>

<span class="ykey">Related Projects</span><span class="ysep">:</span>
  - <a href="http://rjbs.manxome.org/rx/"                 >Rx</a>            <span class="ycom"># Multi-Language Schemata Tool for JSON/YAML</span>
  - <a href="ihttps://www.rubydoc.info/gems/kwalify/"     >Kwalify</a>       <span class="ycom"># Ruby Schemata Tool for JSON/YAML</span> <!--  - <a href="http://github.com/trans/yaml_vim/tree/master">yaml_vim</a>      <span class="ycom"># vim syntax files for YAML</span> -->
  - <a href="https://github.com/Grokzen/pykwalify"        >pyKwalify</a>     <span class="ycom"># Python Schemata Tool for JSON/YAML</span>
  - <a href="http://www.codeplex.com/yaml/"               >yatools.net</a>   <span class="ycom"># Visual Studio editor for YAML</span>
  - <a href="http://json.org/"                            >JSON</a>          <span class="ycom"># Official JSON Website</span>
  - <a href="http://pygments.org/demo/?lang=yaml"         >Pygments</a>      <span class="ycom"># Python language Syntax Colorizer /w YAML support</span>
  - <a href="https://github.com/adrienverge/yamllint"     >yamllint</a>      <span class="ycom"># YAML Linter based on PyYAML</span>
  - <a href="https://yamldiff.com/"                       >YAML Diff</a>     <span class="ycom"># Semantically compare two YAML documents</span>
  - <a href="https://json-schema-everywhere.github.io/yaml">JSON Schema</a>   <span class="ycom"># YAML-compliant JSON standard for data validation</span>
<!--
<span class="ykey">News</span><span class="ysep">:</span>
  - 20-NOV-2011 -- <a href="https://github.com/nodeca/js-yaml">JS-YAML</a>, a JavaScript YAML parser by <a href="https://github.com/ixti">Alexey Zapparov</a> and <a href="https://github.com/puzrin">Vitaly Puzrin</a>.
  - 18-AUG-2010 -- <a href="http://svn.ruby-lang.org/repos/ruby/tags/v1_9_2_0/NEWS">Ruby 1.9.2 includes psych</a>, a libyaml wrapper by <a href="http://github.com/tenderlove">Aaron Patterson</a>. <!--  - 17-AUG-2010 -- <a href="http://yamlvim.hg.sourceforge.net/hgweb/yamlvim/yamlvim/summary">vimscript parser/emitter</a> was created by Nikolay Pavlov. - - >
  - 01-OCT-2009 -- <a href="spec/1.2/">YAML 1.2 (3rd Edition) was patched</a>.
  - 21-JUL-2009 -- <a href="spec/1.2/">YAML 1.2 (3rd Edition) was released</a>.
  - 28-APR-2009 -- <a href="http://trac-hg.assembla.com/snakeyaml/">A new version of SnakeYAML was released</a>.
  - 01-APR-2009 -- The YAML 1.2 spec was planned to be finalized by the end of the month.
  - 07-JAN-2009 -- <a href="http://trac-hg.assembla.com/snakeyaml/">Andrey Somov releases SnakeYAML, a 1.1 YAML Parser</a>
  - 03-JAN-2009 -- <a href="http://www.codeplex.com/yaml/">Burt Harris announced YAML for .NET and editor for Visual Studio</a>
  - 02-DEC-2008 -- <a href="http://code.google.com/p/yaml-cpp/">Jesse Beder released YAML for C++</a>
  - 11-MAY-2008 -- <a href="spec/1.2/">Oren Ben-Kiki has released a new YAML 1.2 spec draft</a>
  - 29-NOV-2007 -- <a href="http://pecl.php.net/package/syck">Alexey Zakhlestin has updated his Syck (YAML 1.0) binding for PHP</a> <!--  - 23-NOV-2007 -- <a href="http://flexonrails.net/?p=98">Derek Wischusen has release Action Script 3 YAML 1.1</a> - - >
  - 01-AUG-2006 -- <a href="http://pyyaml.org/wiki/LibYAML">Kirill Simonov has released libyaml, a parser and emitter in "C"</a> <!--  - 06-JUN-2006 -- <a href="http://jvyaml.dev.java.net">Ola Bini is at it again, this time with a Java implementation</a> - - > <!--  - 03-JUN-2006 -- <a href="http://lumumba.uhasselt.be/~christophe/YAML/">Christophe Lambrechts and Jonathan Slenders announced a .NET parser</a> - - > <!--  - 07-MAY-2006 -- <a href="http://rbyaml.rubyforge.org">Ola Bini released a pure-ruby YAML 1.1 parser and emitter</a> - - >
  - 12-APR-2006 -- Kirill's YAML 1.1 parser for Python is now at PyYAML
  - 05-FEB-2006 -- <a href="http://spyc.sf.net">Spyc YAML for PHP is now at version 0.3</a>
  - 17-DEC-2005 -- <a href="https://www.rubydoc.info/gems/kwalify/">Makoto Kuwata has released Kwalify 0.5, YAML/JSON schema validator</a>
  - 14-DEC-2005 -- <a href="http://jyaml.sourceforge.net">Toby Ho has released Jyaml, a Java library for YAML based on Rolf Veen's work</a> <!--  - 30-AUG-2005 -- <a href="http://pyyaml.org/wiki/PySyck">Kirill Simonov has produce a wonderful Python binding for Syck</a> - - >
  - 08-APR-2005 -- <a href="http://json.org">As it turns out, YAML is a superset of the JSON serialization language</a>
  - 18-MAY-2005 -- <a href="http://whytheluckystiff.net/syck/">Why has released version 0.55 of Syck</a>
  - 28-DEC-2004 -- <a href="spec/">Announcing YAML 1.1 Working Draft</a>
  - 01-OCT-2004 -- <a href="http://will.thimbleby.net/yaml.html">YAML for Cocoa was released by Will Thimbley</a>
  - 08-FEB-2004 -- <a href="http://sourceforge.net/projects/yaml-javascript">Slaven Rezic announced a new version of his JavaScript binding</a>
  - 29-JAN-2004 -- Ingy, Oren, and Clark spent 4 days hacking on the spec in Portland.
  - 10-OCT-2003 -- The Syck implementation with bindings for Ruby, Python,
                   and PHP is now at version .41
  - 26-APR-2003 -- Mike Orr has taken over the Pure Python development.
  - 26-APR-2003 -- Brian Ingerson has created a FIT platform for Wiki-like testing.
  - 24-JAN-2003 -- Updates to specification.
  - 25-JUL-2002 -- Both the Ruby and Python parsers have made significant progress.
                   There is an article about YAML by Kendall Grant Clark at xml.com.
                   There is also a draft XML binding.
  - 02-JUL-2002 -- Brian Ingerson will be giving a 45 minute presentation on YAML at the
                   O'Reilly Open Source Conference in San Diego on July 24th 2002.
  - 01-FEB-2002 -- Brian's Perl implementation YAML.pm, has been updated with new documentation.
                   Included in this release is YSH, a test shell for learning how YAML works.
  - 03-JAN-2002 -- YAML(tm) starts the new year with a new name YAML Ain't Markup Language.
  - 17-MAY-2001 -- YAML now has a mailing list at SourceForge.
  - 15-MAY-2001 -- YAML is started with a first pass specification.
-->
