# js button

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  <script>

    const button = document.createElement('button')
    const in_text = document.createTextNode('출력 로그')
    button.appendChild(in_text)
    document.body.append(button)

    button.addEventListener('click', function(event) {
      console.log('버튼을 클릭했어요!!')
      const printOut = document.createElement('p')
      const node = document.createTextNode('버튼을 클릭했어요!!!!!!!!!!')
      printOut.appendChild(node)
      document.body.append(printOut)
    })
// 버튼 혹은 p, a등 다양한 테그를 console로 만드는 연습이 더 필요하겠다..

  </script>
</body>
</html>
```