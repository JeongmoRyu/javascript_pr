# js_n_queen

```jsx
function findQueens(n) {
  let answer = 0
  const dfs = (board, row) => {
    if (row === n) {
      answer ++
    } else {
      for (let i = 1; i <= n; i++) {
        board[row + 1] = i
        if (Check(board, row+1)) {
          dfs(board, row+1)
        }
      }
    }
  }
  const Check = (board, row) => {
    for (let i=1; i < row; i++) {
      if (board[i]=== board[row]) {
        return false
      }
      if (Math.abs(board[i]-board[row]) === Math.abs(i-row)){ 
	  // Math.abs 절대값	
        return false
      }
    }
    return true
  }
  for (let i=1; i <=n; i++) {
    const board = new Array(n+1).fill(0)
	    // 생성자 new Array()

    board[1] = i
    dfs(board, 1)
  }
  return answer
}

for (let k = 0; k<10; k ++) {
  console.log(`${k} : ${findQueens(k)}`)
}

// 0 : 0
// 1 : 1
// 2 : 0
// 3 : 0
// 4 : 2
// 5 : 10
// 6 : 4
// 7 : 40
// 8 : 92
// 9 : 352
```