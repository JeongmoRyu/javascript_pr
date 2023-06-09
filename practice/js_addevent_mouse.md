# js_addevent_mouse

- mouseenter, mousedown, mousemove, mouseout, mouseover, mouseup, mousewheel 등등 다양한 event가 있으니 찾아보자

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">
</head>
<body>
  <button class="btn btn-primary mt-2 ms-2" id="button">마우스를 올려보세요</button>
  <button class="btn btn-primary mt-2 ms-2" id="button1">마우스를 클릭을 해제할 때 보세요</button>
  <button class="btn btn-primary mt-2 ms-2" id="button2">마우스를 여기서 벗어나보세요</button>

  <script>
    // 이곳에 코드를 작성합니다
    const Btn = document.getElementById('button')
    const Btn1 = document.getElementById('button1')
    const Btn2 = document.getElementById('button2')

    Btn.addEventListener('mouseover', function () {
      alert('mouse over!!')
    })
    Btn1.addEventListener('mouseup', function () {
      alert('mouse up!!')
    })
    Btn2.addEventListener('mouseleave', function () {
      alert('mouse leave!!')
    })
// mouseenter, mousedown, mousemove, mouseout,
// mouseover, mouseup, mousewheel 등등 다양한 event가 있으니 찾아보자
  </script>
</body>
</html>
```