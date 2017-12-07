# Congo

## About
A fully featured and lightweight unit testing framework, providing a decorator to compare arbitrary tuples and report on their identicality.

## Usage

Use the `@congo` decorator around any function that returns a tuple to be compared:

```
@congo
def pass_check:
    return('congo', 'congo')
```

`pass_check : Pass`

```
@congo
def fail_check:
    return('congo', 'red')
```

`fail_check : Fail`
