# Reverse Polish Notation Converter 
For this programming exercise, you will be creating a library which will allow the conversion of a mathematical expression in infix notation to reverse Polish notation (RPN) and visa versa. 

Once your solution is complete, please provide it as a Git repository (publicly available via Github or Bitbucket). Please include within your repository, all source and test code. Also, include a readme.md that describes the library API; how to build it; assumptions; a brief description of the exercise; and the strategy used to solve the problem. Do not include personally identifying information in the readme or comments so that we can anonymously review the solution.

## Infix Notation Rules: 

 * The placement of operators is between operands. For example: a+b
 * Parentheses, (), can be used to surround groups of operands and operators to indicate the intended order in which operations are to be performed.
 * The order of operation, when not overridden by parentheses, is described in the table below by descending order. For example, because division has higher precedence than multiplication, a*b/c is equivalent to a*(b/c).

## Precedence Name Operator 

 1. Exponent ^
 2. Division /
 3. Multiplication *
 4. Subtraction -
 5. Addition +

Operators with equal precedence associate from left to right. For example, a^b^c is
equivalent to (a^b)^c. 

It is not necessary to include the unary negation operator as part of this exercise. 

### Example: -b. 

Valid operands are only lowercase letters: a, b, ..., z 

#### RPN Notation Rules: 

* The operators follow their operands. For example: ab+
* Valid operators are ^, /, *, -, +
* Valid operands are only lowercase letters: a, b, ..., z 

This exercise is based on the ONP - Transform the Expression problem at http://www.spoj.com/problems/ONP/

### Examples: 

    1. Infix to RPN: a+b-c becomes abc-+
    2. Infix to RPN: (a+b)-c becomes ab+c-
    3. Infix to RPN: l/m^n*o-p and ((l/(m^n))*o)-p are equivalent expressions that become lmn^/o*p-
    4. Infix to RPN: ((v/w)^x)*(y-z) becomes vw/x^yz-*
    5. RPN to Infix: ag+ba-c+cedf^*+^* can become (a+g)*(((b-a)+c)^(c+(e*(d^f)))) 

The environment for this programming exercise ​ must​ use: 

    * Ubuntu Linux 14.04
    * The C programming language using the GNU GCC (c99) compiler tool chain
    * GNU Make (no automake nor cmake)
    * Check unit testing framework (See ​ https://libcheck.github.io/check/​ and pkg-config)
    * Git 

The solution will be reviewed for: 

    * Successfully building in ​ Ubuntu Linux 14.04​ without intervention.
    * Providing a test executable with successfully passing tests.
    * Application of Test Driven Development (TDD, see https://www.youtube.com/watch?v=7y7KJN5qWic​ )
    * Test coverage
    * Use of source control and commit frequency in support of TDD
    * Organized and understandable project and algorithm usage
    * Code structure, complexity, function length, single responsibility principle, code duplication
    * Code readability, variable/function names, self-documenting
    * Use of the C language and conventional constructs.
    * Solution completeness including error handling
    * Memory usage, memory leaks (Valgrind will be used to find leaks.) 