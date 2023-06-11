# js todolist

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<ul>

</ul>
<body>
  <script>
    const head = document.createElement('h1')
    head.innerText = 'Today TodoList'
    document.body.appendChild(head)

    const ulbox = document.createElement('ul')
    console.log(ulbox)
    const li1 = document.createElement('li')
    li1.innerText = 'do homework'
    ulbox.appendChild(li1)
    const li2 = document.createElement('li')
    li2.innerText ='study'
    ulbox.appendChild(li2)
    const li3 = document.createElement('li')
    li3.innerText = 'take a rest'
    ulbox.appendChild(li3)
    document.body.appendChild(ulbox)

  </script>
</body>
</html>
```