# javascript practice 1

- for 문 연습해보기

```jsx

const nums = [1,2,3,4,5,6,7,8]

for (let i = 0; i < nums.length; i++) {
  console.log('nums[' + i + ']: ' + nums[i])
}

//nums[0]: 1
//nums[1]: 2
//nums[2]: 3
//nums[3]: 4
//nums[4]: 5
//nums[5]: 6
//nums[6]: 7
//nums[7]: 8

```

```jsx
const nums = [1,2,3,4,5,6,7,8]

for (num in nums) {
  console.log(num, typeof Number(num))
}
// 앞의 num을 Number 해준다면 'number'로 표현된다.

// 0 string
// 1 string
// 2 string
// 3 string
// 4 string
// 5 string
// 6 string
// 7 string
```