# javascript new star

```jsx
for (i=1; i<6; i++) {
    string = '*'
    new_string = string.repeat(2*i - 1)
    add_string = ' '
    added_string = add_string.repeat(5-i)
    answer = added_string + new_string
    console.log(answer)
}
```

```jsx
     *
    ***
   *****
  *******
 *********
```