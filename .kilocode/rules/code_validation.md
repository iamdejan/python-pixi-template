# Code Validation

Hi Kilo Code agent! Whatever model you are using, make sure you validate the code you generated.

## Steps to Validate

Run these commands in sequence:
1. `pixi run lint-ci`: ensure no linter errors.
2. `pixi run lint-fix`: if there is any linter error, fix it with this command.
3. `pixi run lint-ci`: recheck again, maybe there are linter errors that need manual fix.
4. `pixi run type-check`: ensure no type errors.
5. `pixi run test`: build the code, then run all unit tests. This ensures that the code you generate pass all the unit tests.
