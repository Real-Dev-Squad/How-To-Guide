# Tasks

Anytime a new task is assigned, it will be in a new repo on the `master` branch

- Fork the repo under your account
- Branch and checkout into a `develop` branch
- Work on the solution, use a couple of branches under the Git Flow conventions
- Ask any queries using issues on the *original task repo* with proper links and enough details
- Once you have your working solution, send a Pull Request from your `develop`, to be merged into the branch having name `solution/<your name>`


# Solution Complexity

Your solution should contain the following information in the `README.md`: 

- Time complexity of your solution. Mention what the different variables mean properly
- Space complexity

Addition details:
- Small snippets of code that create a complexity. E.g link to the line in code, small snippet of where a forEach loop might exist etc


## Example:

Task: Add the numbers in the given array

README Section:

### Time Complexity

`O(L)` : Where L is the length of the array (number of array elements)

### Space Complexity

`O(1)` : Constant time


### Crtical Parts / Bottleneck:

```js
const arrSum = arr.reduce((acc, curr) => (acc + curr));
```
The reduce function loop is where the main complexity comes from. It runs as many times as there are elements in the array(actually one less, since reduce starts from first element in accumulator in this case, but L-1 ~ L, considering L is a huge number)
