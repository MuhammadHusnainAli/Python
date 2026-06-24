# PYTHON  Complete Learning Roadmap

**LEARNING ROADMAP**
Python 3.10 → 3.14 · compiled from docs.python.org

**Every topic · every standard-library module · every change, 3.10–3.14**

A single, nothing-skipped study path across the whole language: the core syntax and data model, the entire standard library module-by-module, the type system, the runtime and concurrency story, and the new features of every release from 3.10 through 3.14.

Built from the official Python documentation  the Language Reference, the Standard Library reference, and the "What's New" guides at docs.python.org.

**Last Updated :  June 15, 2026**

`Python 3.10` `Python 3.11` `Python 3.12` `Python 3.13` `Python 3.14`

---

## Contents

**[Getting Started: Setup, Tooling & Mental Model](#part-0-getting-started-setup-tooling--mental-model)**
- [0.1 What Python is](#01-what-python-is)
- [0.2 Installing Python](#02-installing-python)
- [0.3 Running Python](#03-running-python)
- [0.4 Editors, IDEs & developer tooling](#04-editors-ides--developer-tooling)
- [0.5 Virtual environments & a first taste of packaging](#05-virtual-environments--a-first-taste-of-packaging)

**[Core Language Foundations](#part-1-core-language-foundations)**
- [1.1 Lexical structure (how source text is read)](#11-lexical-structure-how-source-text-is-read)
- [1.2 Variables, objects & assignment](#12-variables-objects--assignment)
- [1.3 Numbers](#13-numbers)
- [1.4 Strings & text](#14-strings--text)
- [1.5 Sequences: list, tuple, range](#15-sequences-list-tuple-range)
- [1.6 Sets & mappings](#16-sets--mappings)
- [1.7 Binary data types](#17-binary-data-types)
- [1.8 Operators & expressions](#18-operators--expressions)
- [1.9 Control flow](#19-control-flow)

**[Functions, Iteration, Errors & Context Managers](#part-2-functions-iteration-errors--context-managers)**
- [2.1 Functions](#21-functions)
- [2.2 Comprehensions & generator expressions](#22-comprehensions--generator-expressions)
- [2.3 Iterators & generators](#23-iterators--generators)
- [2.4 Exceptions & error handling](#24-exceptions--error-handling)
- [2.5 Context managers & the with statement](#25-context-managers--the-with-statement)

**[Object-Oriented Python & the Data Model](#part-3-object-oriented-python--the-data-model)**
- [3.1 Classes & instances](#31-classes--instances)
- [3.2 Inheritance & composition](#32-inheritance--composition)
- [3.3 The data model (special / "dunder" methods)](#33-the-data-model-special--dunder-methods)
- [3.4 Metaclasses & class creation](#34-metaclasses--class-creation)
- [3.5 Dataclasses & enumerations](#35-dataclasses--enumerations)
- [3.6 Generics & type parameters (the OOP angle)](#36-generics--type-parameters-the-oop-angle)

**[Type Hints & Static Typing](#part-4-type-hints--static-typing)**
- [4.1 Annotation fundamentals](#41-annotation-fundamentals)
- [4.2 The typing vocabulary](#42-the-typing-vocabulary)
- [4.3 Typing in practice](#43-typing-in-practice)

**[Modules, Packages & the Import System](#part-5-modules-packages--the-import-system)**
- [5.1 Modules](#51-modules)
- [5.2 Packages](#52-packages)
- [5.3 The import system internals](#53-the-import-system-internals)

**[The Standard Library: Complete Module Reference](#part-6-the-standard-library-complete-module-reference)**
- [6.1 Built-in functions, constants, types & exceptions](#61-built-in-functions-constants-types--exceptions)
- [6.2 Text Processing Services](#62-text-processing-services)
- [6.3 Binary Data Services](#63-binary-data-services)
- [6.4 Data Types](#64-data-types)
- [6.5 Numeric & Mathematical Modules](#65-numeric--mathematical-modules)
- [6.6 Functional Programming Modules](#66-functional-programming-modules)
- [6.7 File & Directory Access](#67-file--directory-access)
- [6.8 Data Persistence](#68-data-persistence)
- [6.9 Data Compression & Archiving](#69-data-compression--archiving)
- [6.10 File Formats](#610-file-formats)
- [6.11 Cryptographic Services](#611-cryptographic-services)
- [6.12 Generic Operating System Services](#612-generic-operating-system-services)
- [6.13 Command-line interface libraries](#613-command-line-interface-libraries)
- [6.14 Concurrent Execution](#614-concurrent-execution)
- [6.15 Networking & Interprocess Communication](#615-networking--interprocess-communication)
- [6.16 Internet Data Handling](#616-internet-data-handling)
- [6.17 Structured Markup Processing Tools](#617-structured-markup-processing-tools)
- [6.18 Internet Protocols & Support](#618-internet-protocols--support)
- [6.19 Multimedia Services](#619-multimedia-services)
- [6.20 Internationalization](#620-internationalization)
- [6.21 Graphical User Interfaces with Tk](#621-graphical-user-interfaces-with-tk)
- [6.22 Development Tools](#622-development-tools)
- [6.23 Debugging & Profiling](#623-debugging--profiling)
- [6.24 Software Packaging & Distribution](#624-software-packaging--distribution)
- [6.25 Python Runtime Services](#625-python-runtime-services)
- [6.26 Custom Python Interpreters](#626-custom-python-interpreters)
- [6.27 Importing Modules](#627-importing-modules)
- [6.28 Python Language Services](#628-python-language-services)
- [6.29 MS Windows Specific Services](#629-ms-windows-specific-services)
- [6.30 Unix-specific Services](#630-unix-specific-services)
- [6.31 Superseded Modules](#631-superseded-modules)
- [6.32 Removed Modules (know what is gone)](#632-removed-modules-know-what-is-gone)
- [6.33 Security Considerations](#633-security-considerations)

**[Concurrency, Parallelism & Asynchronous Programming](#part-7-concurrency-parallelism--asynchronous-programming)**
- [7.1 The execution model: GIL & free threading](#71-the-execution-model-gil--free-threading)
- [7.2 Threading](#72-threading)
- [7.3 Multiprocessing & process pools](#73-multiprocessing--process-pools)
- [7.4 Subinterpreters](#74-subinterpreters)
- [7.5 Asynchronous programming with asyncio](#75-asynchronous-programming-with-asyncio)

**[Performance, Internals & the CPython Runtime](#part-8-performance-internals--the-cpython-runtime)**
- [8.1 Compilation & bytecode](#81-compilation--bytecode)
- [8.2 The interpreter & JIT](#82-the-interpreter--jit)
- [8.3 Memory management](#83-memory-management)
- [8.4 Profiling, monitoring & debugging at runtime](#84-profiling-monitoring--debugging-at-runtime)
- [8.5 Extending & embedding (C interop)](#85-extending--embedding-c-interop)

**[Testing, Packaging, Distribution & Project Workflow](#part-9-testing-packaging-distribution--project-workflow)**
- [9.1 Testing & quality](#91-testing--quality)
- [9.2 Style, docs & static checks](#92-style-docs--static-checks)
- [9.3 Packaging & distribution](#93-packaging--distribution)

**[What's New, Version by Version (3.10 → 3.14)](#part-10-whats-new-version-by-version-310--314)**
- [10.1 Python 3.10 (October 2021)](#101-python-310-october-2021)
- [10.2 Python 3.11 (October 2022)](#102-python-311-october-2022)
- [10.3 Python 3.12 (October 2023)](#103-python-312-october-2023)
- [10.4 Python 3.13 (October 2024)](#104-python-313-october-2024)
- [10.5 Python 3.14 (October 2025)](#105-python-314-october-2025)
- [10.6 Deprecations & removals: staying current](#106-deprecations--removals-staying-current)

**[The Ecosystem & Where to Go Next](#part-11-the-ecosystem--where-to-go-next)**
- [11.1 PyPI & popular libraries by domain](#111-pypi--popular-libraries-by-domain)
- [11.2 Official resources & next steps](#112-official-resources--next-steps)

**[Built-in Functions: Complete List](#appendix-a-built-in-functions-complete-list)**
- [A. The built-ins](#a-the-built-ins)

**[Built-in Exception Hierarchy](#appendix-b-built-in-exception-hierarchy)**
- [B. Hierarchy](#b-hierarchy)

**[Keywords & Soft Keywords](#appendix-c-keywords--soft-keywords)**
- [C. Reserved words](#c-reserved-words)

**[Operator Precedence (high → low)](#appendix-d-operator-precedence-high--low)**
- [D. Precedence table](#d-precedence-table)

**[Standard-Library Module Checklist](#appendix-e-standard-library-module-checklist)**
- [E. Every module, by group](#e-every-module-by-group)

**[Official Documentation Map](#appendix-f-official-documentation-map)**
- [F. Documentation sections](#f-documentation-sections)

---

## How to use this roadmap

This document is a complete topical map of the Python programming language as it stands across versions 3.10, 3.11, 3.12, 3.13 and 3.14. Its organisation mirrors the official documentation at docs.python.org: the Tutorial and Language Reference feed the core-language parts, the Standard Library reference feeds the complete module catalogue, and the five "What's New" guides feed the version-by-version part and the version badges sprinkled throughout.

It is built to be exhaustive at the level of topics and modules: every standard-library module shipped with CPython 3.14 appears in Part 6, and every major language construct appears in Parts 1–5. Each node is deliberately concise: think of it as a checklist and a study path rather than a replacement for the manual. For the full detail of any single item, open the corresponding page on docs.python.org; the structure here matches it one-to-one so you will always find it.

Suggested use: work top-to-bottom for a from-scratch journey (Parts 0–3 are the foundations, 4–5 round out the language, 6 is reference you return to constantly, 7–9 are the professional layer). If you already know the basics, treat Part 6 as a coverage checklist and use Part 10 to catch up on what changed between the version you learned and 3.14.

### Legend

- **[3.x]**: a feature introduced (or made the default / stabilized) in that Python version. Badges are attached to the exact topic they affect.
- `monospace`: a module, function, keyword, operator, or other literal code identifier.
- Items are ordered roughly beginner → advanced within each part, but the roadmap is also a checklist: every node is something to learn.

---

# PART 0: Getting Started: Setup, Tooling & Mental Model

Install, run, and understand what Python is before writing real code.

Everything you need in place before the language itself: obtaining an interpreter, running code three different ways, isolating projects, and a clear picture of how Python executes.

## 0.1 What Python is

- **Language vs implementation**: Python the language spec vs CPython the reference implementation; the difference matters for performance and C extensions.
- **Alternate implementations**: CPython, PyPy (JIT), Jython, IronPython, MicroPython, GraalPy: same language, different runtimes.
- **Interpreted & dynamically typed**: Source compiled to bytecode, executed by a virtual machine; types are checked at runtime.
- **The release cycle**: One feature release per year (3.x), monthly bugfix releases, ~5 years of support per version; alphas, betas, release candidates.
- **Versioning & EOL**: Know which versions are supported; 3.9 retired around the 3.14 release. Pick a version that is current and supported.

## 0.2 Installing Python

- **Official installers**: Download from python.org for Windows, macOS and source; verify downloads.
- **Windows install manager**: The new `py`-based install manager (Store or download) replaces the legacy Windows installer.
- **macOS / Linux**: System Python vs a managed install; on Linux use the distro packages or build from source.
- **Version managers**: `pyenv` and similar tools to install and switch between many Python versions per project.
- **The `py` launcher (Windows)**: Select interpreter versions with `py -3.14`; understand shebang handling.
- **Verifying an install**: `python --version`, `python -V`, locating the executable, multiple side-by-side versions.
- **[3.14]** Official Android binary releases are now available; official macOS/Windows binaries ship an experimental JIT. PGP signatures are discontinued (PEP 761) in favour of Sigstore.
- **[3.13]** Android and iOS became Tier-3 supported platforms; an experimental free-threaded build is offered in the Windows/macOS installers.

## 0.3 Running Python

- **The interactive interpreter (REPL)**: Start `python`, evaluate expressions, `_` last result, `help()`, `exit()`.
- **The new PyREPL**: Multiline editing, history browsing, bracketed paste, colour prompts; `PYTHON_BASIC_REPL` to fall back.
- **Running scripts**: `python script.py`, shebang lines, making files executable, `__name__ == "__main__"`.
- **Running modules & packages**: `python -m module`, `-m pip`, `-m venv`, running a package via `__main__.py`, zipapps.
- **Command-line interface**: `-c`, `-m`, `-i`, `-O`/`-OO`, `-B`, `-W`, `-X` options, `-` for stdin, exit codes.
- **Environment variables**: `PYTHONPATH`, `PYTHONSTARTUP`, `PYTHONDONTWRITEBYTECODE`, `PYTHONUTF8`, `PYTHONWARNINGS`, `PYTHON_COLORS`, `NO_COLOR`, `PYTHON_JIT`.
- **[3.13]** Brand-new interactive interpreter based on PyPy's, with multiline editing and colourised tracebacks by default.
- **[3.14]** Syntax highlighting in the default REPL, and colour output in several stdlib CLIs (`unittest`, `argparse`, `json`, `calendar`).

## 0.4 Editors, IDEs & developer tooling

- **Editors / IDEs**: VS Code, PyCharm, vim/neovim, the bundled IDLE; language servers and autocompletion.
- **Linters & formatters**: `ruff`, `flake8`, `pylint`, `black`, `isort`: third-party, but standard practice (PEP 8 conformance).
- **Type checkers**: `mypy`, `pyright`/Pylance run the static analysis the `typing` module enables (Part 4).
- **Debuggers**: Built-in `pdb`; IDE debuggers; new remote attach interface (Part 8).
- **REPL alternatives**: IPython and Jupyter for exploratory/data work (third-party).

## 0.5 Virtual environments & a first taste of packaging

- **Why isolate**: Per-project dependency isolation; avoid polluting the system interpreter.
- **`venv`**: `python -m venv .venv`, activate/deactivate, where packages land, recreating environments.
- **`pip`**: Installing, upgrading, uninstalling, `requirements.txt`, `pip freeze`, editable installs.
- **`ensurepip`**: How `pip` is bootstrapped into a fresh environment.
- **Project metadata**: First sight of `pyproject.toml`; full packaging is Part 9.
- **Alternative managers**: `uv`, `poetry`, `pipenv`, `conda`: third-party workflow tools to be aware of.

---

# PART 1: Core Language Foundations

Lexical structure, the built-in data types, operators, and control flow.

The syntax and the data you manipulate. Maps to the Tutorial chapters 1–5 and to the Language Reference chapters 2 (Lexical analysis), 6 (Expressions) and parts of 7–8.

## 1.1 Lexical structure (how source text is read)

- **Line structure**: Logical vs physical lines, explicit line joining with `\`, implicit joining inside brackets, blank lines.
- **Indentation**: Significant whitespace, INDENT/DEDENT, tabs vs spaces, consistent blocks.
- **Tokens**: Identifiers, keywords, literals, operators, delimiters, NEWLINE/INDENT/DEDENT.
- **Identifiers & keywords**: Naming rules, Unicode identifiers, reserved keywords, soft keywords (`match`, `case`, `type`, `_`).
- **Comments & encoding**: `#` comments, the source encoding declaration, UTF-8 default.
- **Literals**: String, bytes, numeric, and the boolean/None literals.
- **String & bytes literals**: Quote styles, triple quotes, escape sequences, raw `r""`, byte `b""`, f-strings `f""`, template strings `t""`.
- **Numeric literals**: Integer (incl. `0x`/`0o`/`0b`), float, imaginary `j`, underscores in numerals `1_000_000`.
- **Operators & delimiters**: The full operator/delimiter set, including `:=`, `@`, `->`, augmented assignment.
- **[3.12]** f-strings were formalised in the grammar (PEP 701): arbitrary nesting, reuse of quotes, multi-line expressions, backslashes and comments inside `{}`.
- **[3.14]** Template string literals `t"..."` produce a `Template` (PEP 750) for safe, custom interpolation: a sibling to f-strings.

## 1.2 Variables, objects & assignment

- **Names bind to objects**: Variables are references; assignment binds a name, it does not copy.
- **Objects, identity, type, value**: `id()`, `type()`, `is` vs `==`, mutability vs immutability.
- **Interning & caching**: Small-integer cache (`-5` to `256`), string interning, `sys.intern()`; why `is` is unreliable for value comparison.
- **Assignment forms**: Simple, multiple targets `a = b = 0`, tuple/list unpacking, starred targets `a, *rest = ...`, nested unpacking.
- **Augmented assignment**: `+=`, `-=`, ... and how they differ for mutable vs immutable targets.
- **Assignment expressions**: The walrus operator `:=` for binding inside expressions.
- **`del`**: Unbinding names and removing items/slices/attributes.
- **Constants & conventions**: There are no true constants; UPPER_CASE convention, `Final` (Part 4).

## 1.3 Numbers

- **`int`**: Arbitrary precision, bit operations, `int.bit_length()`, `to_bytes`/`from_bytes`, integer-string conversion length limit.
- **`float`**: IEEE-754 double, special values (`inf`, `nan`), `float.is_integer()`, `as_integer_ratio()`, hex floats.
- **`complex`**: `real`/`imag`, `j` literals; deep math in `cmath` (Part 6).
- **`bool`**: A subclass of `int`; `True`/`False`; truthiness rules.
- **Numeric operations**: Arithmetic, `//` floor division, `%` modulo, `**` power, `divmod()`, mixed-type coercion.
- **Conversions & bases**: `int()`, `float()`, `complex()`, `bin()`, `oct()`, `hex()`, `round()`.
- **Precision tools**: `decimal` and `fractions` when float rounding is unacceptable (Part 6).

## 1.4 Strings & text

- **`str` fundamentals**: Immutability, Unicode code points, indexing, slicing, iteration, concatenation, `*` repetition.
- **Common methods**: Case (`upper`/`lower`/`casefold`/`title`), search (`find`/`index`/`startswith`), split/join, strip, replace, `partition`, `removeprefix`/`removesuffix`, `translate`/`maketrans`.
- **Testing methods**: `isalpha`, `isdigit`, `isnumeric`, `isspace`, `isidentifier`, etc.
- **Formatting: f-strings**: `f"{value!r:>10.2f}"`, conversions `!s`/`!r`/`!a`, format spec mini-language, `=` self-documenting, nested fields.
- **Formatting: `str.format` & `%`**: `{}`/`{0}`/`{name}` fields, `format()` builtin, the older `%`-style and when you still meet it.
- **The format spec mini-language**: Fill/align, sign, `#`, `0`, width, grouping `,`/`_`, precision, type codes.
- **Encoding/decoding**: `str.encode`/`bytes.decode`, codecs, errors handlers (`strict`/`ignore`/`replace`).
- **Template strings**: `string.Template` for $-substitution; `t""` template literals for safe interpolation.
- **[3.14]** `t""` template strings (PEP 750) capture static text plus interpolations as a `Template` object for safe HTML/SQL/shell building.

## 1.5 Sequences: list, tuple, range

- **`list`**: Mutable ordered sequence; methods (`append`, `extend`, `insert`, `pop`, `remove`, `sort`, `reverse`), copying, nesting.
- **`tuple`**: Immutable sequence, single-element `(x,)`, packing/unpacking, named tuples (Part 6).
- **`range`**: Lazy integer sequence, `range(start, stop, step)`, memory efficiency.
- **Common sequence operations**: Indexing, slicing `a[i:j:k]`, `+`, `*`, `in`, `len`, `min`/`max`/`sum`, `sorted`, `reversed`, `enumerate`, `zip`.
- **Slicing in depth**: Negative indices, step, slice assignment, deleting slices, `slice` objects.
- **Mutability pitfalls**: Aliasing, shallow vs deep copy, default-argument traps.

## 1.6 Sets & mappings

- **`set`**: Mutable unordered unique collection; add/discard/pop, set algebra (`|`, `&`, `-`, `^`), subset/superset.
- **`frozenset`**: Immutable, hashable set; usable as dict keys / set members.
- **`dict`**: Insertion-ordered mapping; CRUD, `get`/`setdefault`/`pop`/`update`, `keys`/`values`/`items` views.
- **Dict operations**: Membership, iteration, merge `|`/update `|=`, comprehensions, nested dicts.
- **Hashing & keys**: Hashability requirements, custom `__hash__`/`__eq__`, key ordering guarantees.
- **Specialised mappings**: `collections` (`defaultdict`, `Counter`, `OrderedDict`, `ChainMap`), `types.MappingProxyType` (Part 6).
- **[3.10]** Note: dict union operators `|`/`|=` arrived in 3.9 and are core vocabulary by 3.10+.

## 1.7 Binary data types

- **`bytes`**: Immutable byte sequence, literals `b""`, hex helpers, decoding to `str`.
- **`bytearray`**: Mutable byte buffer; in-place edits, growth.
- **`memoryview`**: Zero-copy views over buffer-protocol objects; slicing without copying.
- **The buffer protocol**: How objects expose memory to C-level consumers (PEP 688 exposed it to Python type checkers).
- **Binary tooling**: `struct`, `codecs`, `base64`, `binascii` for packing and encoding (Part 6).
- **[3.12]** The buffer protocol is now expressible in Python via `collections.abc.Buffer` / `__buffer__` (PEP 688).

## 1.8 Operators & expressions

- **Arithmetic & bitwise**: `+ - * / // % **`, `& | ^ ~ << >>`, operand types and coercion.
- **Comparisons**: `< <= > >= == !=`, chaining `0 < x < 10`, rich comparison semantics.
- **Boolean logic**: `and`, `or`, `not`, short-circuit evaluation, truthiness.
- **Identity & membership**: `is`/`is not`, `in`/`not in`.
- **Conditional expression**: `x if cond else y` (the ternary).
- **Power & unary**: `**` right-associativity, unary `+`/`-`/`~`.
- **Operator precedence & evaluation order**: The full precedence table; left-to-right evaluation; parenthesising for clarity.
- **The walrus `:=`**: Assignment expressions in comprehensions, `while`, and conditionals.

## 1.9 Control flow

- **`if` / `elif` / `else`**: Branching, truthiness, nesting, the conditional expression alternative.
- **`while`**: Condition loops, `break`, `continue`, the loop `else` clause.
- **`for`**: Iterating any iterable, unpacking in the target, `enumerate`/`zip`, the loop `else` clause.
- **`break` / `continue` / `pass`**: Loop control and the no-op statement.
- **`match` / `case`**: Structural pattern matching: literal, capture, wildcard `_`, sequence, mapping, class, OR `|`, guards `if`, `as` patterns; positional class patterns via `__match_args__`.
- **[3.10]** Structural pattern matching (`match`/`case`) introduced (PEP 634–636), plus much more precise SyntaxError/NameError/AttributeError messages with suggestions.

---

# PART 2: Functions, Iteration, Errors & Context Managers

Callables, the iterator/generator protocols, exceptions, and `with`.

The control-and-flow machinery that turns scripts into programs. Maps to Tutorial chapters 4 & 8 and Language Reference chapters 7–8.

## 2.1 Functions

- **Definition & call**: `def`, arguments, `return`, returning multiple values via tuples, the implicit `None`.
- **Parameters & arguments**: Positional, keyword, defaults, `*args`, `**kwargs`, positional-only `/`, keyword-only `*`, argument order rules.
- **Docstrings**: Conventions (PEP 257), `__doc__`, tools that read them (`help`, `pydoc`, `doctest`).
- **Annotations**: Parameter/return annotations, `__annotations__`, their relationship to typing (Part 4).
- **`lambda`**: Anonymous single-expression functions and where they fit.
- **Scope & namespaces**: LEGB rule, `global`, `nonlocal`, closures and late binding.
- **Higher-order functions**: Functions as values, `map`/`filter`, `functools` helpers, returning functions.
- **Decorators**: `@decorator`, wrapping with `functools.wraps`, parameterised decorators, stacking, class decorators.
- **Recursion**: Base/recursive cases, the recursion limit, `sys.setrecursionlimit`.
- **Partial application & dispatch**: `functools.partial`, `singledispatch`, `lru_cache`/`cache`.
- **Function introspection**: `__name__`/`__qualname__`, `__defaults__`/`__kwdefaults__`, `__closure__`, `__globals__`, `__code__`, `__wrapped__`; `inspect.signature`.
- **[3.14]** Annotations are no longer evaluated eagerly at definition time (PEP 649/749): they are computed lazily; introspect them via the new `annotationlib`. `from __future__ import annotations` still forces strings.

## 2.2 Comprehensions & generator expressions

- **List/set/dict comprehensions**: `[f(x) for x in it if cond]`, set and dict forms, conditional expressions inside.
- **Nested & multiple clauses**: Multiple `for`, multiple `if`, nested comprehensions, readability limits.
- **Generator expressions**: Lazy `(expr for x in it)`; memory efficiency; passing to `sum`/`any`/`all`.
- **The walrus in comprehensions**: Capturing intermediate results with `:=`.
- **Scoping**: Comprehension variables do not leak; performance characteristics.
- **[3.12]** Comprehensions are now inlined (PEP 709), making them meaningfully faster.

## 2.3 Iterators & generators

- **The iterator protocol**: `__iter__`/`__next__`, `iter()`/`next()`, `StopIteration`, the two-argument `iter()`.
- **Iterables vs iterators**: What `for` actually does; re-iterability.
- **Generator functions**: `yield`, lazy evaluation, statefulness, `return` value in `StopIteration`.
- **`yield from`**: Delegating to sub-generators / iterables.
- **Generator methods**: `send()`, `throw()`, `close()`; generators as lightweight coroutines.
- **Itertools mindset**: Composing pipelines with `itertools` (Part 6).
- **Async iteration (preview)**: `async for`, async generators: fully covered in Part 7.

## 2.4 Exceptions & error handling

- **`try` / `except` / `else` / `finally`**: Catching, ordering handlers, the `else` and `finally` clauses, cleanup guarantees.
- **`raise`**: Raising, re-raising, `raise ... from ...` explicit chaining, bare `raise`.
- **The exception hierarchy**: `BaseException` -> `Exception` -> concrete types; `KeyboardInterrupt`/`SystemExit`/`GeneratorExit` siblings.
- **Built-in exceptions**: `ValueError`, `TypeError`, `KeyError`, `IndexError`, `AttributeError`, `OSError` family, etc.
- **Custom exceptions**: Subclassing `Exception`, adding attributes, designing exception APIs.
- **Exception context**: Implicit chaining (`__context__`), explicit (`__cause__`), suppressing with `from None`.
- **Notes on exceptions**: `Exception.add_note()` to attach human-readable context.
- **Exception groups**: `ExceptionGroup`/`BaseExceptionGroup` and `except*` for handling several errors at once (esp. async).
- **Warnings**: The warning categories and the `warnings` module (Part 6).
- **`assert`**: Assertions, `-O` stripping, when (not) to use them.
- **[3.11]** Exception groups and `except*` (PEP 654); `Exception.add_note()` (PEP 678); fine-grained error locations in tracebacks point at the exact sub-expression (PEP 657).
- **[3.14]** `except`/`except*` may omit the parentheses around multiple exception types (PEP 758). Using `return`/`break`/`continue` to exit a `finally` block is now disallowed (PEP 765).

## 2.5 Context managers & the `with` statement

- **The `with` statement**: Deterministic setup/teardown; why it beats `try`/`finally` for resources.
- **The context-manager protocol**: `__enter__`/`__exit__`, swallowing exceptions, returning a bound value with `as`.
- **Multiple & parenthesized managers**: `with a() as x, b() as y:` and parenthesised multi-line groups.
- **`contextlib` toolkit**: `@contextmanager`, `closing`, `suppress`, `redirect_stdout`, `ExitStack`, `chdir` (Part 6).
- **Async context managers (preview)**: `async with`, `__aenter__`/`__aexit__`: see Part 7.
- **[3.10]** Parenthesized context managers became officially supported syntax (new PEG parser), allowing clean multi-line `with (...)` groups.

---

# PART 3: Object-Oriented Python & the Data Model

Classes, inheritance, dunder methods, and the protocols that make objects work.

How to design types and how Python's object system works underneath. Maps to Tutorial chapter 9 and Language Reference chapter 3 (Data model) and 8.7–8.11.

## 3.1 Classes & instances

- **Defining classes**: `class`, instantiation, the `self` parameter, instance vs class namespace.
- **`__init__` & `__new__`**: Initialisation vs allocation; when `__new__` matters (immutables, singletons).
- **Instance & class attributes**: Shared vs per-instance state; mutable class-attribute pitfalls.
- **Methods**: Instance methods, `@classmethod`, `@staticmethod`, bound vs unbound.
- **Encapsulation**: Public/`_protected`/`__private` conventions, name mangling.
- **Properties & descriptors**: `@property`, getters/setters/deleters; the descriptor protocol (`__get__`/`__set__`/`__delete__`/`__set_name__`).
- **`__slots__`**: Memory savings and attribute restriction; interactions with inheritance and `__dict__`.

## 3.2 Inheritance & composition

- **Single inheritance**: Extending classes, overriding, calling base behaviour with `super()`.
- **Multiple inheritance & MRO**: C3 linearisation, `__mro__`, cooperative `super()`, diamond problem.
- **`super()` in depth**: Zero-argument form, proxy objects, cooperative multiple inheritance.
- **`__init_subclass__`**: Customising subclass creation without a metaclass.
- **Mixins & composition**: Favouring composition; designing reusable mixins.
- **`isinstance`/`issubclass`**: Runtime type checks; virtual subclassing via ABCs.

## 3.3 The data model (special / "dunder" methods)

- **Object basics**: `__repr__`, `__str__`, `__format__`, `__bytes__`, `__hash__`, `__eq__`, `__bool__`.
- **Rich comparison**: `__lt__`/`__le__`/`__gt__`/`__ge__`, `functools.total_ordering`.
- **Attribute access**: `__getattr__`, `__getattribute__`, `__setattr__`, `__delattr__`, `__dir__`.
- **Container protocols**: `__len__`, `__getitem__`, `__setitem__`, `__delitem__`, `__contains__`, `__iter__`, `__reversed__`, `__missing__`.
- **Callable & numeric**: `__call__`; the full numeric/arithmetic dunders incl. reflected `__radd__` and in-place `__iadd__`.
- **Numeric conversion**: `__int__`, `__float__`, `__complex__`, `__index__` (lossless int for slicing/indexing), `__round__`/`__trunc__`/`__floor__`/`__ceil__`.
- **Type-check & creation hooks**: `__instancecheck__`/`__subclasscheck__`, `__class_getitem__` (subscripting types), `__mro_entries__`, `__match_args__`, disabling hashing with `__hash__ = None`.
- **Length & sizing**: `__len__`, `__length_hint__` for pre-sizing from iterators.
- **Context & async**: `__enter__`/`__exit__`, `__aenter__`/`__aexit__`, `__await__`, `__aiter__`/`__anext__`.
- **Object lifecycle**: `__del__`, weak references, resurrection caveats.
- **Copy & pickle hooks**: `__copy__`, `__deepcopy__`, `__reduce__`, `__getstate__`/`__setstate__`, `__replace__`.
- **The standard type hierarchy**: How built-in types fit together: None, numbers, sequences, mappings, callables, modules, classes.
- **[3.13]** `copy.replace()` and the `__replace__` protocol let you produce modified copies of immutable-style objects.

## 3.4 Metaclasses & class creation

- **`type` as the metaclass**: Classes are objects; `type(name, bases, ns)`; `metaclass=` keyword.
- **Custom metaclasses**: `__new__`/`__init__` on the metaclass, `__prepare__`, when they are justified.
- **`__set_name__` & class body**: Hooks that run during class creation; ordering.
- **Abstract base classes**: `abc.ABC`/`ABCMeta`, `@abstractmethod`, registering virtual subclasses, `collections.abc`.

## 3.5 Dataclasses & enumerations

- **`@dataclass`**: Auto-generated `__init__`/`__repr__`/`__eq__`; `field()`, defaults, `default_factory`.
- **Dataclass options**: `frozen`, `order`, `kw_only`, `slots`, `__post_init__`, inheritance.
- **`enum`**: `Enum`, `IntEnum`, `StrEnum`, `Flag`/`IntFlag`, `auto()`, members, aliases, `@unique`, functional API.
- **`namedtuple` & `typing.NamedTuple`**: Lightweight record types; defaults and methods.
- **[3.10]** `dataclasses` gained `slots=True` and `kw_only=True`.
- **[3.11]** `enum` added `StrEnum`, the `@verify` decorator, and reworked `Flag` boundaries / `__str__` behaviour.

## 3.6 Generics & type parameters (the OOP angle)

- **Generic classes**: Parameterising containers and protocols; the new `class C[T]:` syntax.
- **Type parameter lists**: `def f[T](...)`, bounds `[T: Bound]`, constraints, defaults, variance.
- **The `type` statement**: `type Alias[T] = ...` for generic, lazily-evaluated aliases.
- **Relationship to `typing`**: Full treatment, including `TypeVar`/`ParamSpec`/`TypeVarTuple`, in Part 4.
- **[3.12]** Native type-parameter syntax for classes, functions and aliases plus the `type` statement (PEP 695): no more explicit `TypeVar` for the common cases.
- **[3.13]** Type parameters can declare defaults (PEP 696).

---

# PART 4: Type Hints & Static Typing

Annotations, the `typing` module, and the static-analysis ecosystem.

Optional static typing: how to annotate code, the vocabulary of `typing`, and how checkers use it. Maps to the `typing` docs and the typing PEPs.

## 4.1 Annotation fundamentals

- **Where annotations go**: Variables, parameters, returns, attributes; `x: int = 0`.
- **`__annotations__`**: How annotations are stored and introspected on functions, classes and modules.
- **Deferred evaluation**: Lazy annotation evaluation and `from __future__ import annotations`; string vs object forms.
- **`annotationlib`**: The supported way to introspect annotations across evaluation modes.
- **Runtime vs static**: Annotations do not enforce types at runtime by themselves; checkers and validators (e.g. pydantic) do.
- **[3.14]** Annotations are evaluated lazily by default (PEP 649/749); introspect them with the new `annotationlib` module instead of touching `__annotations__` directly.

## 4.2 The `typing` vocabulary

- **Basics**: `Optional[X]`, `Union[X, Y]` / `X | Y`, `Any`, `object`, `None`.
- **Containers**: Built-in generics `list[int]`, `dict[str, int]`, `tuple[int, ...]`, `Sequence`, `Mapping`, `Iterable`, `Iterator`.
- **Callables**: `Callable[[int], str]`, `Concatenate`, `ParamSpec` for decorators.
- **Special forms**: `Literal`, `Final`, `ClassVar`, `Annotated`, `TypeAlias` / the `type` statement, `Never`/`NoReturn`.
- **`TypedDict`**: Typed dictionaries; `Required`/`NotRequired`, `ReadOnly`, total/partial, `**kwargs` typing.
- **Protocols**: `Protocol` structural typing, `@runtime_checkable`.
- **Type variables**: `TypeVar` (bounds/constraints/variance/defaults), `ParamSpec`, `TypeVarTuple` + `Unpack`.
- **Narrowing helpers**: `TypeGuard`, `TypeIs`, `assert_type`, `assert_never`, `cast`, `reveal_type`.
- **Decorators & markers**: `@overload`, `@final`, `@override`, `@deprecated`, `@no_type_check`.
- **Self & string types**: `Self`, `LiteralString`.
- **Named/typed records**: `NamedTuple`, `NewType`.
- **[3.10]** `X | Y` union syntax (PEP 604), `ParamSpec` (612), `TypeAlias` (613), `TypeGuard` (647).
- **[3.11]** `Self` (673), variadic generics `TypeVarTuple` (646), `Required`/`NotRequired` (655), `LiteralString` (675), `assert_type`/`reveal_type`.
- **[3.12]** `@override` (698), `TypedDict` for `**kwargs` (692), `type` statement & generic syntax (695).
- **[3.13]** `TypeIs` (742), `ReadOnly` TypedDict items (705), `@deprecated` (702), type-parameter defaults (696).

## 4.3 Typing in practice

- **Gradual typing**: Annotate incrementally; `Any` as an escape hatch; partial coverage.
- **Static type checkers**: `mypy`, `pyright`/Pylance, `pyre`, `pytype`: third-party tools that read your hints.
- **Stub files**: `.pyi` stubs, `typeshed`, shipping types with `py.typed`.
- **Runtime validation**: `dataclasses` + checkers vs runtime validators like `pydantic` (third-party).
- **Common patterns**: Overloads for polymorphic APIs, generics for containers, protocols for duck typing.
- **Official guidance**: The "Static Typing with Python" guide and the typing specification.

---

# PART 5: Modules, Packages & the Import System

Code organisation and the machinery behind `import`.

Structuring code across files and the full import machinery. Maps to Tutorial chapter 6 and Language Reference chapter 5 (The import system).

## 5.1 Modules

- **What a module is**: A `.py` file as a namespace; module-level code runs once on first import.
- **`import` forms**: `import m`, `import m as n`, `from m import x`, `from m import x as y`, `from m import *` and `__all__`.
- **Module attributes**: `__name__`, `__file__`, `__doc__`, `__dict__`, `__all__`.
- **The `__main__` idiom**: `if __name__ == "__main__":`, script vs import behaviour.
- **Module caching**: `sys.modules`, reloading with `importlib.reload`, circular-import hazards.
- **Bytecode caching**: `__pycache__`, `.pyc` files, `compileall`, `PYTHONDONTWRITEBYTECODE`.

## 5.2 Packages

- **Regular packages**: `__init__.py`, the package namespace, sub-packages.
- **Namespace packages**: Implicit packages spread across directories (PEP 420).
- **Relative vs absolute imports**: `from . import x`, `from ..pkg import y`, when relative imports are allowed.
- **Executable packages**: `__main__.py`, `python -m package`, zipapps.
- **Package data & resources**: Reading bundled files with `importlib.resources`.

## 5.3 The import system internals

- **Import protocol**: Finders and loaders, meta path, the path-based finder, path entry finders.
- **`sys.path`**: Search-path construction, `sys.path` initialisation, `site` customisation, `.pth` files.
- **Loading**: Module specs (`ModuleSpec`), `__spec__`, loaders, executing module code.
- **Customising imports**: Writing import hooks, replacing the import system, `importlib.util` helpers.
- **Packaging metadata**: `importlib.metadata` for entry points, versions, distributions.
- **Related modules**: `importlib`, `importlib.resources`, `importlib.resources.abc`, `zipimport`, `pkgutil`, `modulefinder`, `runpy` (Part 6).

---

# PART 6: The Standard Library: Complete Module Reference

Every module shipped with CPython 3.14, grouped by the official categories.

Python's "batteries included" library. Every module below ships with CPython 3.14; the grouping and order match the official Standard Library table of contents, so nothing is skipped. Use this as a catalogue: skim to discover, then open the matching docs page for full APIs. Modules new since 3.10 carry a version badge in their group.

## 6.1 Built-in functions, constants, types & exceptions

**Built-in functions (always available, no import)**

The ~70 builtins: `print`, `input`, `len`, `range`, `enumerate`, `zip`, `map`, `filter`, `sorted`, `reversed`, `sum`, `min`, `max`, `abs`, `round`, `pow`, `divmod`, `iter`, `next`, `open`, `type`, `isinstance`, `issubclass`, `getattr`, `setattr`, `hasattr`, `delattr`, `dir`, `vars`, `id`, `hash`, `repr`, `ascii`, `format`, `bin`/`oct`/`hex`, `int`/`float`/`complex`/`bool`/`str`/`bytes`/`bytearray`/`list`/`tuple`/`dict`/`set`/`frozenset`, `object`, `super`, `property`, `staticmethod`/`classmethod`, `callable`, `eval`/`exec`/`compile`, `globals`/`locals`, `__import__`, `memoryview`, `slice`, `any`/`all`, `breakpoint`, `help`, `aiter`/`anext`. (Full list in Appendix A.)

**Built-in constants**

- `True` / `False` / `None`: The core singletons.
- `NotImplemented` / `Ellipsis` (`...`): Operator-fallback sentinel and the ellipsis literal.
- `__debug__`: Reflects whether assertions are active (`-O`).
- `site` constants: `quit`, `exit`, `copyright`, `credits`, `license` added by the `site` module.

**Built-in types**

- **Truth-value testing**: What counts as true/false across types.
- **Numeric types**: `int`, `float`, `complex`, `bool`; operations and limits.
- **Iterator types**: The iterator/generator protocol surface.
- **Sequence types**: `list`, `tuple`, `range`; the shared sequence operations.
- **Text & binary sequences**: `str`, `bytes`, `bytearray`, `memoryview`; method summaries.
- **Set types**: `set`, `frozenset`.
- **Mapping types**: `dict` and its view objects.
- **Context-manager types**: Objects supporting `with`.
- **Type-annotation types**: `GenericAlias`, `Union`, special attributes.
- **Other built-in types**: modules, classes/instances, functions, methods, code, frame, `None`/`NotImplemented` types, etc.
- **Integer string-conversion limit**: The safety cap on `int`<->`str` conversion length.

**Built-in exceptions**

- **Base classes**: `BaseException`, `Exception`, `ArithmeticError`, `LookupError`, `OSError`.
- **Concrete exceptions**: `ValueError`, `TypeError`, `KeyError`, `IndexError`, `AttributeError`, `RuntimeError`, `StopIteration`, etc.
- **Warnings**: `Warning` and its subclasses.
- **Exception groups**: `ExceptionGroup` / `BaseExceptionGroup`; the `except*` partner.
- **Exception context**: Chaining and the full exception hierarchy.

**Thread Safety Guarantees**

- **Thread-safety levels**: What the language guarantees for built-in containers.
- **Per-type guarantees**: Documented behaviour for `list`, `dict`, `set`, `bytearray`, `memoryview` objects.
- **[3.14]** A dedicated "Thread Safety Guarantees" chapter was added, important for the free-threaded build.

## 6.2 Text Processing Services

- `string`: Constants (`ascii_letters`, `digits`, ...), `Template`, `Formatter`, helpers.
- `string.templatelib`: Support for `t""` template-string literals: `Template`, `Interpolation`.
- `re`: Regular expressions: patterns, flags, groups, `match`/`search`/`findall`/`finditer`/`sub`/`split`, compiled patterns, lookaround, named groups.
- `difflib`: Sequence diffing: `SequenceMatcher`, `unified_diff`, `HtmlDiff`, `get_close_matches`.
- `textwrap`: Wrap/fill/shorten/indent/dedent text.
- `unicodedata`: Unicode character database: names, categories, normalisation (`NFC`/`NFD`/`NFKC`/`NFKD`).
- `stringprep`: RFC 3454 string preparation tables.
- `readline`: GNU readline interface: history, completion, key bindings.
- `rlcompleter`: Tab-completion for the interactive interpreter.
- **[3.14]** `string.templatelib` is new, backing PEP 750 template strings.

## 6.3 Binary Data Services

- `struct`: Pack/unpack C structs to/from `bytes`; format strings, byte order, alignment, `Struct` objects.
- `codecs`: Codec registry, encoders/decoders, incremental codecs, stream readers/writers, BOM constants.

## 6.4 Data Types

- `datetime`: `date`, `time`, `datetime`, `timedelta`, `tzinfo`/`timezone`; parsing/formatting (`strftime`/`strptime`/`fromisoformat`), arithmetic, aware vs naive.
- `zoneinfo`: IANA time-zone support backing `datetime`; `ZoneInfo`, key lookup, `tzdata`.
- `calendar`: Calendar maths and text/HTML calendars; CLI.
- `collections`: `namedtuple`, `deque`, `Counter`, `OrderedDict`, `defaultdict`, `ChainMap`, `UserDict`/`UserList`/`UserString`.
- `collections.abc`: Abstract base classes: `Iterable`, `Iterator`, `Sequence`, `Mapping`, `Set`, `Callable`, `Hashable`, `Buffer`, ...
- `heapq`: Binary-heap priority queue: `heappush`/`heappop`/`heapify`, `nlargest`/`nsmallest`, `merge`.
- `bisect`: Binary search / sorted-list insertion: `bisect_left`/`bisect_right`, `insort`.
- `array`: Compact typed numeric arrays.
- `weakref`: Weak references, `WeakValueDictionary`/`WeakKeyDictionary`/`WeakSet`, finalizers, proxies.
- `types`: Dynamic type creation and names: `SimpleNamespace`, `MappingProxyType`, `ModuleType`, function/method types, `new_class`.
- `copy`: `copy()` shallow, `deepcopy()`, `copy.replace()`, the copy hooks.
- `pprint`: Pretty-print nested data structures.
- `reprlib`: Length-limited `repr` for large/recursive objects.
- `enum`: `Enum`, `IntEnum`, `StrEnum`, `Flag`, `IntFlag`, `auto`, `@unique`, `@verify`.
- `graphlib`: Topological sorting via `TopologicalSorter`.
- **[3.13]** `copy.replace()` added for producing modified copies.

## 6.5 Numeric & Mathematical Modules

- `numbers`: The numeric tower of abstract base classes (`Number`, `Complex`, `Real`, `Rational`, `Integral`).
- `math`: Real-valued math: trig, log/exp, `gcd`/`lcm`, `isqrt`, `comb`/`perm`, `prod`, `fsum`, `nan`/`inf`, `dist`/`hypot`.
- `cmath`: Complex-number math functions and constants.
- `decimal`: Correctly-rounded decimal floating point; `Context`, precision, rounding modes, signals.
- `fractions`: Exact rational arithmetic with `Fraction`.
- `random`: PRNGs: `random`/`randint`/`randrange`/`choice`/`choices`/`sample`/`shuffle`, distributions, `SystemRandom`, seeding, CLI.
- `statistics`: `mean`/`median`/`mode`, variance/stdev, `quantiles`, `correlation`/`covariance`/`linear_regression`, `NormalDist`.
- **[3.13]** `random` gained a command-line interface.

## 6.6 Functional Programming Modules

- `itertools`: Iterator building blocks: `count`/`cycle`/`repeat`, `chain`, `islice`, `tee`, `product`/`permutations`/`combinations`, `groupby`, `accumulate`, `pairwise`, `batched`.
- `functools`: `reduce`, `partial`, `lru_cache`/`cache`, `cached_property`, `singledispatch`/`singledispatchmethod`, `wraps`, `total_ordering`, `cmp_to_key`.
- `operator`: Functional versions of operators: `add`/`mul`/..., `itemgetter`, `attrgetter`, `methodcaller`.
- **[3.10]** `itertools.pairwise` added.
- **[3.12]** `itertools.batched` added for fixed-size chunking.

## 6.7 File & Directory Access

- `pathlib`: Object-oriented paths: `Path`/`PurePath`, joining with `/`, globbing, read/write helpers, `stat`, `resolve`.
- `os.path`: Classic path string ops: `join`, `split`, `exists`, `isfile`/`isdir`, `abspath`, `splitext`, `expanduser`.
- `stat`: Interpreting `os.stat()` results; mode bit constants and helpers.
- `filecmp`: Compare files and directory trees.
- `tempfile`: Temporary files/dirs: `TemporaryFile`, `NamedTemporaryFile`, `TemporaryDirectory`, `mkstemp`/`mkdtemp`.
- `glob`: Shell-style pathname expansion, recursive `**`.
- `fnmatch`: Unix filename pattern matching.
- `linecache`: Random access to lines of text files (used by tracebacks).
- `shutil`: High-level file ops: `copy`/`copytree`/`move`/`rmtree`, `make_archive`/`unpack_archive`, `which`, `disk_usage`.

## 6.8 Data Persistence

- `pickle`: Native object serialisation; protocols, `__reduce__`, security caveats, `pickletools`.
- `copyreg`: Register reduction functions used by `pickle`/`copy`.
- `shelve`: Dict-like persistent storage backed by `dbm` + `pickle`.
- `marshal`: Internal serialisation (used for `.pyc`); not for general use.
- `dbm`: Simple key-value databases: `dbm.sqlite3`, `dbm.gnu`, `dbm.ndbm`, `dbm.dumb`.
- `sqlite3`: Embedded SQL database (DB-API 2.0): connections, cursors, parameters, transactions, adapters/converters, `Row`, blobs.
- **[3.13]** `dbm.sqlite3` is now the default `dbm` backend.

## 6.9 Data Compression & Archiving

- `compression` **(package)**: The new namespace gathering compression modules.
- `compression.zstd`: Zstandard compression/decompression (PEP 784).
- `zlib`: gzip-compatible deflate compression.
- `gzip`: Read/write `.gz` files; `GzipFile`, CLI.
- `bz2`: bzip2 compression; `BZ2File`.
- `lzma`: XZ/LZMA compression; `LZMAFile`.
- `zipfile`: Create/read ZIP archives; `ZipFile`, `Path`, `ZipInfo`, AES-less encryption read.
- `tarfile`: Read/write tar archives; extraction filters for safety.
- **[3.14]** New `compression` package and `compression.zstd` module add Zstandard support.

## 6.10 File Formats

- `csv`: Read/write CSV/TSV: `reader`/`writer`, `DictReader`/`DictWriter`, dialects, `Sniffer`.
- `configparser`: INI-style configuration files; interpolation, sections, defaults.
- `tomllib`: Read-only TOML parser (`load`/`loads`).
- `netrc`: Parse `.netrc` credential files.
- `plistlib`: Read/write Apple `.plist` property lists.
- **[3.11]** `tomllib` added to the stdlib (read-only TOML, PEP 680).

## 6.11 Cryptographic Services

- `hashlib`: Secure hashes: SHA-2/3, BLAKE2, `pbkdf2_hmac`, `scrypt`, `file_digest`.
- `hmac`: Keyed-hash message authentication; `compare_digest` for constant-time comparison.
- `secrets`: Cryptographically strong randomness for tokens/passwords: `token_hex`, `token_urlsafe`, `choice`.
- **[3.14]** `hmac` ships a built-in implementation using formally-verified HACL* code.

## 6.12 Generic Operating System Services

- `os`: OS interface: environment, processes, files/descriptors, paths, `os.walk`, `os.scandir`, permissions, signals on Unix.
- `io`: Stream framework: `TextIOWrapper`, `BytesIO`/`StringIO`, buffering, the `open()` machinery.
- `time`: Clocks and conversions: `time`/`perf_counter`/`monotonic`/`process_time`, `sleep`, `strftime`/`strptime`, `struct_time`.
- `logging`: The logging framework: loggers, handlers, formatters, levels, `basicConfig`, propagation.
- `logging.config`: Configure logging from dicts/files.
- `logging.handlers`: Rotating/file/socket/SMTP/syslog and other handlers.
- `platform`: Identify OS, machine, Python build, versions.
- `errno`: Standard system error numbers and `errorcode`.
- `ctypes`: Call C libraries from Python: load DLL/.so, C types, structures, callbacks, calling conventions.

## 6.13 Command-line interface libraries

- `argparse`: Full-featured argument parser: positional/optional args, subcommands, types, help, groups.
- `optparse`: Older option parser (superseded by `argparse`).
- `getpass`: Prompt for passwords without echo; get the login name.
- `fileinput`: Iterate lines across multiple files / stdin with in-place editing.
- `curses`: Terminal handling for character-cell displays.
- `curses.textpad`: Editable text-box widget for curses.
- `curses.ascii`: ASCII character classification utilities.
- `curses.panel`: Stacked-window panel extension for curses.
- `cmd`: Framework for line-oriented command interpreters (REPL-style tools).
- **[3.14]** `argparse` (and `json`/`unittest`/`calendar`) CLIs gained colour output.

## 6.14 Concurrent Execution

Listed here as reference; the conceptual deep dive (GIL, free threading, async, subinterpreters) is Part 7.

- `threading`: Threads, `Lock`/`RLock`/`Semaphore`/`Event`/`Condition`/`Barrier`, `local`, daemon threads.
- `multiprocessing`: Process-based parallelism: `Process`, `Pool`, `Queue`/`Pipe`, managers, start methods.
- `multiprocessing.shared_memory`: Shared-memory blocks across processes; `ShareableList`.
- `concurrent` **(package)**: Namespace for high-level execution helpers.
- `concurrent.futures`: `ThreadPoolExecutor`, `ProcessPoolExecutor`, `InterpreterPoolExecutor`, `Future`, `as_completed`, `map`.
- `concurrent.interpreters`: Multiple interpreters (subinterpreters) in one process (PEP 734).
- `subprocess`: Run external commands: `run`, `Popen`, pipes, `check_output`, timeouts, shell vs argv.
- `sched`: General-purpose event scheduler.
- `queue`: Thread-safe queues: `Queue`, `LifoQueue`, `PriorityQueue`, `SimpleQueue`.
- `contextvars`: Context-local state (works with `asyncio`): `ContextVar`, `Context`, `copy_context`.
- `_thread`: Low-level threading primitives underlying `threading`.
- **[3.14]** `concurrent.interpreters` exposes subinterpreters; `InterpreterPoolExecutor` added; on non-macOS Unix `ProcessPoolExecutor` now defaults to the `forkserver` start method.

## 6.15 Networking & Interprocess Communication

- `asyncio`: Async I/O framework (full treatment in Part 7): event loop, coroutines, tasks, streams, sync primitives, subprocesses.
- `socket`: Low-level BSD sockets: TCP/UDP, addresses, options, blocking/non-blocking, `socketpair`.
- `ssl`: TLS/SSL wrapper for sockets: `SSLContext`, certificate verification, SNI, ALPN.
- `select`: Low-level I/O readiness: `select`, `poll`, `epoll`, `kqueue`.
- `selectors`: High-level I/O multiplexing built on `select`.
- `signal`: Set handlers for asynchronous signals; alarms; `SIGINT` etc.
- `mmap`: Memory-mapped files / shared memory regions.

## 6.16 Internet Data Handling

- `email`: Email/MIME package: `EmailMessage`, parsing/generating, headers, policies, attachments.
- `json`: JSON encode/decode: `dump`/`dumps`/`load`/`loads`, custom encoders/decoders, `object_hook`, CLI.
- `mailbox`: Read/write mailbox formats (mbox, Maildir, ...).
- `mimetypes`: Map filenames to MIME types and back.
- `base64`: Base16/32/64/85 encodings.
- `binascii`: Convert between binary and ASCII (hex, base64 primitives, CRCs).
- `quopri`: Encode/decode MIME quoted-printable.
- **[3.14]** `json` CLI gained colour output.

## 6.17 Structured Markup Processing Tools

- `html`: HTML helpers: `escape`/`unescape`.
- `html.parser`: Event-driven `HTMLParser` for HTML/XHTML.
- `html.entities`: HTML named-entity tables.
- `xml` **(package)**: Overview of XML modules and security warnings (XML attacks).
- `xml.etree.ElementTree`: The pragmatic XML API: parse, build, `find`/`findall`, XPath subset, `iterparse`.
- `xml.dom`: Document Object Model interfaces and constants.
- `xml.dom.minidom`: Lightweight DOM implementation.
- `xml.dom.pulldom`: Build partial DOM trees from SAX events.
- `xml.sax`: Event-driven SAX2 parsing.
- `xml.sax.handler`: Base classes for SAX content/error handlers.
- `xml.sax.saxutils`: SAX helper classes and escaping utilities.
- `xml.sax.xmlreader`: Interface for SAX XML readers.
- `xml.parsers.expat`: Fast non-validating XML parsing via Expat.

## 6.18 Internet Protocols & Support

- `webbrowser`: Open URLs in the user's browser.
- `wsgiref`: Reference WSGI implementation and utilities; a simple server.
- `urllib` **(package)**: URL-handling umbrella package.
- `urllib.request`: Open and read URLs: openers, handlers, proxies, auth, headers.
- `urllib.response`: Response objects returned by `urllib.request`.
- `urllib.parse`: Parse/recombine URLs, query strings (`urlencode`/`parse_qs`), quoting.
- `urllib.error`: `URLError`/`HTTPError` exception classes.
- `urllib.robotparser`: Parse `robots.txt` rules.
- `http` **(package)**: HTTP status codes (`HTTPStatus`) and methods (`HTTPMethod`).
- `http.client`: Low-level HTTP/HTTPS client (`HTTPConnection`).
- `ftplib`: FTP client (`FTP`/`FTP_TLS`).
- `poplib`: POP3 client.
- `imaplib`: IMAP4 client.
- `smtplib`: SMTP client for sending mail.
- `uuid`: UUID generation/parsing: versions 1–8, `uuid4` random, namespace UUIDs.
- `socketserver`: Framework for TCP/UDP servers; threading/forking mix-ins.
- `http.server`: Simple HTTP servers and request handlers (incl. CGI-free static serving).
- `http.cookies`: Server-side cookie management.
- `http.cookiejar`: Client-side cookie storage/policy.
- `xmlrpc` **(package)**: XML-RPC client/server umbrella.
- `xmlrpc.client`: XML-RPC client access.
- `xmlrpc.server`: Basic XML-RPC servers.
- `ipaddress`: IPv4/IPv6 address, network and interface objects.
- **[3.14]** `uuid` now supports versions 6–8 and generates versions 3–5 up to ~40% faster.

## 6.19 Multimedia Services

- `wave`: Read/write WAV audio files.
- `colorsys`: Convert between RGB/YIQ/HLS/HSV colour systems.

Note: many legacy multimedia modules (`aifc`, `audioop`, `chunk`, `imghdr`, `sndhdr`, `sunau`, `ossaudiodev`) were removed in 3.13: see section 6.32.

## 6.20 Internationalization

- `gettext`: Message catalogues and translation (`_()`, plural forms).
- `locale`: Locale-aware formatting of numbers, currency, dates; encodings.

## 6.21 Graphical User Interfaces with Tk

- `tkinter`: Python interface to Tcl/Tk: widgets, geometry managers (pack/grid/place), events, variables.
- `tkinter.colorchooser`: Colour-picker dialog.
- `tkinter.font`: Font objects and helpers.
- **Tkinter dialogs**: Common dialog modules (`filedialog`, `simpledialog`, `commondialog`).
- `tkinter.messagebox`: Standard message/confirmation prompts.
- `tkinter.scrolledtext`: Text widget with built-in scrollbar.
- `tkinter.dnd`: Experimental drag-and-drop support.
- `tkinter.ttk`: Themed Tk widgets (modern look, `Treeview`, `Notebook`, styles).
- **IDLE**: The bundled editor/shell (itself written in tkinter).
- `turtle`: Turtle graphics for learning/visualisation; `turtledemo`.

## 6.22 Development Tools

- `typing`: The static-typing support module (full vocabulary in Part 4).
- `pydoc`: Generate docs and the interactive `help()` system; `pydoc -b` browser.
- **Python Development Mode**: `-X dev` / `PYTHONDEVMODE`: extra checks and warnings for catching bugs early.
- `doctest`: Run examples embedded in docstrings as tests.
- `unittest`: xUnit testing framework: `TestCase`, assertions, fixtures, discovery, runners, skips.
- `unittest.mock`: Mocking: `Mock`/`MagicMock`, `patch`, `autospec`, call assertions, `mock_open`.
- `unittest.mock` **: getting started**: The worked tutorial for mock usage.
- `test`: CPython's own regression-test package.
- `test.support`: Utilities used by the test suite (semi-public).
- `test.support.socket_helper`: Socket-test helpers.
- `test.support.script_helper`: Helpers for spawning Python in tests.
- `test.support.bytecode_helper`: Helpers for asserting on generated bytecode.
- `test.support.threading_helper`: Threading-test helpers.
- `test.support.os_helper`: OS/filesystem test helpers.
- `test.support.import_helper`: Import-machinery test helpers.
- `test.support.warnings_helper`: Warning-related test helpers.

## 6.23 Debugging & Profiling

- **Audit events table**: The reference list of runtime audit hooks (`sys.audit`).
- `bdb`: Debugger framework underpinning `pdb`.
- `faulthandler`: Dump Python tracebacks on faults/timeouts/signals.
- `pdb`: The interactive debugger: breakpoints, stepping, `breakpoint()`, post-mortem, remote attach.
- **The Python Profilers**: `profile` and `cProfile` deterministic profilers + `pstats`.
- `timeit`: Micro-benchmark small snippets; CLI and API.
- `trace`: Trace statement execution / coverage.
- `tracemalloc`: Trace memory allocations and find leaks.
- **[3.14]** A zero-overhead external debugger interface (PEP 768) lets tools attach to a running process; `pdb` can use it.

## 6.24 Software Packaging & Distribution

- `ensurepip`: Bootstrap `pip` into an environment.
- `venv`: Create virtual environments (API + CLI).
- `zipapp`: Build executable `.pyz` zip applications.

End-to-end packaging (`pyproject.toml`, building wheels, uploading) is Part 9; `distutils` was removed in 3.12 (see 6.32).

## 6.25 Python Runtime Services

- `sys`: Interpreter hooks: `argv`, `path`, `modules`, `stdin`/`stdout`/`stderr`, `exc_info`, `setrecursionlimit`, `getsizeof`, `flags`, `version_info`, hooks.
- `sys.monitoring`: Low-overhead execution-event monitoring API for tools (PEP 669).
- `sysconfig`: Access build/install configuration paths and variables.
- `builtins`: The module holding all built-in names.
- `__main__`: The top-level script environment.
- `warnings`: Issue and filter warnings; categories; `simplefilter`/`filterwarnings`; `catch_warnings`.
- `dataclasses`: `@dataclass`, `field`, `asdict`/`astuple`, `replace`, `make_dataclass`.
- `contextlib`: `@contextmanager`, `closing`, `suppress`, `redirect_stdout`/`stderr`, `ExitStack`/`AsyncExitStack`, `nullcontext`, `chdir`.
- `abc`: Abstract base classes: `ABC`/`ABCMeta`, `@abstractmethod`, registration.
- `atexit`: Register functions to run at interpreter exit.
- `traceback`: Format/print exceptions and stacks; `TracebackException`.
- `__future__`: Opt into upcoming language behaviour (e.g. `annotations`).
- `gc`: Control the cyclic garbage collector: `collect`, thresholds, `freeze`, debugging.
- `inspect`: Introspect live objects: signatures, source, members, stack frames, `getmembers`.
- `annotationlib`: Introspect annotations across eager/lazy/string evaluation modes.
- `site`: Site-specific initialisation, `.pth` files, `sys.path` extension, user site.
- **[3.11]** `contextlib.chdir` added.
- **[3.12]** `sys.monitoring` added for efficient debuggers/profilers (PEP 669); per-interpreter GIL groundwork (PEP 684).
- **[3.14]** `annotationlib` added for annotation introspection (PEP 649/749).

## 6.26 Custom Python Interpreters

- `code`: Build interactive interpreters / REPLs (`InteractiveConsole`).
- `codeop`: Compile possibly-incomplete Python source (REPL support).

## 6.27 Importing Modules

- `zipimport`: Import modules directly from ZIP archives.
- `pkgutil`: Package utilities: iterate sub-modules, namespace-package support.
- `modulefinder`: Determine the modules a script imports.
- `runpy`: Locate and run modules/paths as `__main__` (`-m` machinery).
- `importlib`: Programmatic import: `import_module`, `reload`, `util`, finders/loaders, `abc`.
- `importlib.resources`: Read package data files in a portable way.
- `importlib.resources.abc`: Abstract base classes for resource readers.
- `importlib.metadata`: Read installed-distribution metadata, versions, entry points.
- `sys.path` **initialisation**: How the module search path is built at startup.

## 6.28 Python Language Services

- `ast`: Abstract syntax trees: `parse`, `NodeVisitor`/`NodeTransformer`, `unparse`, `literal_eval`.
- `symtable`: Access the compiler's symbol tables.
- `token`: Token-type constants for the tokenizer/parser.
- `keyword`: Test for keywords and soft keywords.
- `tokenize`: Tokenise Python source into a token stream.
- `tabnanny`: Detect ambiguous tab/space indentation.
- `pyclbr`: Module class/function browser support.
- `py_compile`: Compile a single source file to bytecode.
- `compileall`: Byte-compile whole directory trees.
- `dis`: Disassemble bytecode; instruction set, `Bytecode`, adaptive/specialised instructions.
- `pickletools`: Analyse/optimise pickle streams.

## 6.29 MS Windows Specific Services

- `msvcrt`: Useful routines from the MS VC++ runtime (console/file locking).
- `winreg`: Access the Windows registry.
- `winsound`: Play sounds on Windows.

## 6.30 Unix-specific Services

- `shlex`: Shell-style lexical analysis / safe command splitting (`shlex.split`/`quote`).
- `posix`: Direct POSIX system calls (use `os` instead).
- `pwd`: The Unix password database.
- `grp`: The Unix group database.
- `termios`: POSIX tty control.
- `tty`: Terminal mode helpers (raw/cbreak).
- `pty`: Pseudo-terminal utilities.
- `fcntl`: `fcntl`/`ioctl` system calls; file locking.
- `resource`: Query/set process resource limits and usage.
- `syslog`: Unix syslog interface.

## 6.31 Superseded Modules

- `getopt`: C-style command-line parsing (prefer `argparse`).
- `optparse`: Older option parser, also superseded by `argparse` (listed in 6.13).

## 6.32 Removed Modules (know what is gone)

Several long-deprecated modules have been deleted. They appear here so you recognise them in old code and know the modern replacement.

- **PEP 594 "dead batteries"**: Removed in 3.13: `aifc`, `audioop`, `cgi`, `cgitb`, `chunk`, `crypt`, `imghdr`, `mailcap`, `msilib`, `nis`, `nntplib`, `ossaudiodev`, `pipes`, `sndhdr`, `spwd`, `sunau`, `telnetlib`, `uu`, `xdrlib`.
- `distutils`: Removed in 3.12: use `setuptools` / modern build backends and `pyproject.toml`.
- `lib2to3` / `2to3`: Removed; the Python-2 migration tooling is no longer shipped.
- **[3.12]** `distutils` removed from the standard library.
- **[3.13]** The PEP 594 batch of 19 legacy modules removed.

## 6.33 Security Considerations

- **Security-sensitive modules**: Guidance on `pickle`, `marshal`, `subprocess`, `os.system`, XML parsers, `tempfile`, `ssl` defaults.
- **`-I` isolated mode & audit hooks**: Reducing attack surface; `sys.addaudithook` and the audit-events table.
- **Input handling**: Avoiding injection, validating untrusted data, safe deserialisation.

---

# PART 7: Concurrency, Parallelism & Asynchronous Programming

Threads, processes, async/await, subinterpreters, and life with(out) the GIL.

Doing many things at once. This part turns the modules from 6.14–6.15 into a mental model: when to use threads vs processes vs async, and what the recent free-threading and subinterpreter work changes.

## 7.1 The execution model: GIL & free threading

- **The Global Interpreter Lock**: What it protects, why it limits CPU-bound threading, why it never blocked I/O concurrency.
- **Free-threaded CPython**: The `--disable-gil` build (`python3.xt`); true multi-core threading; ecosystem/C-extension caveats.
- **Thread-safety guarantees**: What the language promises for built-in containers under free threading (see 6.1).
- **Per-interpreter GIL**: Each subinterpreter can own its own GIL, enabling isolation-based parallelism.
- **Choosing a model**: I/O-bound -> threads or async; CPU-bound -> processes, free threading, or subinterpreters.
- **[3.12]** Per-interpreter GIL groundwork (PEP 684).
- **[3.13]** Experimental free-threaded build (PEP 703) and the experimental JIT (PEP 744) ship.
- **[3.14]** Free-threaded Python is officially supported (PEP 779); the single-thread penalty dropped to roughly 5–10% and the adaptive interpreter is enabled in that build.

## 7.2 Threading

- **Creating threads**: `Thread`, `start`/`join`, daemon threads, naming.
- **Synchronisation**: `Lock`, `RLock`, `Semaphore`, `Event`, `Condition`, `Barrier`; deadlocks.
- **Thread-local data**: `threading.local`, and `contextvars` for context propagation.
- **Coordination patterns**: Producer/consumer with `queue`, thread pools via `concurrent.futures`.

## 7.3 Multiprocessing & process pools

- **Processes**: `Process`, start methods (`spawn`/`fork`/`forkserver`), picklability of arguments.
- **IPC**: `Queue`, `Pipe`, `Manager` proxies, `Value`/`Array`, `shared_memory`.
- **Pools**: `multiprocessing.Pool` vs `ProcessPoolExecutor`; chunking, `map`/`imap`.
- **Pitfalls**: Fork-safety, the `if __name__ == "__main__"` guard on Windows/spawn.
- **[3.14]** On Unix (except macOS) the default start method for `ProcessPoolExecutor` is now `forkserver`.

## 7.4 Subinterpreters

- `concurrent.interpreters`: Create isolated interpreters in one process (PEP 734); send/receive data through channels/queues.
- `InterpreterPoolExecutor`: A `concurrent.futures` executor backed by a pool of subinterpreters.
- **When to reach for it**: CPU parallelism with stronger isolation than threads and lower overhead than processes.
- **[3.14]** Subinterpreters exposed to Python and `InterpreterPoolExecutor` added.

## 7.5 Asynchronous programming with `asyncio`

- **`async` / `await`**: Coroutine functions, awaitables, the event-loop model.
- **Running async code**: `asyncio.run`, the event loop, `get_running_loop`, debugging mode.
- **Tasks & futures**: `create_task`, `gather`, `wait`, `as_completed`, cancellation, `shield`.
- **Task groups & timeouts**: `asyncio.TaskGroup` for structured concurrency; `asyncio.timeout`.
- **Synchronisation**: Async `Lock`/`Event`/`Condition`/`Semaphore`, `Queue`.
- **Streams & networking**: `open_connection`, `start_server`, protocols/transports, async subprocesses.
- **Async iteration & context**: `async for`, async generators, `async with`, `contextlib.aclosing`/`AsyncExitStack`.
- **Introspection**: Inspect running tasks; the new CLI to inspect async state of a live process.
- **`contextvars` with async**: Propagating context across `await` boundaries.
- **[3.11]** `asyncio.TaskGroup` and `asyncio.timeout` add structured concurrency.
- **[3.14]** Significantly improved asyncio introspection, including a command-line tool to inspect the tasks of a running process.

---

# PART 8: Performance, Internals & the CPython Runtime

Bytecode, the adaptive interpreter, the JIT, memory, and C interop.

How CPython runs your code and how to make it faster. Useful once the language is comfortable and you need to optimise or extend.

## 8.1 Compilation & bytecode

- **Source -> bytecode**: Parsing (PEG), AST, compilation, code objects, `__pycache__`.
- `dis`: Reading disassembly; instructions; `compile()`; frames and the evaluation loop.
- **Code & frame objects**: `co_*` attributes, `inspect` for live frames, `sys._getframe`.

## 8.2 The interpreter & JIT

- **Specialising adaptive interpreter**: Per-opcode specialisation (PEP 659): the "faster CPython" core.
- **The JIT compiler**: Experimental copy-and-patch JIT (PEP 744); how it complements the adaptive interpreter; `PYTHON_JIT`.
- **New tail-call interpreter**: An alternative interpreter that, with newer compilers, is notably faster (opt-in, build from source).
- **[3.11]** The specialising adaptive interpreter delivers broad speedups (PEP 659).
- **[3.13]** Experimental JIT introduced (PEP 744).
- **[3.14]** New tail-call interpreter offers significant speedups on certain compilers; experimental JIT now included in official macOS/Windows binaries.

## 8.3 Memory management

- **Reference counting**: How most objects are reclaimed; cycles and why the GC exists.
- **Cyclic garbage collector**: `gc` module: generations, thresholds, `collect`, `freeze`, debugging leaks.
- **Measuring memory**: `sys.getsizeof`, `tracemalloc`, object overhead, `__slots__`.
- **Allocator internals**: pymalloc arenas/pools (conceptual).

## 8.4 Profiling, monitoring & debugging at runtime

- **Profilers**: `cProfile`/`profile` + `pstats`; statistical profilers (third-party).
- **Timing**: `timeit`, `time.perf_counter`, micro-benchmark hygiene.
- **`sys.monitoring`**: Low-overhead event monitoring for tools (PEP 669).
- **Remote debugging**: Zero-overhead external debugger interface (PEP 768); attaching to a running process.
- **Faults & traces**: `faulthandler`, `trace`, audit hooks.
- **[3.14]** External debugger attach interface (PEP 768).

## 8.5 Extending & embedding (C interop)

- `ctypes`: Call shared libraries without compiling.
- **C extension modules**: Writing extensions in C; the build story; alternatives (`cffi`, Cython, `pybind11`: third-party).
- **The Python/C API**: Reference for embedding/extending; the stable ABI / limited API.
- **Configuring the runtime in C**: The improved C API for interpreter configuration (PEP 741).
- **Embedding**: Running Python inside a host C/C++ application.
- **[3.14]** Improved C API for configuring Python (PEP 741).

---

# PART 9: Testing, Packaging, Distribution & Project Workflow

From tests and style to building and publishing a package.

The professional layer that turns code into a maintainable, shippable project.

## 9.1 Testing & quality

- `unittest`: Test cases, fixtures (`setUp`/`tearDown`), assertions, discovery, subtests, skips/expected failures.
- `unittest.mock`: Patching, mocks/spies, autospec, asserting calls.
- `doctest`: Executable documentation examples.
- `pytest`: The de-facto third-party runner: fixtures, parametrisation, plugins (worth adopting).
- **Coverage & property testing**: `coverage.py`, `hypothesis` (third-party).
- **Dev mode & warnings-as-errors**: `-X dev`, `-W error` to surface latent bugs and deprecations.

## 9.2 Style, docs & static checks

- **PEP 8 & PEP 257**: Style and docstring conventions.
- **Formatters/linters**: `ruff`, `black`, `flake8`, `isort`, `pylint` (third-party).
- **Type checking in CI**: `mypy`/`pyright` as a gate (Part 4).
- **Documentation**: Docstrings + Sphinx/MkDocs (third-party) for published docs.

## 9.3 Packaging & distribution

- `pyproject.toml`: The standard project metadata + build-system table; PEP 517/518/621.
- **Build backends**: `setuptools`, `hatchling`, `flit`, `pdm`, `maturin` (third-party backends).
- **Building artifacts**: `python -m build` to produce sdists and wheels; the wheel format.
- **Publishing**: `twine upload` to PyPI; TestPyPI; trusted publishing.
- **Versioning & dependencies**: Specifiers, extras, environment markers, lockfiles.
- **Stdlib helpers**: `venv`, `ensurepip`, `zipapp`, `importlib.metadata` (Parts 6.24/6.27).
- **Official guidance**: The Python Packaging User Guide is the canonical reference.

---

# PART 10: What's New, Version by Version (3.10 → 3.14)

The dedicated changelog view: the same features, grouped per release.

A consolidated, release-by-release summary so you can see exactly what changed between any two versions. Each entry references the PEP where one applies. These mirror the official "What's New" guides.

## 10.1 Python 3.10 (October 2021)

- **Structural pattern matching**: `match`/`case` (PEP 634/635/636).
- **Parenthesized context managers**: Clean multi-line `with (...)` groups.
- **Better error messages**: Far more precise SyntaxError/NameError/AttributeError/IndentationError with suggestions; precise line numbers.
- `X | Y` **union types**: PEP 604 union syntax in annotations and `isinstance`.
- **Typing additions**: `ParamSpec` (612), `TypeAlias` (613), `TypeGuard` (647).
- `EncodingWarning`: Opt-in warning for implicit text encodings (PEP 597).
- **dataclasses**: `slots=True`, `kw_only=True`.
- **Library**: `itertools.pairwise`; `statistics` correlation/covariance/linear_regression; `zoneinfo` matured.

## 10.2 Python 3.11 (October 2022)

- **Faster CPython**: The specializing adaptive interpreter (PEP 659): broadly 10–60% faster.
- **Exception groups & `except*`**: Handle multiple concurrent errors (PEP 654).
- **Fine-grained tracebacks**: Carets point at the exact failing sub-expression (PEP 657).
- `tomllib`: Read-only TOML parser in the stdlib (PEP 680).
- **Typing**: `Self` (673), `TypeVarTuple` variadic generics (646), `Required`/`NotRequired` (655), `LiteralString` (675), `assert_type`/`reveal_type`.
- `Exception.add_note()`: Attach context to exceptions (PEP 678).
- **asyncio**: `TaskGroup` and `timeout` (structured concurrency).
- **enum**: `StrEnum`, `@verify`, reworked `Flag`.
- **Other**: `contextlib.chdir`; CPython startup/maths speedups.

## 10.3 Python 3.12 (October 2023)

- **Type parameter syntax**: `class C[T]`, `def f[T]`, and the `type` statement (PEP 695).
- **f-string formalisation**: Nesting, quote reuse, multi-line, backslashes, comments inside `{}` (PEP 701).
- **Typing**: `TypedDict` for `**kwargs` (692); `@override` (698).
- **Per-interpreter GIL**: Foundation for subinterpreter parallelism (PEP 684).
- `sys.monitoring`: Low-impact monitoring API (PEP 669).
- **Comprehension inlining**: Faster comprehensions (PEP 709).
- **Buffer protocol in Python**: `__buffer__` / `collections.abc.Buffer` (PEP 688).
- **Library**: `itertools.batched`; `pathlib` subclassing improvements; improved error messages.
- **Removals**: `distutils` removed from the stdlib.

## 10.4 Python 3.13 (October 2024)

- **New interactive interpreter**: PyPy-derived REPL: multiline editing, history, colour; colour tracebacks by default.
- **Experimental free threading**: `--disable-gil` build (PEP 703).
- **Experimental JIT**: Copy-and-patch JIT, off by default (PEP 744).
- `locals()` **semantics**: Defined behaviour for mutating the returned mapping (PEP 667).
- **Typing**: `TypeIs` (742), `ReadOnly` TypedDict items (705), `@deprecated` (702), type-parameter defaults (696).
- **Platforms**: Android and iOS become Tier-3 supported.
- **Library**: `copy.replace()`; `dbm.sqlite3` default; `random` CLI; `__static_attributes__`.
- **Removals**: PEP 594 "dead batteries" (19 modules) removed.

## 10.5 Python 3.14 (October 2025)

- **Template strings (t-strings)**: `t"..."` -> `Template` for safe interpolation (PEP 750).
- **Deferred annotations**: Annotations evaluated lazily; new `annotationlib` (PEP 649/749).
- **Subinterpreters in the stdlib**: `concurrent.interpreters` and `InterpreterPoolExecutor` (PEP 734).
- **Free threading supported**: No longer experimental (PEP 779); single-thread penalty ~5–10%.
- **Zstandard**: `compression` package with `compression.zstd` (PEP 784).
- **Syntax & errors**: `except`/`except*` without brackets (PEP 758); no `return`/`break`/`continue` exiting `finally` (PEP 765); even better messages.
- **Tooling**: Syntax highlighting in PyREPL; colour CLIs (`unittest`/`argparse`/`json`/`calendar`); asyncio process-inspection CLI.
- **Debugging & C API**: External debugger attach interface (PEP 768); improved configuration C API (PEP 741).
- **Performance**: New tail-call interpreter; experimental JIT in official macOS/Windows binaries.
- **Library**: `uuid` v6–8 + faster v3–5; built-in HACL* `hmac`.
- **Build/platform**: PGP signatures dropped for Sigstore (PEP 761); Emscripten Tier-3 (PEP 776); official Android binaries; new Windows install manager.

## 10.6 Deprecations & removals: staying current

- **Read the "Deprecated" / "Removed" sections**: Every "What's New" ends with them; plan migrations early.
- **Surface issues ahead of time**: Run `-W error::DeprecationWarning` and your tests on the next version before upgrading.
- **Common removals to watch**: `distutils` (3.12) and the PEP 594 modules (3.13); see 6.32 for replacements.

---

# PART 11: The Ecosystem & Where to Go Next

Beyond the stdlib: PyPI, domain libraries, and official learning resources.

The standard library is only the core. This part points outward so the roadmap connects to real-world work: all clearly third-party unless noted.

## 11.1 PyPI & popular libraries by domain

- **Package Index**: PyPI hosts hundreds of thousands of packages; install with `pip`.
- **Web**: Django, Flask, FastAPI; `requests`/`httpx` for HTTP clients.
- **Data & science**: NumPy, pandas, polars, SciPy, matplotlib.
- **Machine learning**: scikit-learn, PyTorch, TensorFlow, JAX.
- **Automation & scraping**: Selenium/Playwright, BeautifulSoup, Scrapy.
- **Validation & settings**: pydantic, attrs.
- **CLI & TUI**: Click, Typer, Rich, Textual.
- **Tooling**: ruff, black, mypy, pytest, uv, poetry.

## 11.2 Official resources & next steps

- **The Tutorial**: Read it end-to-end if you skipped it; it complements Parts 0–5.
- **Python HOWTOs**: Deep topic guides: logging, regex, sorting, Unicode, argparse, descriptors, enums, functional programming, sockets, typing, concurrency, annotations, etc.
- **FAQs**: General, programming, design-and-history, library, and Windows FAQs.
- **Language & Library references**: The authoritative specs this roadmap maps onto.
- **"What's New" guides**: Track each release; pair with Part 10.
- **The Packaging User Guide**: Canonical packaging/distribution reference.
- **Static Typing guide**: For going deep on type systems.
- **Contributing**: The Developer's Guide, the CPython repo, PEPs, and the community/discuss forums.

---

# APPENDIX A: Built-in Functions: Complete List

Every always-available function.

All built-in functions available without any import (alphabetical).

## A. The built-ins

- **A–C**: `abs`, `aiter`, `all`, `anext`, `any`, `ascii`, `bin`, `bool`, `breakpoint`, `bytearray`, `bytes`, `callable`, `chr`, `classmethod`, `compile`, `complex`.
- **D–G**: `delattr`, `dict`, `dir`, `divmod`, `enumerate`, `eval`, `exec`, `filter`, `float`, `format`, `frozenset`, `getattr`, `globals`.
- **H–L**: `hasattr`, `hash`, `help`, `hex`, `id`, `input`, `int`, `isinstance`, `issubclass`, `iter`, `len`, `list`, `locals`.
- **M–R**: `map`, `max`, `memoryview`, `min`, `next`, `object`, `oct`, `open`, `ord`, `pow`, `print`, `property`, `range`, `repr`, `reversed`, `round`.
- **S–Z**: `set`, `setattr`, `slice`, `sorted`, `staticmethod`, `str`, `sum`, `super`, `tuple`, `type`, `vars`, `zip`, `__import__`.

---

# APPENDIX B: Built-in Exception Hierarchy

The exception tree to memorise.

Concrete classes inherit from these bases; catch at the right level.

## B. Hierarchy

- `BaseException`: Root of all exceptions.
  - `BaseExceptionGroup`: Base for groups; `ExceptionGroup` when all members are `Exception`.
  - `KeyboardInterrupt`, `SystemExit`, `GeneratorExit`: Control-flow exceptions not caught by bare `except Exception`.
  - `Exception`: Base for ordinary errors.
    - `ArithmeticError`: `ZeroDivisionError`, `OverflowError`, `FloatingPointError`.
    - `LookupError`: `IndexError`, `KeyError`.
    - `OSError`: `FileNotFoundError`, `PermissionError`, `TimeoutError`, `ConnectionError` family, etc.
    - `ValueError`, `TypeError`, `RuntimeError`: Incl. `UnicodeError`, `RecursionError`, `NotImplementedError`.
    - `NameError`, `AttributeError`, `ImportError`: Incl. `ModuleNotFoundError`.
    - `StopIteration`, `StopAsyncIteration`: Iterator termination signals.
    - `Warning`: `DeprecationWarning`, `UserWarning`, `EncodingWarning`, etc.

---

# APPENDIX C: Keywords & Soft Keywords

Reserved words and the context-sensitive ones.

Hard keywords cannot be used as identifiers; soft keywords are only special in context.

## C. Reserved words

**Hard keywords**

`False`, `None`, `True`, `and`, `as`, `assert`, `async`, `await`, `break`, `class`, `continue`, `def`, `del`, `elif`, `else`, `except`, `finally`, `for`, `from`, `global`, `if`, `import`, `in`, `is`, `lambda`, `nonlocal`, `not`, `or`, `pass`, `raise`, `return`, `try`, `while`, `with`, `yield`.

**Soft keywords**

- `match`, `case`, `_`: Structural pattern matching (3.10+).
- `type`: The `type` statement for type aliases (3.12+).

---

# APPENDIX D: Operator Precedence (high → low)

Resolve ambiguity without guessing.

From most-binding to least-binding; parenthesise when in doubt.

## D. Precedence table

- **Parentheses / display**: `(...)`, `[...]`, `{...}`, comprehensions.
- **Subscription / call / attribute**: `x[i]`, `x(...)`, `x.attr`.
- `await`: Await expression.
- `**`: Exponentiation (right-associative).
- **Unary**: `+x`, `-x`, `~x`.
- `* / // % @`: Multiplicative / matmul.
- `+ -`: Additive.
- `<< >>`: Shifts.
- `&` then `^` then `|`: Bitwise AND, XOR, OR.
- **Comparisons**: `< <= > >= == != is in` (and negations); chainable.
- `not` -> `and` -> `or`: Boolean operators.
- `if`/`else` **ternary**: Conditional expression.
- `lambda`: Lambda.
- `:=`: Assignment expression (lowest).

---

# APPENDIX E: Standard-Library Module Checklist

Tick every module off as you learn it.

A compact, grouped index of every stdlib module covered in Part 6: use it as a progress tracker. (Grouping matches the official categories.)

## E. Every module, by group

- **Text:** string, string.templatelib, re, difflib, textwrap, unicodedata, stringprep, readline, rlcompleter
- **Binary data:** struct, codecs
- **Data types:** datetime, zoneinfo, calendar, collections, collections.abc, heapq, bisect, array, weakref, types, copy, pprint, reprlib, enum, graphlib
- **Numeric/math:** numbers, math, cmath, decimal, fractions, random, statistics
- **Functional:** itertools, functools, operator
- **Files/dirs:** pathlib, os.path, stat, filecmp, tempfile, glob, fnmatch, linecache, shutil
- **Persistence:** pickle, copyreg, shelve, marshal, dbm, sqlite3
- **Compression:** compression, compression.zstd, zlib, gzip, bz2, lzma, zipfile, tarfile
- **File formats:** csv, configparser, tomllib, netrc, plistlib
- **Crypto:** hashlib, hmac, secrets
- **Generic OS:** os, io, time, logging, logging.config, logging.handlers, platform, errno, ctypes
- **CLI libs:** argparse, optparse, getpass, fileinput, curses, curses.textpad, curses.ascii, curses.panel, cmd
- **Concurrency:** threading, multiprocessing, multiprocessing.shared_memory, concurrent, concurrent.futures, concurrent.interpreters, subprocess, sched, queue, contextvars, _thread
- **Networking/IPC:** asyncio, socket, ssl, select, selectors, signal, mmap
- **Internet data:** email, json, mailbox, mimetypes, base64, binascii, quopri
- **Markup:** html, html.parser, html.entities, xml.etree.ElementTree, xml.dom, xml.dom.minidom, xml.dom.pulldom, xml.sax, xml.sax.handler, xml.sax.saxutils, xml.sax.xmlreader, xml.parsers.expat
- **Internet protocols:** webbrowser, wsgiref, urllib(.request/.response/.parse/.error/.robotparser), http(.client/.server/.cookies/.cookiejar), ftplib, poplib, imaplib, smtplib, uuid, socketserver, xmlrpc(.client/.server), ipaddress
- **Multimedia:** wave, colorsys
- **i18n:** gettext, locale
- **Tk GUI:** tkinter, tkinter.colorchooser, tkinter.font, tkinter dialogs, tkinter.messagebox, tkinter.scrolledtext, tkinter.dnd, tkinter.ttk, IDLE, turtle
- **Dev tools:** typing, pydoc, devmode, doctest, unittest, unittest.mock, test, test.support(+helpers)
- **Debug/profile:** bdb, faulthandler, pdb, profile, cProfile, timeit, trace, tracemalloc, audit events
- **Packaging:** ensurepip, venv, zipapp
- **Runtime:** sys, sys.monitoring, sysconfig, builtins, __main__, warnings, dataclasses, contextlib, abc, atexit, traceback, __future__, gc, inspect, annotationlib, site
- **Custom interpreters:** code, codeop
- **Importing:** zipimport, pkgutil, modulefinder, runpy, importlib, importlib.resources, importlib.resources.abc, importlib.metadata
- **Language services:** ast, symtable, token, keyword, tokenize, tabnanny, pyclbr, py_compile, compileall, dis, pickletools
- **Windows:** msvcrt, winreg, winsound
- **Unix:** shlex, posix, pwd, grp, termios, tty, pty, fcntl, resource, syslog
- **Superseded:** getopt

---

# APPENDIX F: Official Documentation Map

Where each part of this roadmap lives on docs.python.org.

Open any of these to get the full detail behind a roadmap node.

## F. Documentation sections

- **Tutorial**: docs.python.org/3/tutorial: Parts 0–5.
- **Language Reference**: docs.python.org/3/reference: Parts 1–3, 5.
- **Standard Library**: docs.python.org/3/library: Part 6 (and 4, 7, 8.x modules).
- **Setup & Usage**: docs.python.org/3/using: Part 0.
- **HOWTOs**: docs.python.org/3/howto: deep dives across many parts.
- **Installing / Distributing**: docs.python.org/3/installing & /distributing + the Packaging Guide: Part 9.
- **Extending & Embedding / C API**: docs.python.org/3/extending & /c-api: Part 8.
- **What's New**: docs.python.org/3/whatsnew: Part 10.
- **FAQs**: docs.python.org/3/faq: Part 11.
