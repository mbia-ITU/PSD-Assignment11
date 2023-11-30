# Assignment 11

## 12.1

add addIFZERO, to Contcomp.fs.

## 12.2

Move boolean comparison with constants, from run-time to compile-time.

To check that our upgrade has worked, we ran the compiler on the following inputs.

`if (11 == 22) {print 33;} else { print 44;}`
Generates:
`[LDARGS; CALL (1, "L1"); STOP; Label "L1"; Label "L2"; CSTI 44; PRINTI;RET 1]`

and

`print 100 != 10;`

Generates:

`[LDARGS; CALL (1, "L1"); STOP; Label "L1"; CSTI 1; PRINTI; RET 1]`

On both, we see that the integer literals are not included in the code, only the result of the boolean expressions.

## 12.3

Add trinary statements to micro-C. And make the bool comparison at compile-time.

## 12.4

Upgrade boolean conditions AND and OR, to use the above trinary statements.

Changed the semantic action of `SEQAND`, and `SEQOR`, to use Cond, and not the purpose build Andalso or Orelse.
