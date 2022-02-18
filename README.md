# Arithmetic-Evaluator

Arithmetic expression evaluator. 

This program interactively receives instructions.

## Execution

Run `cabal run` and interact with main program.

Possible commands are:
* `EVAL <order> <expr>` 
    - `<order>` is one of `PRE` or `POST` indicating preorder or post order evaluation respectively
    - `<expr>` is a well formed arithmetic expression in the indicated `<order>`. Valid operations are `+`,`-`,`*`,`/`.
    The result of this command is the evaluation of the given expression, or an error if the expression is malformed.
* `MOSTRAR <orden> <expr>`: Displays an *infix notation* expression provided a preorder or postorder expression using the same rules as above.
* `SALIR`: exit program.

## Running instructions

To run testcases use:

```bash
cabal clean
cabal configure --enable-tests --enable-coverage`
```

and then run: `cabal test`

---

Coverage tests information is under:

`dist/hpc/vanilla/eval-test/*`
