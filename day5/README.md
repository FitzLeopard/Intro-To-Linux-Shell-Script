## Notes on Day 5

### A Built-in Variable

`UID` is a built-in variable. The `UID` of root user is always 0 throughout all the Linux systems.

### Conditional Statement

The format is

```bash
if [[ <condition> ]]
then
  <statements>
else
  <statements>
fi
```

- There exists a single-bracket form---`if [ <condition> ]` . But it is both old-fashion and risky. So use the double-bracket form.
- The space after the opening bracket and before closing brackets is crucial.