# Assignment 11

Solved by the group Recursive Rebels.

## Exercises

PLC: 12.1, 12.2, 12.3, 12.4.

## Run instructions

```{}
fslex --unicode <LexerSpecification>.fsl
fsyacc --module <ParserName> <ParserSpecification>.fsy
dotnet fsi -r FsLexYacc.Runtime.dll ...
```

On MacBook

```{}
mono ~/bin/fsharp/fslex.exe --unicode <LexerSpefication>.fsl
mono ~/bin/fsharp/fsyacc.exe --module <ParserName> <ParserSpecification>.fsy
dotnet fsi -r FsLexYacc.Runtime.dll ...
```

## Handin details

Handin file name:

- BPRD-11-AMDH-EMNO-MBIA.zip

Files to handin:

- assignment.md
