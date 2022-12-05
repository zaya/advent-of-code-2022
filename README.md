# aoc-kotlin-template

Template for solving the [advent-of-code](https://adventofcode.com/) puzzles with Kotlin 

## How to get the most out of this template

### Preparation

1. Install [just](https://just.systems)
2. Log-in on https://adventofcode.com/
3. Inspect your cookies and copy content of the `AOC_SESSION` cookie
4. Export an `AOC_SESSION` environment variable with the content of the `AOC_COOKIE`


### Each day

*(replace `$DAY` by the current day of the month)*

1. get your personal puzzle input with `just day=$DAY get-input`
2. start the tests with `just day=$DAY watch"`
   (it'll automatically rerun the tests when the source change)
3. Write your tests in `src/test/kotlin/Day${DAY}Test`
4. Solve the puzzle in `src/main/kotlin/Day${DAY}`
5. Once you think you're done, enable the test `should return expected output for the puzzle input` and watch it fail.
   The failure message contains your puzzle answer.
6. If your answer is correct, write it as the expected value for that test. (so that all the test pass)
7. Refactor as you please
