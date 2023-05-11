# javascript palindrome

```jsx
words = ['level', 'noon', 'mom', 'happy', 'naver', 'life']

function palindrome(word) {
  let word_reverse = ''

  for (let i = word.length-1; i>-1; i--){
    word_reverse += word[i]
  }
  // console.log(word_reverse)

  if (word === word_reverse) {
    return true
  }
  else {
    return false
  }
    // word가 회문인지 아닌지 판별
  }
  
for (const word of words) {
  console.log(palindrome(word))
}

// 출력 예시
// true
// true
// true
// false
// false
// false
```