# ui-regression-testing

Different ways to test UI regression

## Using Backstop to detect regression in UI

Here is a sample diff from failed test after `border-radius` value has been changed:

![image](https://user-images.githubusercontent.com/14539/30296125-5f7be58a-9743-11e7-9dba-4c59183e8c9c.png)

Depending on configuration settings if a change ratio is within treshold set for tests `Backstop` will throw errors in tests:

```bash
      COMMAND | Command `report` ended with an error after [1.375s]
      COMMAND | Error: Mismatch errors found.
                    at /Users/piotrblazejewicz/git/ui-regression-testing/node_modules/backstopjs/core/command/report.js:113:17
                    at <anonymous>
                    at process._tickCallback (internal/process/next_tick.js:188:7)
      COMMAND | Command `test` ended with an error after [5.284s]
      COMMAND | Error: Mismatch errors found.
                    at /Users/piotrblazejewicz/git/ui-regression-testing/node_modules/backstopjs/core/command/report.js:113:17
                    at <anonymous>
                    at process._tickCallback (internal/process/next_tick.js:188:7)
error Command failed with exit code 1.
```

## Author

@peterblazejewicz
