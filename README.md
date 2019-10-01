 ![Logo](awesome.png)

> Static program analysis is the analysis of computer software that is performed without actually executing programs — [Wikipedia](https://en.wikipedia.org/wiki/Static_program_analysis)

This is a collection of static analysis tools and code quality checkers starting with this list: https://github.com/mre/awesome-static-analysis and improving it (by removing outdated projects and unrealistically expensive commercial tools). Further, some tools had limited functionality that other tools might have excelled at; choice adjustments were made to limit the number of tool functionality overlap. 


# Table of Contents

#### [Programming Languages](#programming-languages-1)

<details>
 <summary>Show languages</summary>
  <!-- Please use HTML syntax here so that it works for Github and mkdocs -->
  <ul>
    <li><a href="#cc">C/C++</a></li>
    <li><a href="#c">C#</a></li>
    <li><a href="#go">Go</a></li>
    <li><a href="#java">Java</a></li>
    <li><a href="#javascript">JavaScript</a></li>
    <li><a href="#php">PHP</a></li>
    <li><a href="#python">Python</a></li>
    <li><a href="#ruby">Ruby</a></li>
    <li><a href="#rust">Rust</a></li>
    <li><a href="#shell">Shell</a></li>
    <li><a href="#sql">SQL</a></li>
  </ul>
</details>

#### [Multiple languages](#multiple-languages-1)

#### [Other](#other-1)

---

# Compiled Programming Languages

## C/C++ #
[Metrics]
* [cqmetrics](https://github.com/dspinellis/cqmetrics) - quality metrics for C code
* [CScout](https://www.spinellis.gr/cscout/) - complexity and quality metrics for for C and C preprocessor code
* [include-gardener](https://github.com/feddischson/include_gardener) - a static analyzer for C/C++/Obj-C to create a graph (in dot or graphml format) which shows all `#include` relations of a given set of files.

[Quality]
* [clang-tidy](http://clang.llvm.org/extra/clang-tidy/) - clang static analyser
* [cppcheck](https://github.com/danmar/cppcheck) - static analysis of C/C++ code
* [flawfinder](http://www.dwheeler.com/flawfinder/) - finds possible security weaknesses
* [Frama-C](http://frama-c.com/) - a sound and extensible static analyzer for C code
* [scan-build](https://clang-analyzer.llvm.org/scan-build.html) - Analyzes C/C++ code using LLVM at compile-time

[Linter]
* [cpplint](https://github.com/google/styleguide/tree/gh-pages/cpplint) - automated C++ checker that follows Google's style guide
* [oclint](http://oclint.org/) - A static source code analysis tool to improve quality and reduce defects for C, C++ and Objective-C
* [splint](https://github.com/ravenexp/splint) - Annotation-assisted static program checker

[Correctness]
* [CBMC](http://www.cprover.org/cbmc/) - bounded model-checker for C programs, user-defined assertions, standard assertions, several coverage metric analyses
* [IKOS](https://github.com/nasa-sw-vnv/ikos) - a sound static analyzer for C/C++ code based on LLVM
* [SVF](https://github.com/SVF-tools/SVF) - a static tool that enables scalable and precise interprocedural dependence analysis for C and C++ programs.

## C# #
* [.NET Analyzers](https://github.com/DotNetAnalyzers) - An organization for the development of analyzers (diagnostics and code fixes) using the .NET Compiler Platform.
* [Code Analysis Rule Collection](https://carc.codeplex.com/) - Contains a set of diagnostics, code fixes and refactorings built on the Microsoft .NET Compiler Platform "Roslyn".
* [code-cracker](https://github.com/code-cracker/code-cracker) - An analyzer library for C# and VB that uses Roslyn to produce refactorings, code analysis, and other niceties.
* [Gendarme](http://www.mono-project.com/docs/tools+libraries/tools/gendarme/) - Gendarme inspects programs and libraries that contain code in ECMA CIL format (Mono and .NET).
* [Puma Scan](https://github.com/pumasecurity/puma-scan) - Puma Scan provides real time secure code analysis for common vulnerabilities (XSS, SQLi, CSRF, LDAPi, crypto, deserialization, etc.) as development teams write code in Visual Studio.
* [Refactoring Essentials](http://vsrefactoringessentials.com/) - The free Visual Studio 2015 extension for C# and VB.NET refactorings, including code best practice analyzers.
* [Roslyn Security Guard](https://dotnet-security-guard.github.io/) - Project that focuses on the identification of potential vulnerabilities such as SQL injection, cross-site scripting (XSS), CSRF, cryptography weaknesses, hardcoded passwords and many more.
* [Roslynator](https://github.com/JosefPihrt/Roslynator/) - A collection of 190+ analyzers and 190+ refactorings for C#, powered by Roslyn.
* [Security Code Scan](https://security-code-scan.github.io/) - Security code analyzer for C# and VB.NET. Detects various security vulnerability patterns: SQLi, XSS, CSRF, XXE, Open Redirect, etc.
* [SonarLint for Visual Studio](https://vs.sonarlint.org/) - SonarLint is an extension for Visual Studio 2015 and 2017 that provides on-the-fly feedback to developers on new bugs and quality issues injected into .NET code.
* [VSDiagnostics](https://github.com/Vannevelj/VSDiagnostics) - A collection of static analyzers based on Roslyn that integrates with VS.


## Go
* [deadcode](https://github.com/tsenart/deadcode) - Finds unused code.
* [dingo-hunter](https://github.com/nickng/dingo-hunter) - Static analyser for finding deadlocks in Go.
* [dupl](https://github.com/mibk/dupl) - Reports potentially duplicated code.
* [errcheck](https://github.com/kisielk/errcheck) - Check that error return values are used.
* [flen](https://github.com/lafolle/flen) - Get info on length of functions in a Go package.
* [gas](https://github.com/GoASTScanner/gas) - Inspects source code for security problems by scanning the Go AST.
* [Go Meta Linter](https://github.com/alecthomas/gometalinter) - Concurrently run Go lint tools and normalise their output.
* [go tool vet --shadow](https://golang.org/cmd/vet/#hdr-Shadowed_variables) - Reports variables that may have been unintentionally shadowed.
* [go vet](https://golang.org/cmd/vet/) - Examines Go source code and reports suspicious.
* [go-consistent](https://github.com/Quasilyte/go-consistent) - Analyzer that helps you to make your Go programs more consistent.
* [go-critic](https://github.com/go-critic/go-critic) - Go source code linter that maintains checks which are currently not implemented in other linters.
* [go-staticcheck](https://github.com/dominikh/go-tools/tree/master/cmd/staticcheck) - go vet on steroids, similar to ReSharper for C#.
* [go/ast](https://golang.org/pkg/go/ast/) - Package ast declares the types used to represent syntax trees for Go packages.
* [goconst](https://github.com/jgautheron/goconst) - Finds repeated strings that could be replaced by a constant.
* [gocyclo](https://github.com/fzipp/gocyclo) - Calculate cyclomatic complexities of functions in Go source code.
* [gofmt -s](https://golang.org/cmd/gofmt/) - Checks if the code is properly formatted and could not be further simplified.
* [goimports](https://godoc.org/golang.org/x/tools/cmd/goimports) - Checks missing or unreferenced package imports.
* [GolangCI-Lint](https://github.com/golangci/golangci-lint) - Alternative to `Go Meta Linter`: GolangCI-Lint is a linters aggregator.
* [golint](https://github.com/golang/lint) - Prints out coding style mistakes in Go source code.
* [goreporter](https://github.com/wgliang/goreporter) - concurrently runs many linters and normalises their output to a report.
* [goroutine-inspect](https://github.com/linuxerwang/goroutine-inspect) - An interactive tool to analyze Golang goroutine dump.
* [gosimple](https://github.com/dominikh/go-tools/tree/master/cmd/gosimple) - Report simplifications in code.
* [gotype](https://golang.org/x/tools/cmd/gotype) - Syntactic and semantic analysis similar to the Go compiler.
* [ineffassign](https://github.com/gordonklaus/ineffassign) - Detect ineffectual assignments in Go code
* [interfacer](https://github.com/mvdan/interfacer) - Suggest narrower interfaces that can be used.
* [lll](https://github.com/walle/lll) - Report long lines.
* [maligned](https://github.com/mdempsky/maligned) -  Detect structs that would take less memory if their fields were sorted.
* [megacheck](https://github.com/dominikh/go-tools/tree/master/cmd/megacheck) - Run staticcheck, gosimple and unused, sharing work.
* [misspell](https://github.com/client9/misspell) - Finds commonly misspelled English words.
* [nakedret](https://github.com/alexkohler/nakedret) - Finds naked returns.
* [nargs](https://github.com/alexkohler/nargs) - Finds unused arguments in function declarations.
* [prealloc](https://github.com/alexkohler/prealloc) - Finds slice declarations that could potentially be preallocated.
* [revive](https://github.com/mgechev/revive) - Fast, configurable, extensible, flexible, and beautiful linter for Go. Drop-in replacement of golint.
* [safesql](https://github.com/stripe/safesql) - Static analysis tool for Golang that protects against SQL injections.
* [structcheck](https://github.com/opennota/check) - Find unused struct fields.
* [test](http://golang.org/pkg/testing/) - Show location of test failures from the stdlib testing module.
* [testify](https://github.com/stretchr/testify) - Show location of failed testify assertions.
* [unconvert](https://github.com/mdempsky/unconvert) - Detect redundant type conversions.
* [unimport](https://github.com/alexkohler/unimport) - Finds unnecessary import aliases
* [unparam](https://github.com/mvdan/unparam) - Find unused function parameters.
* [unused](https://github.com/dominikh/go-tools/tree/master/cmd/unused) - Find unused variables.
* [varcheck](https://github.com/opennota/check) - Find unused global variables and constants.

## Java (Interpreted)
[Metrics]
* [ck](https://github.com/mauricioaniche/ck) - calculates Chidamber and Kemerer object-oriented metrics by processing the source Java files
* [ckjm](http://www.spinellis.gr/sw/ckjm/) - calculates Chidamber and Kemerer object-oriented metrics by processing the bytecode of compiled Java files
* [ClassGraph](https://github.com/classgraph/classgraph) - a classpath and module path scanner for querying or visualizing class metadata or class relatedness

[Linting]
* [checkstyle](https://github.com/checkstyle/checkstyle) - checking Java source code for adherence to a Code Standard or set of validation rules (best practices)
* [google-java-format](https://github.com/google/google-java-format) - Google Style Reformat

[Quality]
* [CogniCrypt](https://www.eclipse.org/cognicrypt/) - checks Java source and byte code for incorrect uses of cryptographic APIs
* [Error-prone](https://github.com/google/error-prone) - Catch common Java mistakes as compile-time errors
* [fb-contrib](https://github.com/mebigfatguy/fb-contrib) - A plugin for FindBugs with additional bug detectors
* [Find Security Bugs](https://find-sec-bugs.github.io/) - IDE/SonarQube plugin for security audits of Java web applications.
* [SpotBugs](https://spotbugs.github.io/) - SpotBugs is FindBugs' successor. A tool for static analysis to look for bugs in Java code.
* [HuntBugs](https://github.com/amaembo/huntbugs) - Bytecode static analyzer tool based on Procyon Compiler Tools aimed to supersede FindBugs.
* [NullAway](https://github.com/uber/NullAway) - Type-based null-pointer checker with low build-time overhead; an [Error Prone](http://errorprone.info/) plugin
* [OWASP Dependency Check](https://www.owasp.org/index.php/OWASP_Dependency_Check) - Checks dependencies for known, publicly disclosed, vulnerabilities.

[Correctness]
* [Checker Framework](https://github.com/typetools/checker-framework/) - Pluggable type-checking for Java http://checkerframework.org/
* [JBMC](http://www.cprover.org/jbmc/) - bounded model-checker for Java (bytecode), verifies user-defined assertions, standard assertions, several coverage metric analyses
* [Soot](https://sable.github.io/soot/) - A framework for analyzing and transforming Java and Android applications.
* [Spoon](https://github.com/INRIA/spoon) - Library to write your own static analyses and architectural rule checkers for Java. Can be integrated in Maven and Gradle.

[Test]
* [ArchUnit](https://www.archunit.org/) - Unit test your Java architecture

## Ruby (Interpreted)
* [brakeman](https://github.com/presidentbeef/brakeman) - A static analysis security vulnerability scanner for Ruby on Rails applications
* [cane](https://github.com/square/cane) - Code quality threshold checking as part of your build
* [dawnscanner](https://github.com/thesp0nge/dawnscanner) - a static analysis security scanner for ruby written web applications. It supports Sinatra, Padrino and Ruby on Rails frameworks.
* [flay](https://github.com/seattlerb/flay) - Flay analyzes code for structural similarities.
* [flog](https://github.com/seattlerb/flog) - Flog reports the most tortured code in an easy to read pain report. The higher the score, the more pain the code is in.
* [quality](https://github.com/apiology/quality) - Runs quality checks on your code using community tools, and makes sure your numbers don't get any worse over time.
* [Querly](https://github.com/soutaro/querly) - Pattern Based Checking Tool for Ruby
* [Railroader](https://railroader.org/) - An open source static analysis security vulnerability scanner for Ruby on Rails applications.
* [reek](https://github.com/troessner/reek) - Code smell detector for Ruby
* [RuboCop](https://github.com/rubocop-hq/rubocop) - A Ruby static code analyzer, based on the community Ruby style guide.
* [Rubrowser](https://github.com/blazeeboy/rubrowser) - Ruby classes interactive dependency graph generator.
* [rubycritic](https://github.com/whitesmith/rubycritic) - A Ruby code quality reporter
* [Sorbet](https://github.com/sorbet/sorbet) - A fast, powerful type checker designed for Ruby

## Rust
* [cargo-audit](https://github.com/RustSec/cargo-audit) - Audit Cargo.lock for crates with security vulnerabilities reported to the [RustSec Advisory Database](https://github.com/RustSec/advisory-db/).
* [cargo-inspect](https://github.com/mre/cargo-inspect) - Inspect Rust code without syntactic sugar to see what the compiler does behind the curtains.
* [clippy](https://github.com/Manishearth/rust-clippy) - A code linter to catch common mistakes and improve your Rust code
* [linter-rust](https://github.com/AtomLinter/linter-rust) - Linting your Rust-files in Atom, using rustc and cargo
* [rustfix](https://github.com/killercup/rustfix) - read and apply the suggestions made by rustc (and third-party lints, like those offered by clippy).

# Markup Languages
## HTML
* [HTML Tidy](http://www.html-tidy.org/) - Corrects and cleans up HTML and XML documents by fixing markup errors and upgrading legacy code to modern standards.
* [HTMLHint](https://github.com/yaniswang/HTMLHint) - A Static Code Analysis Tool for HTML
* [Polymer-analyzer](https://github.com/Polymer/polymer-analyzer) - A static analysis framework for Web Components.

## CSS
* [CSS Stats](https://github.com/cssstats/cssstats) - Potentially interesting stats on stylesheets
* [CSScomb](https://github.com/csscomb/csscomb.js) - a coding style formatter for CSS. Supports own configurations to make style sheets beautiful and consistent
* [CSSLint](https://github.com/CSSLint/csslint) - Does basic syntax checking and finds problematic patterns or signs of inefficiency
* [GraphMyCSS.com](https://graphmycss.com) - CSS Specificity Graph Generator
* [Project Wallace CSS Analyzer](https://github.com/projectwallace/css-analyzer) - Analytics for CSS, part of [Project Wallace](https://www.projectwallace.com)
* [sass-lint](https://github.com/sasstools/sass-lint) - A Node-only Sass linter for both sass and scss syntax.
* [scsslint](https://github.com/brigade/scss-lint) - Linter for SCSS files
* [Stylelint](http://stylelint.io/) - Linter for SCSS/CSS files

# Script Based Languages
## JavaScript
[Metrics]
* [complexity-report](https://github.com/jared-stilwell/complexity-report) - Software complexity analysis for JavaScript projects
* [escomplex](https://github.com/jared-stilwell/escomplex) - Software complexity analysis of JavaScript-family abstract syntax trees.
* [yardstick](https://github.com/calmh/yardstick) - Javascript code metrics
[Linting]
* [ClosureLinter](https://github.com/google/closure-linter) - ensures that all of your project's JavaScript code follows the guidelines in the Google JavaScript Style Guide. It can also automatically fix many common errors
* [coffeelint](https://github.com/clutchski/coffeelint) - A style checker that helps keep CoffeeScript code clean and consistent.
* [eslint](https://github.com/eslint/eslint) - A fully pluggable tool for identifying and reporting on patterns in JavaScript
* [JSLint](https://github.com/douglascrockford/JSLint) :warning: - The JavaScript Code Quality Tool
* [Prettier](https://github.com/prettier/prettier) - An opinionated code formatter.
* [standard](http://standardjs.com/) - An npm module that checks for Javascript Styleguide issues
* [xo](https://github.com/xojs/xo) - Opinionated but configurable ESLint wrapper with lots of goodies included. Enforces strict and readable code.

[Quality]
* [jshint](https://github.com/jshint/jshint) - detect errors and potential problems in JavaScript code and enforce your team's coding conventions
* [JSPrime](https://github.com/dpnishant/jsprime) - static security analysis tool
* [NodeJSScan](https://github.com/ajinabraham/NodeJsScan) - NodeJsScan is a static security code scanner for Node.js applications.
* [retire.js](https://github.com/RetireJS/retire.js) - Scanner detecting the use of JavaScript libraries with known vulnerabilities
* [tern](https://github.com/ternjs/tern) - A JavaScript code analyzer for deep, cross-editor language support

[Correctness]
* [aether](https://github.com/codecombat/esper.js) - Lint, analyze, normalize, transform, sandbox, run, step through, and visualize user JavaScript, in node or the browser.
* [Esprima](https://github.com/jquery/esprima) - ECMAScript parsing infrastructure for multipurpose analysis
* [flow](https://flow.org/) - A static type checker for JavaScript.

## PHP
* [dephpend](https://github.com/mihaeu/dephpend) - Dependency analysis tool
* [deprecation-detector](https://github.com/sensiolabs-de/deprecation-detector) - Finds usages of deprecated (Symfony) code
* [deptrac](https://github.com/sensiolabs-de/deptrac) - Enforce rules for dependencies between software layers.
* [DesignPatternDetector](https://github.com/Halleck45/DesignPatternDetector) - detection of design patterns in PHP code
* [EasyCodingStandard](https://github.com/Symplify/EasyCodingStandard) - combine [PHP_CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer) and [PHP-CS-Fixer](https://github.com/FriendsOfPHP/PHP-CS-Fixer)
* [exakat](https://github.com/exakat/exakat) - An automated code reviewing engine for PHP
* [GrumPHP](https://github.com/phpro/grumphp) - checks code on every commit
* [Mondrian](https://github.com/Trismegiste/Mondrian) - a set of static analysis and refactoring tools which use graph theory
* [parallel-lint](https://github.com/JakubOnderka/PHP-Parallel-Lint) - This tool checks syntax of PHP files faster than serial check with a fancier output.
* [Parse](https://github.com/psecio/parse) - A Static Security Scanner
* [pdepend](https://pdepend.org/) - Calculates software metrics like cyclomatic complexity for PHP code.
* [phan](https://github.com/etsy/phan) - a modern static analyzer from etsy
* [PHP Assumptions](https://github.com/rskuipers/php-assumptions) - Checks for weak assumptions
* [PHP Coding Standards Fixer](http://cs.sensiolabs.org/) - Fixes your code according to standards like PSR-1, PSR-2, and the Symfony standard.
* [Php Inspections (EA Extended)](https://github.com/kalessil/phpinspectionsea) - A Static Code Analyzer for PHP.
* [PHP Refactoring Browser](https://github.com/QafooLabs/php-refactoring-browser) - Refactoring helper
* [PHP Semantic Versioning Checker](https://github.com/tomzx/php-semver-checker) - Suggests a next version according to semantic versioning
* [PHP-Parser](https://github.com/nikic/PHP-Parser) - A PHP parser written in PHP
* [PHP-Token-Reflection](https://github.com/Andrewsville/PHP-Token-Reflection) - Library emulating the PHP internal reflection
* [php7cc](https://github.com/sstalle/php7cc) - PHP 7 Compatibility Checker
* [php7mar](https://github.com/Alexia/php7mar) - assist developers in porting their code quickly to PHP 7
* [PHP_CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer) - detects violations of a defined set of coding standards
* [phpca](https://github.com/wapmorgan/PhpCodeAnalyzer) - Finds usage of non-built-in extensions
* [phpcf](http://wapmorgan.github.io/PhpCodeFixer/) - Finds usage of deprecated PHP features
* [phpcpd](https://github.com/sebastianbergmann/phpcpd) - Copy/Paste Detector for PHP code.
* [phpdcd](https://github.com/sebastianbergmann/phpdcd) - Dead Code Detector (DCD) for PHP code.
* [PhpDependencyAnalysis](https://github.com/mamuz/PhpDependencyAnalysis) - builds a dependency graph for a project
* [phpdoc-to-typehint](https://github.com/dunglas/phpdoc-to-typehint) - Add scalar type hints and return types to existing PHP projects using PHPDoc annotations
* [phpDocumentor](https://www.phpdoc.org/) - Analyzes PHP source code to generate documentation
* [PHPMD](https://phpmd.org/) - finds possible bugs in your code
* [PhpMetrics](http://www.phpmetrics.org/) - Calculates and visualizes various code quality metrics
* [phpmnd](https://github.com/povils/phpmnd) - Helps to detect magic numbers
* [PHPQA](https://github.com/EdgedesignCZ/phpqa) - A tool for running QA tools (phploc, phpcpd, phpcs, pdepend, phpmd, phpmetrics)
* [phpqa - jakzal](https://github.com/jakzal/phpqa) - Many tools for PHP static analysis in one container
* [phpqa - jmolivas](https://github.com/jmolivas/phpqa) - PHPQA all-in-one Analyzer CLI tool
* [phpsa](https://github.com/ovr/phpsa) - Static analysis tool for PHP.
* [PHPStan](https://github.com/phpstan/phpstan) - PHP Static Analysis Tool - discover bugs in your code without running it!
* [Progpilot](https://github.com/designsecurity/progpilot) - A static analysis tool for security purposes
* [Psalm](https://getpsalm.org/) - Static analysis tool for finding type errors in PHP applications
* [Qafoo Quality Analyzer](https://github.com/Qafoo/QualityAnalyzer) - Visualizes metrics and source code
* [Tuli](https://github.com/ircmaxell/Tuli) - A static analysis engine
* [twig-lint](https://github.com/asm89/twig-lint) - twig-lint is a lint tool for your twig files.
* [WAP](https://www.owasp.org/index.php/OWASP_WAP-Web_Application_Protection) - Tool to detect and correct input validation vulnerabilities in PHP (4.0 or higher) web applications and predicts false positives by combining static analysis and data mining.

## Python
* [bandit](https://github.com/PyCQA/bandit) - a tool to find common security issues in Python code
* [bellybutton](https://github.com/hchasestevens/bellybutton) - a linting engine supporting custom project-specific rules
* [Black](https://github.com/ambv/black) - The uncompromising Python code formatter
* [cohesion](https://github.com/mschwager/cohesion) - a tool for measuring Python class cohesion
* [Dlint](https://github.com/duo-labs/dlint) - a tool for ensuring Python code is secure
* [jedi](https://github.com/davidhalter/jedi) - autocompletion/static analysis library for Python
* [linty fresh](https://github.com/lyft/linty_fresh) - parse lint errors and report them to Github as comments on a pull request
* [mccabe](https://github.com/PyCQA/mccabe) - check McCabe complexity
* [mypy](https://github.com/python/mypy) - a static type checker that aims to combine the benefits of duck typing and static typing, frequently used with [MonkeyType](https://github.com/Instagram/MonkeyType)
* [py-find-injection](https://github.com/uber/py-find-injection) - find SQL injection vulnerabilities in Python code
* [pycodestyle](https://github.com/PyCQA/pycodestyle) - (formerly `pep8`) check Python code against some of the style conventions in PEP 8
* [pydocstyle](https://github.com/PyCQA/pydocstyle) - check compliance with Python docstring conventions
* [pyflakes](https://github.com/pyflakes/pyflakes/) - check Python source files for errors
* [pylint](https://github.com/PyCQA/pylint) - looks for programming errors, helps enforcing a coding standard and sniffs for some code smells. It additionally includes `pyreverse` (an UML diagram generator) and `symilar` (a similarities checker).
* [pyre-check](https://github.com/facebook/pyre-check) - A fast, scalable type checker for large Python codebases
* [pyright](https://github.com/Microsoft/pyright) - Static type checker for Python, created to address gaps in existing tools like mypy.
* [pyroma](https://github.com/regebro/pyroma) - rate how well a Python project complies with the best practices of the Python packaging ecosystem, and list issues that could be improved
* [PyT - Python Taint](https://github.com/python-security/pyt) - A static analysis tool for detecting security vulnerabilities in Python web applications.
* [pytype](https://github.com/google/pytype) - A static type analyzer for Python code.
* [radon](https://github.com/rubik/radon) - a Python tool that computes various metrics from the source code
* [vulture](https://github.com/jendrikseipp/vulture) - find unused classes, functions and variables in Python code
* [wemake-python-styleguide](https://github.com/wemake-services/wemake-python-styleguide) - the strictest and most opinionated python linter ever
* [wily](https://github.com/tonybaloney/wily) - a command-line tool for archiving, exploring and graphing the complexity of Python source code
* [xenon](https://github.com/rubik/xenon) - monitor code complexity using [`radon`](https://github.com/rubik/radon)

## Python wrappers
* [ciocheck](https://github.com/ContinuumIO/ciocheck) - linter, formatter and test suite helper. As a linter, it is a wrapper around `pep8`, `pydocstyle`, `flake8`, and `pylint`.
* [flake8](https://github.com/PyCQA/flake8) - a wrapper around `pyflakes`, `pycodestyle` and `mccabe`
* [multilint](https://github.com/adamchainz/multilint) - a wrapper around `flake8`, `isort` and `modernize`
* [prospector](https://github.com/PyCQA/prospector) - a wrapper around `pylint`, `pep8`, `mccabe` and others

## Shell
* [i-Code CNES for Shell](https://github.com/lequal/i-CodeCNES) - An open source static code analysis tool for Shell and Fortran (77 and 90).
* [shellcheck](https://github.com/koalaman/shellcheck) - ShellCheck, a static analysis tool that gives warnings and suggestions for bash/sh shell scripts

# Multiple languages
* [coala](https://coala.io/) - Language independent framework for creating code analysis - supports [over 60 languages](https://coala.io/languages) by default
* [codeburner](https://github.com/groupon/codeburner) - Provides a unified interface to sort and act on the issues it finds
* [cqc](https://github.com/xcatliu/cqc) - Check your code quality for js, jsx, vue, css, less, scss, sass and styl files.
* [Depends](https://github.com/multilang-depends/depends) - Analyses the comprehensive dependencies of code elements for Java, C/C++, Ruby.
* [DevSkim](https://github.com/microsoft/devskim) - Regex-based static analysis tool for Visual Studio, VS Code, and Sublime Text - C/C++, C#, PHP, ASP, Python, Ruby, Java, and others.
* [Goodcheck](https://github.com/sideci/goodcheck) - Regexp based customizable linter
* [graudit](https://github.com/wireghoul/graudit) - Grep rough audit - source code auditing tool - C/C++, PHP, ASP, C#, Java, Perl, Python, Ruby
* [Hound CI](https://houndci.com/) - Comments on style violations in GitHub pull requests. Supports Coffeescript, Go, HAML, JavaScript, Ruby, SCSS and Swift.
* [imhotep](https://github.com/justinabrahms/imhotep) - Comment on commits coming into your repository and check for syntactic errors and general lint warnings.
* [Infer](https://github.com/facebook/infer) - A static analyzer for Java, C and Objective-C
* [pfff](https://github.com/facebook/pfff) - Facebook's tools for code analysis, visualizations, or style-preserving source transformation for many languages
* [PMD](https://pmd.github.io/) - A source code analyzer for Java, Javascript, PLSQL, XML, XSL and others
* [Pronto](https://github.com/prontolabs/pronto) - Quick automated code review of your changes. Supports more than 40 runners for various languages, including Clang, Elixir, JavaSCript, PHP, Ruby and more
* [pre-commit](https://github.com/pre-commit/pre-commit) - A framework for managing and maintaining multi-language pre-commit hooks.
* [PT.PM](https://github.com/PositiveTechnologies/PT.PM) - An engine for searching patterns in the source code, based on Unified AST or UST. At present time C#, Java, PHP, PL/SQL, T-SQL, and JavaScript are supported. Patterns can be described within the code or using a DSL.
* [Reviewdog](https://github.com/haya14busa/reviewdog) - A tool for posting review comments from any linter in any code hosting service.
* [qulice](https://www.qulice.com/) - combines a few (pre-configured) static analysis tools (checkstyle, PMD, Findbugs, ...).
* [Security Code Scan](https://security-code-scan.github.io/) - Security code analyzer for C# and VB.NET. Detects various security vulnerability patterns: SQLi, XSS, CSRF, XXE, Open Redirect, etc.
* [shipshape](https://github.com/google/shipshape) - Static program analysis platform that allows custom analyzers to plug in through a common interface
* [STOKE](https://github.com/StanfordPL/stoke) - a programming-language agnostic stochastic optimizer for the x86_64 instruction set. It uses random search to explore the extremely high-dimensional space of all possible program transformations
* [TscanCode](https://github.com/Tencent/TscanCode) - A fast and accurate static analysis solution for C/C++, C#, Lua codes provided by Tencent. Using GPLv3 license.
* [Undebt](https://github.com/Yelp/undebt) - Language-independent tool for massive, automatic, programmable refactoring based on simple pattern definitions
* [WALA](http://wala.sourceforge.net/wiki/index.php/Main_Page) - static analysis capabilities for Java bytecode and related languages and for JavaScript
* [Wotan](https://github.com/fimbullinter/wotan) - Pluggable TypeScript and JavaScript linter

# Other
## Build tools
* [checkmake](https://github.com/mrtazz/checkmake) - Linter / Analyzer for Makefiles
* [codechecker](https://github.com/Ericsson/codechecker) - a defect database and viewer extension for the Clang Static Analyzer

## Binaries
* [BinSkim](https://github.com/Microsoft/binskim) - A binary static analysis tool that provides security and correctness results for Windows portable executables.
* [cwe_checker](https://github.com/fkie-cad/cwe_checker) - cwe_checker finds vulnerable patterns in binary executables.
* [Jakstab](https://github.com/jkinder/jakstab) - Jakstab is an Abstract Interpretation-based, integrated disassembly and static analysis framework for designing analyses on executables and recovering reliable control flow graphs.
* [Manalyze](https://github.com/JusticeRage/Manalyze) - A static analyzer, which checks portable executables for malicious content.
* [Twiggy](https://github.com/rustwasm/twiggy) - Analyzes a binary's call graph to profile code size. The goal is to slim down binaries.

## Containers
* [anchore](https://anchore.io/) - Discover, analyze, and certify container images
* [clair](https://github.com/coreos/clair) - Vulnerability Static Analysis for Containers
* [collector](https://github.com/banyanops/collector) - Run arbitrary scripts inside containers, and gather useful information
* [dagda](https://github.com/eliasgranderubio/dagda) - Perform static analysis of known vulnerabilities in docker images/containers.
* [Docker Label Inspector](https://github.com/garethr/docker-label-inspector) - Lint and validate Dockerfile labels
* [Haskell Dockerfile Linter](https://github.com/lukasmartinelli/hadolint) - A smarter Dockerfile linter that helpsyou build best practice Docker images
* [kube-score](https://github.com/zegl/kube-score) - Static code analysis of your Kubernetes object definitions.


## Config Files
* [dotenv-linter](https://github.com/wemake-services/dotenv-linter) - Linting dotenv files like a charm.
* [gixy](https://github.com/yandex/gixy) - a tool to analyze Nginx configuration. The main goal is to prevent misconfiguration and automate flaw detection.

## IDE Plugins
* [ale](https://github.com/w0rp/ale) - Asynchronous Lint Engine for Vim and NeoVim with support for many languages
* [DevSkim](https://github.com/Microsoft/DevSkim) - Inline, realtime security analysis. Works with multiple programming languages and IDEs (VS, VS Code, Sublime Text, ...).
* [Puma Scan](https://github.com/pumasecurity/puma-scan) - Puma Scan provides real time secure code analysis for common vulnerabilities (XSS, SQLi, CSRF, LDAPi, crypto, deserialization, etc.) as development teams write code in Visual Studio.
* [Security Code Scan](https://security-code-scan.github.io/) - Security code analyzer for C# and VB.NET that integrates into Visual Studio 2015 and newer. Detects various security vulnerability patterns: SQLi, XSS, CSRF, XXE, Open Redirect, etc.
* [vint](https://github.com/Kuniwak/vint) - Fast and Highly Extensible Vim script Language Lint implemented by Python.

## Makefiles
* [portlint](https://www.freebsd.org/cgi/man.cgi?query=portlint&sektion=1&manpath=FreeBSD+8.1-RELEASE+and+Ports) - A verifier for FreeBSD and DragonFlyBSD port directories.

## Mobile
* [android-lint-summary](https://github.com/passy/android-lint-summary) - Combines lint errors of multiple projects into one output, check lint results of multiple sub-projects at once.
* [FlowDroid](https://github.com/secure-software-engineering/soot-infoflow-android) - static taint analysis tool for Android applications
* [paprika](https://github.com/GeoffreyHecht/paprika) - A toolkit to detect some code smells in analyzed Android applications.
* [qark](https://github.com/linkedin/qark) - Tool to look for several security related Android application vulnerabilities

## Packages
* [lintian](https://github.com/Debian/lintian) - Static analysis tool for Debian packages
* [rpmlint](https://github.com/rpm-software-management/rpmlint) - Tool for checking common errors in rpm packages

## SQL
* [sqlint](https://github.com/purcell/sqlint) - Simple SQL linter
* [tsqllint](https://github.com/tsqllint/tsqllint) - T-SQL-specific linter

## Supporting Tools
* [LibVCS4j](https://github.com/uni-bremen-agst/libvcs4j) - A Java library that allows existing tools to analyse the evolution of software systems by providing a common API for different version control systems and issue trackers.
* [Violations Lib](https://github.com/tomasbjerre/violations-lib) - Java library for parsing report files from static code analysis. Used by a bunch of Jenkins, Maven and Gradle plugins.

## Template-Languages
* [ember-template-lint](https://github.com/rwjblue/ember-template-lint) - Linter for Ember or Handlebars templates.
* [haml-lint](https://github.com/brigade/haml-lint) - Tool for writing clean and consistent HAML
* [slim-lint](https://github.com/sds/slim-lint) - Configurable tool for analyzing Slim templates
* [yamllint](https://github.com/adrienverge/yamllint) - Checks YAML files for syntax validity, key repetition and cosmetic problems such as lines length, trailing spaces, and indentation.


## Writing
* [After the Deadline](https://afterthedeadline.com/) :warning: - spell, style and grammar checker
* [codespell](https://github.com/codespell-project/codespell) - check code for common misspellings
* [languagetool](https://github.com/languagetool-org/languagetool) - Style and grammar checker for 25+ languages. It finds many errors that a simple spell checker cannot detect.
* [misspell-fixer](https://github.com/vlajos/misspell-fixer) - Quick tool for fixing common misspellings, typos in source code
* [Misspelled Words In Context](https://github.com/jwilk/mwic) - a spell-checker that groups possible misspellings and shows them in their contexts
* [proselint](https://github.com/amperser/proselint/) - a linter for English prose with a focus on writing style instead of grammar.
* [vale](https://github.com/ValeLint/vale) - A customizable, syntax-aware linter for prose.
* [write-good](https://github.com/btford/write-good) - A linter with a focus on eliminating "weasel words".

## Web services
* [Codecheker](https://github.com/Ericsson/codechecker) - static analysis of C/C++ code, with web GUI
* [QuantifiedCode](https://www.quantifiedcode.com/) - Automated code review & repair

# Less Common Use Cases
ABAP, Ada, Awk, Configuration Management, Crystal, Dlang, Elixir, Elm, Erlang, F#, Fortran, Gherkin, Groovy, Haskell, Haxe, Kotlin, LaTeX, Lua, Markdown, MATLAB, Perl, R, Scala, Solidity, Swift, Tcl, TypeScript, Translation
* See: [Less Common Tools] (https://github.com/mr-segfault/awesome-static-analysis/blob/master/lessCommon.md)

## Commercial Tools
* See: [Commercial Tools] (https://github.com/mr-segfault/awesome-static-analysis/blob/master/commercialTools.md)

## Deprecated Tools
* [2012][CMetrics](https://github.com/MetricsGrimoire/CMetrics) - Measures size and complexity for C files
* [2018][flint++](http://l2program.co.uk/category/flint) - cross-platform, zero-dependency port of flint, a lint program for C++ developed and used at Facebook.
* [2015][vera++](https://bitbucket.org/verateam/vera/wiki/Introduction) - Vera++ is a programmable tool for verification, analysis and transformation of C++ source code.
* [2017][HTML Inspector](https://github.com/philipwalton/html-inspector) - HTML Inspector is a code quality tool to help you and your team write better markup.
* [2017][Corrode](https://github.com/jameysharp/corrode) - Semi-automatic translation from C to Rust. Could reveal bugs in the original implementation by showing Rust compiler warnings and errors.
* [2016][Hopper](https://github.com/cuplv/hopper) - A static analysis tool written in scala for languages that run on JVM
* [2015][quality](https://github.com/jden/quality) - zero configuration code and module linting
* [2016][plato](https://github.com/es-analysis/plato) - Visualize JavaScript source complexity
* [NoLongerOnline][sqlcheck](https://github.com/jarulraj/sqlcheck) - Automatically identify anti-patterns in SQL queries
* [2017] [TSqlRules](https://github.com/ashleyglee/TSqlRules) - TSQL Static Code Analysis Rules for SQL Server
* [2016] [Parker](https://github.com/katiefenn/parker) - Stylesheet analysis tool
* [2016] [Specificity Graph](https://github.com/pocketjoso/specificity-graph) - CSS Specificity Graph Generator
* [2015] [CSharpEssentials](https://github.com/DustinCampbell/CSharpEssentials) - C# Essentials is a collection of Roslyn diagnostic analyzers, code fixes and refactorings that make it easy to work with C# 6 language features.
* [2016][Wintellect.Analyzers](https://github.com/Wintellect/Wintellect.Analyzers) - .NET Compiler Platform ("Roslyn") diagnostic analyzers and code fixes.
* [2011][laser](https://github.com/michaeledgar/laser) - Static analysis and style linter for Ruby code.
* [2015][pelusa](https://github.com/codegram/pelusa) - Static analysis Lint-type tool to improve your OO Ruby code
* [2017][ruby-lint](https://gitlab.com/yorickpeterse/ruby-lint) - Static code analysis for Ruby
* [2015][SandiMeter](https://github.com/makaroni4/sandi_meter) - Static analysis tool for checking Ruby code for Sandi Metz' rules.
* [2017] [electrolysis](https://github.com/Kha/electrolysis) - A tool for formally verifying Rust programs by transpiling them into definitions in the Lean theorem prover.
* [2016] [herbie](https://github.com/mcarton/rust-herbie-lint) - Adds warnings or errors to your crate when using a numerically unstable floating point expression.
* [2018] [Rust Language Server](https://github.com/rust-lang-nursery/rls) - Supports functionality such as 'goto definition', symbol search, reformatting, and code completion, and enables renaming and refactorings.

## License
[![CC0](https://i.creativecommons.org/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

Title image [Designed by Freepik](http://www.freepik.com).
