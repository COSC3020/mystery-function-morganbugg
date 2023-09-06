[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11753688&assignment_repo_type=AssignmentRepo)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```

Answer:
If the length of the input provided is 1, the function returns the value of the
single item. If not, it sets a new variable "foo" to a call of the mystery
function using all values of the input except the first and last values. Then
if foo evaluates to be greater than the first value in the input, the function
returns foo. Else the function returns the first value of the input. Through
this process, the function is finding the maximum value in the input.