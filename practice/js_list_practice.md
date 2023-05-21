# javascript list practice

```jsx
const participantNums =  [[1, 3, 2, 2, 1], 
[3, 7, 100, 21, 13, 6, 5, 7, 5, 6, 3, 13, 21],
[9, 1, 8, 7, 71, 33, 62, 35, 11, 4, 7, 71, 33, 8, 9, 1, 4, 11, 35]
]

const Num = function (participantNum) {
    for (let i=0; i<participantNum.length; i++) {
        if (participantNum.slice(i+1, participantNum.length).includes(participantNum[i]) === false) {
            console.log(participantNum[i])
            break
        }
    }
}

for (const participantNum of participantNums) {
    console.log(Num(participantNum))
}
// 3
// 100
// 62
```