# Programming Languages

## Reasons for Studying Programming Concepts
- Increased ability to express ideas
- Improved background for choosing appropriate languages
- Increased ability to learn new languages
- Better understanding of significance of implementation
- Better use of languages already known
- Overall advancement of computing

## Programming Domains
- Scientific applications: Fortran (arrays, floating-point computations)
- Business applications: COBOL (reports, decimal numbers, characters)
- Artificial intelligence: LISP (linked lists, symbol manipulation)
- Systems programming: C (efficiency)
- Web Software: XHTML, PHP, Java

## Language Evaluation Criteria
- Readability: Ease of reading/understanding code
- Writability: Ease of writing code
- Reliability: Conformance to specifications
- Cost: Total cost (training, writing, compiling, executing, maintaining)

## Readability
- Orthogonality: Small set of primitive constructs combined in a limited number of ways, each combination is legal.

## Writability
- Simplicity and Orthogonality: Few constructs, small number of primitives, simple rules for combination.

## Reliability
- Type checking: Testing for type errors

## Cost Factors
- Training programmers
- Writing programs
- Compiling and executing programs
- Availability of free compilers
- Maintaining programs
- Other criteria: Portability, Generality, Well-definedness

## Von Neumann Architecture
- Imperative languages dominant
- Data and programs stored in memory
- CPU fetches and executes instructions from memory

## Programming Methodologies Evolution
- 1950s-1960s: Machine efficiency
- Late 1960s: Readability, structured programming, top-down design
- Late 1970s: Data abstraction
- Mid-1980s: Object-oriented programming (data abstraction + inheritance + polymorphism)

## Language Categories
- Imperative: Variables, assignment statements, iteration (e.g., C, Java)
- Functional: Functions as primary computation (e.g., LISP, Scheme)
- Logic: Rule-based (e.g., Prolog)
- Markup/Hybrid: JSTL, XSLT

## Language Design Trade-offs
- Reliability vs. Cost of execution
- Readability vs. Writability
- Writability vs. Reliability

## Implementation Methods
- Compilation: Source language to machine language (slow translation, fast execution)
- Pure Interpretation: Interpreter runs the program (slow execution)
- Hybrid Implementation: Combination of compilation and interpretation (e.g., Java bytecode, .NET JIT)

## Data Aggregation
- Lists: Mutable, ordered, indexed by number
- Tuples: Immutable, ordered, indexed by number
- Dictionaries: Mutable, unordered, indexed by keys

## Key Python Constructs
- Variables: Named storage
- Loops: while, for
- Conditional statements: if, elif, else
- Functions: def keyword, pass by value/reference
- Indentation: Enforced for readability and structure

## Functions
- Define using def
- Return values using return
- Pass by value: Copy of the value is passed
- Pass by reference: Reference to the original value is passed

## Common Data Aggregates
- Lists: Mutable sequence, indexed by numbers
- Tuples: Immutable sequence, indexed by numbers
- Dictionaries: Mutable mapping, indexed by keys

## Example Usage
- Lists: cats = ['Tom', 'Snappy']
- Tuples: months = ('January', 'February')
- Dictionaries: phonebook = {'Alice': 12345}

## Advanced Topics
- Preprocessors: Expand macros before compilation
- Just-in-Time (JIT) Compilation: Intermediate language compiled at runtime

## Higher-Order Functions
Definition: A function that takes another function as a parameter or returns a function as a return value.
Examples:
- map()
- filter()
- reduce()

## Python Basics
### Creating and Running Python Scripts:
- Use ‘nano (yourfilename).py’ to create a file.
### Example:
-  def square(n):
- return n * n
- ilist = [2, 4, 6]
- olist = map(square, ilist)
- print(list(olist))
- Save and exit: ‘Ctrl+X’, ‘Y’, ‘Enter’
- Run: ‘python (yourfilename).py’
- Create and change directories:
- ‘mkdir (directoryname)’
- ‘cd (directoryname)’

## Lambda Expressions and Conditional Statements
### Lambda Expressions:
### Example:
- x = lambda a: a + 10
- print(x(5))  # Output: 15
### Conditional Statements:
### Example:
- raining = False
- print("Let's go to the", 'beach' if not raining else 'library')  # Output: Let's go to the beach
- raining = True
- print("Let's go to the", 'beach' if not raining else 'library')  # Output: Let's go to the library
- age = 12
- s = 'minor' if age < 21 else 'adult'
- print(s)  # Output: minor
- result = 'yes' if ('qux' in ['foo', 'bar', 'baz']) else 'no'
- print(result)  # Output: no

## Syntax and Semantics
### Definitions:
- Syntax: The form or structure of expressions, statements, and program units.
- Semantics: The meaning of expressions, statements, and program units.
### Language Definition Users:
- Language designers
- Implementers
- Programmers
### Key Concepts:
- Sentence: A string of characters over an alphabet.
- Language: A set of sentences.
- Lexeme: The lowest level syntactic unit (e.g., *, sum, begin).
- Token: A category of lexemes (e.g., identifier).
- BNF (Backus-Naur Form):
- Describes syntax using context-free grammars.
- BNF Rule Example:
- <ident_list> → identifier | identifier, <ident_list>
- <if_stmt> → if <logic_expr> then <stmt>

## Operational, Denotational, and Axiomatic Semantics
### Operational Semantics:
- Defines the meaning by executing statements on a machine.
- Needs a virtual machine for high-level languages.
### Denotational Semantics:
- Uses mathematical objects and functions to define meaning.
### Axiomatic Semantics:
- Uses formal logic to define semantics.
### Assertions:
- Precondition: Before a statement.
- Postcondition: After a statement.
- Weakest Precondition: Least restrictive condition ensuring the postcondition.

## Loop Invariants
### Definition: An assertion that is true before and after each iteration of a loop.
### Requirements:
- True initially before the loop.
- Maintained true during loop execution.
- Ensures postcondition upon loop termination.

## Syntax Analysis
### Components:
- Lexical Analyzer: Matches character patterns to tokens.
- Syntax Analyzer (Parser): Builds the parse tree.
### Parsing Techniques:
- Top-Down Parsing:
- Starts from the root and works down.
- Example methods: Recursive descent, LL parsers.
- Bottom-Up Parsing:
- Starts from the leaves and works up.
- Example: LR parsing.

## Quiz Notes
### Implementation Types:
- Interpretation: Translates source code during execution (Portability).
- Compilation: Translates source code to native language before execution (Speed).
### Data Aggregates:
- Homogeneous: Elements of the same type.
- Heterogeneous: Elements of different types.
- Addressing:
- By Number: Integer addressing.
- By Name: String addressing.
- Size:
- Fixed: Size cannot change.
- Dynamic: Size can change.
### Key Terms:
- Semantics: Meaning of program units.
- Lexeme: Lowest level unit of a language.
- Syntax: Form or structure of program units.
- Token: Category of lexemes.
