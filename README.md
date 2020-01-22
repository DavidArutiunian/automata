# Lexer4J

![GitHub top language](https://img.shields.io/github/languages/top/DavidArutiunian/lexer4j.svg)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/DavidArutiunian/lexer4j.svg)
![GitHub last commit](https://img.shields.io/github/last-commit/DavidArutiunian/lexer4j.svg)
[![TLOC](https://tokei.rs/b1/github/DavidArutiunian/lexer4j)](https://github.com/DavidArutiunian/lexer4j)


## Getting Started

### 📃 Create an input file with some code

You can find code example in `test/test.txt`

```bash
$ cat test/test.txt > input.txt
```

Or you can link the test file

Linux:
```bash
$ ln -s test/test.txt input.txt
```

Windows:
```cmd
$ mklink input.txt test/test.txt
```

### 🚀 Run lexer

Pass the file with code to lexer

```bash
$ java -jar lexer.jar input.txt
```

You should get something like this

```
CLASS 'class' [L1:0]
IDENTIFIER 'Foo' [L1:6]
OPENING_CURLY_BRACE '{' [L1:10]
PRIVATE 'private' [L2:16]
DOUBLE 'double' [L2:24]
IDENTIFIER 'big' [L2:31]
ASSIGNMENT '=' [L2:35]
SCIENTIFIC_LITERAL '3.2e+23' [L2:37]
SEMICOLON ';' [L2:44]
PRIVATE 'private' [L3:76]
DOUBLE 'double' [L3:84]
IDENTIFIER 'small' [L3:91]
ASSIGNMENT '=' [L3:97]
SUBTRACTION '-' [L3:99]
SCIENTIFIC_LITERAL '4.70e-9' [L3:100]
SEMICOLON ';' [L3:107]
PRIVATE 'private' [L5:142]
IDENTIFIER 'String' [L5:150]
IDENTIFIER 'message' [L5:157]
ASSIGNMENT '=' [L5:165]
STRING_LITERAL '"Foo >> "' [L5:167]
SEMICOLON ';' [L5:176]
PRIVATE 'private' [L6:182]
IDENTIFIER 'char' [L6:190]
IDENTIFIER 'newline' [L6:195]
ASSIGNMENT '=' [L6:203]
CHAR_LITERAL ''\n'' [L6:205]
SEMICOLON ';' [L6:209]
PRIVATE 'private' [L8:216]
INT 'int' [L8:224]
IDENTIFIER 'hex' [L8:228]
ASSIGNMENT '=' [L8:232]
HEX_LITERAL '0x0A0B0C' [L8:234]
SEMICOLON ';' [L8:242]
PRIVATE 'private' [L9:248]
INT 'int' [L9:256]
IDENTIFIER 'octal' [L9:260]
ASSIGNMENT '=' [L9:266]
OCTAL_LITERAL '0737' [L9:268]
SEMICOLON ';' [L9:272]
PRIVATE 'private' [L10:278]
INT 'int' [L10:286]
IDENTIFIER 'binary' [L10:290]
ASSIGNMENT '=' [L10:297]
BINARY_LITERAL '0b01001001110' [L10:299]
SEMICOLON ';' [L10:312]
PRIVATE 'private' [L12:319]
IDENTIFIER 'String' [L12:327]
IDENTIFIER 'multiline' [L12:334]
ASSIGNMENT '=' [L12:344]
MULTILINE_STRING_LITERAL '"""
        Hello, World!
        Who I am?
    """' [L12:346]
SEMICOLON ';' [L15:397]
PUBLIC 'public' [L21:471]
VOID 'void' [L21:478]
IDENTIFIER 'main' [L21:483]
OPENING_BRACE '(' [L21:487]
IDENTIFIER 'String' [L21:488]
OPENING_SQUARE_BRACE '[' [L21:494]
CLOSING_SQUARE_BRACE ']' [L21:495]
IDENTIFIER 'args' [L21:497]
CLOSING_BRACE ')' [L21:501]
OPENING_CURLY_BRACE '{' [L21:503]
INT 'int' [L22:513]
IDENTIFIER 'size' [L22:517]
ASSIGNMENT '=' [L22:522]
INT_LITERAL '3' [L22:524]
SEMICOLON ';' [L22:525]
INT 'int' [L23:535]
OPENING_SQUARE_BRACE '[' [L23:539]
IDENTIFIER 'size' [L23:540]
CLOSING_SQUARE_BRACE ']' [L23:544]
IDENTIFIER 'array' [L23:546]
ASSIGNMENT '=' [L23:552]
OPENING_CURLY_BRACE '{' [L23:554]
INT_LITERAL '1' [L23:556]
COMMA ',' [L23:557]
INT_LITERAL '2' [L23:559]
COMMA ',' [L23:560]
INT_LITERAL '3' [L23:562]
CLOSING_CURLY_BRACE '}' [L23:564]
SEMICOLON ';' [L23:565]
INT 'int' [L24:575]
IDENTIFIER 'index' [L24:579]
ASSIGNMENT '=' [L24:585]
INT_LITERAL '0' [L24:587]
SEMICOLON ';' [L24:588]
FLOAT 'float' [L25:598]
IDENTIFIER 'e' [L25:604]
ASSIGNMENT '=' [L25:606]
DOUBLE_LITERAL '2.73' [L25:608]
SEMICOLON ';' [L25:612]
WHILE 'while' [L26:622]
OPENING_BRACE '(' [L26:628]
IDENTIFIER 'index' [L26:629]
NOT_EQUALS '!=' [L26:635]
INT_LITERAL '0' [L26:638]
CLOSING_BRACE ')' [L26:639]
OPENING_CURLY_BRACE '{' [L26:641]
IDENTIFIER 'index' [L27:655]
ASSIGNMENT '=' [L27:661]
IDENTIFIER 'index' [L27:663]
SUBTRACTION '-' [L27:669]
INT_LITERAL '1' [L27:671]
SEMICOLON ';' [L27:672]
IDENTIFIER 'var' [L28:686]
IDENTIFIER 'coefficient' [L28:690]
ASSIGNMENT '=' [L28:702]
IDENTIFIER 'big' [L28:704]
MULTIPLICATION '*' [L28:708]
IDENTIFIER 'small' [L28:710]
DIVISION '/' [L28:716]
IDENTIFIER 'hex' [L28:718]
SEMICOLON ';' [L28:721]
IDENTIFIER 'println' [L29:735]
OPENING_BRACE '(' [L29:742]
IDENTIFIER 'message' [L29:743]
COMMA ',' [L29:750]
IDENTIFIER 'array' [L29:752]
OPENING_SQUARE_BRACE '[' [L29:757]
IDENTIFIER 'index' [L29:758]
CLOSING_SQUARE_BRACE ']' [L29:763]
MULTIPLICATION '*' [L29:765]
IDENTIFIER 'coefficient' [L29:767]
COMMA ',' [L29:778]
IDENTIFIER 'newline' [L29:780]
CLOSING_BRACE ')' [L29:787]
SEMICOLON ';' [L29:788]
CLOSING_CURLY_BRACE '}' [L30:798]
FOR 'for' [L31:808]
OPENING_BRACE '(' [L31:812]
IDENTIFIER 'var' [L31:813]
IDENTIFIER 'num' [L31:817]
COLON ':' [L31:821]
IDENTIFIER 'array' [L31:823]
CLOSING_BRACE ')' [L31:828]
OPENING_CURLY_BRACE '{' [L31:830]
IDENTIFIER 'var' [L32:844]
IDENTIFIER 'coefficient' [L32:848]
ASSIGNMENT '=' [L32:860]
IDENTIFIER 'big' [L32:862]
MULTIPLICATION '*' [L32:866]
IDENTIFIER 'small' [L32:868]
DIVISION '/' [L32:874]
IDENTIFIER 'hex' [L32:876]
SEMICOLON ';' [L32:879]
IDENTIFIER 'println' [L33:893]
OPENING_BRACE '(' [L33:900]
IDENTIFIER 'message' [L33:901]
COMMA ',' [L33:908]
IDENTIFIER 'num' [L33:910]
MULTIPLICATION '*' [L33:914]
IDENTIFIER 'coefficient' [L33:916]
COMMA ',' [L33:927]
IDENTIFIER 'newline' [L33:929]
CLOSING_BRACE ')' [L33:936]
SEMICOLON ';' [L33:937]
CLOSING_CURLY_BRACE '}' [L34:947]
IDENTIFIER 'var' [L35:957]
IDENTIFIER 'secret' [L35:961]
ASSIGNMENT '=' [L35:968]
IDENTIFIER 'hex' [L35:970]
XOR '^' [L35:974]
IDENTIFIER 'octal' [L35:976]
XOR '^' [L35:982]
IDENTIFIER 'binary' [L35:984]
SEMICOLON ';' [L35:990]
IDENTIFIER 'println' [L36:1000]
OPENING_BRACE '(' [L36:1007]
IDENTIFIER 'secret' [L36:1008]
CLOSING_BRACE ')' [L36:1014]
SEMICOLON ';' [L36:1015]
CLOSING_CURLY_BRACE '}' [L37:1021]
CLOSING_CURLY_BRACE '}' [L37:1023]
```
