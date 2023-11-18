JSON (JavaScript Object Notation) is a lightweight data-interchange format. It is easy for humans to read and write. It is easy for machines to parse and generate. It is based on a subset of the JavaScript Programming Language Standard ECMA-262 3rd Edition - December 1999. JSON is a text format that is completely language independent but uses conventions that are familiar to programmers of the C-family of languages, including C, C++, C#, Java, JavaScript, Perl, Python, and many others. These properties make JSON an ideal data-interchange language.

![JSON](https://github.com/bbauska/yaml/assets/41387907/b9cf0e09-5d5a-4080-8cf6-dd3aa60d2c2f)

![image](https://github.com/bbauska/yaml/assets/41387907/c6891e72-0835-488b-b497-663ff33ba9ec)

![image](https://github.com/bbauska/yaml/assets/41387907/afb84a25-bf5c-43b0-8fb2-7e3b71fc6908)

![image](https://github.com/bbauska/yaml/assets/41387907/a88754ae-e5c3-4899-b474-4d64fc11944b)

![image](https://github.com/bbauska/yaml/assets/41387907/b51b8f66-b826-4985-939b-c46525e13f64)

!["do" is a reserved word](https://github.com/bbauska/yaml/assets/41387907/a2896a00-c886-40a3-8e38-8a1b20f94bdd)

https://www.youtube.com/watch?v=TjVcVWB0oFk&list=PLEzQf147-uEoNCeDlRrXv6ClsLDN-HtNm

JSON is built on two structures:

A collection of name/value pairs. In various languages, this is realized as an object, record, struct, dictionary, hash table, keyed list, or associative array.
An ordered list of values. In most languages, this is realized as an array, vector, list, or sequence.
These are universal data structures. Virtually all modern programming languages support them in one form or another. It makes sense that a data format that is interchangeable with programming languages also be based on these structures.

In JSON, they take on these forms:

An object is an unordered set of name/value pairs. An object begins with {left brace and ends with }right brace. Each name is followed by :colon and the name/value pairs are separated by ,comma.


An array is an ordered collection of values. An array begins with [left bracket and ends with ]right bracket. Values are separated by ,comma.


A value can be a string in double quotes, or a number, or true or false or null, or an object or an array. These structures can be nested.


A string is a sequence of zero or more Unicode characters, wrapped in double quotes, using backslash escapes. A character is represented as a single character string. A string is very much like a C or Java string.


A number is very much like a C or Java number, except that the octal and hexadecimal formats are not used.


Whitespace can be inserted between any pair of tokens. Excepting a few encoding details, that completely describes the language.


json
element

value
object
array
string
number
"true"
"false"
"null"

object
'{' ws '}'
'{' members '}'

members
member
member ',' members

member
ws string ws ':' element

array
'[' ws ']'
'[' elements ']'

elements
element
element ',' elements

element
ws value ws

string
'"' characters '"'

characters
""
character characters

character
'0020' . '10FFFF' - '"' - '\'
'\' escape

escape
'"'
'\'
'/'
'b'
'f'
'n'
'r'
't'
'u' hex hex hex hex

hex
digit
'A' . 'F'
'a' . 'f'

number
integer fraction exponent

integer
digit
onenine digits
'-' digit
'-' onenine digits

digits
digit
digit digits

digit
'0'
onenine

onenine
'1' . '9'

fraction
""
'.' digits

exponent
""
'E' sign digits
'e' sign digits

sign
""
'+'
'-'

ws
""
'0020' ws
'000A' ws
'000D' ws
'0009' ws
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
What is YAML?
YAML is a data serialization language for storing information in a human-readable form. It originally stood for “Yet Another Markup Language” but has since been changed to “YAML Ain’t Markup Language” to distinguish itself as different from a true markup language.

It is similar to XML and JSON files but uses a more minimalist syntax even while maintaining similar capabilities. YAML is commonly used to create configuration files in Infrastructure as Code (IoC) programs or to manage containers in the DevOps development pipeline.

More recently, YAML has been used to create automation protocols that can execute a series of commands listed in a YAML file. This means your systems can be more independent and responsive without additional developer attention.

As more and more companies embrace DevOps and virtualization, YAML is quickly becoming a must-have skill for modern developer positions. YAML is also easy to incorporate with existing technologies through the support of popular technologies like Python using PyYAML library, Docker, or Ansible.


YAML vs JSON vs XML
YAML (.yml):

Human-readable code
Minimalist syntax
Solely designed for data
Similar inline style to JSON (is a superset of JSON)
Allows comments
Strings without quotation marks
Considered the “cleaner” JSON
Advanced features (extensible data types, relational anchors, and mapping types preserving key order)
Use Case: YAML is best for data-heavy apps that use DevOps pipelines or VMs. It’s also helpful for when other developers on your team will work with this data often and therefore need it to be more readable.

JSON

Harder to read
Explicit, strict syntax requirements
Similar inline style to YAML (some YAML parsers can read JSON files)
No comments
Strings require double quotes
Use Case: JSON is favored in web development as it’s best for serialization formats and transmitting data over HTTP connections.

XML

Harder to read
More verbose
Acts as a markup language, while YAML is for data formatting
Contains more features than YAML, like tag attributes
More rigidly defined document schema
Use Case: XML is best for complex projects that require fine control over validation, schema, and namespace. XML is not human-readable and requires more bandwidth and storage capacity, but offers unparalleled control.
