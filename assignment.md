# Assignment 11

## 12.1

add addIFZERO, to Contcomp.fs.

## 12.2

Move boolean comparison with constants, from run-time to compile-time.

if (11 == 22) {print 33;} else { print 44;}

Generates:

[LDARGS; CALL (1, "L1"); STOP; Label "L1"; Label "L2"; CSTI 44; PRINTI;RET 1]

print 100 != 10;

Generates: 

 [LDARGS; CALL (1, "L1"); STOP; Label "L1"; CSTI 1; PRINTI; RET 1]

## 12.3

Add trinary statements to micro-C. And make the bool comparison at compile-time.

## 12.4

Upgrade boolean conditions AND and OR, to use the above trinary statements.

