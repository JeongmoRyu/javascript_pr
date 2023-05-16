# javascript electric bus swea

16127

```jsx
const inputs = [
		[3, 10, 5, [1, 3, 5, 7, 9]],    // 3
	  [3, 10, 5, [1, 3, 7, 8, 9]],    // 0
	  [5, 20, 5, [4, 7, 9, 14, 17]],  // 4
]

 function solution(K, N, M, chargers) {
    let here = 0
    let station = 0
    let count = 0
    let i = 0

 while (here < N) {
      here = station + K - i
      i += 1

      if (here === station) {
          count = 0
          break
      }
      else if (chargers.includes(here) === true) {
          station = here
          i = 0
          count += 1
      }
	  }
    console.log(`# ${count}`)

}
   
for (const input of inputs) {
    solution(input[0], input[1], input[2], input[3])
} 
		
```

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Document</title>
</head>
<body>
  
  <script>
    // 이곳에 코드를 작성합니다.
		const inputs = [
    [3, 10, 5, [1, 3, 5, 7, 9]],    // 3
    [3, 10, 5, [1, 3, 7, 8, 9]],    // 0
    [5, 20, 5, [4, 7, 9, 14, 17]],  // 4
    ]

    function solution(K, N, M, chargers) {
      let here = 0
      let station = 0
      let count = 0
      let i = 0

      while (here < N) {
          here = station + K - i
          i += 1

          if (here === station) {
              count = 0
              break
          }
          else if (chargers.includes(here) === true) {
              station = here
              i = 0
              count += 1
          }
        }
      console.log(`# ${count}`)

    }
   
    for (const input of inputs) {
      solution(input[0], input[1], input[2], input[3])
    }    // 이곳에 코드를 작성합니다.
		const inputs = [
    [3, 10, 5, [1, 3, 5, 7, 9]],    // 3
    [3, 10, 5, [1, 3, 7, 8, 9]],    // 0
    [5, 20, 5, [4, 7, 9, 14, 17]],  // 4
    ]

    function solution(K, N, M, chargers) {
      let here = 0
      let station = 0
      let count = 0
      let i = 0

      while (here < N) {
          here = station + K - i
          i += 1

          if (here === station) {
              count = 0
              break
          }
          else if (chargers.includes(here) === true) {
              station = here
              i = 0
              count += 1
          }
        }
      console.log(`# ${count}`)

    }
   
    for (const input of inputs) {
      solution(input[0], input[1], input[2], input[3])
    }

  </script>
</body>
</html>
```