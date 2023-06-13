# js todolist 2

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
  <!-- <input type="text" id="input_text"> -->
  <!-- <input type="submit" value="add" id="input_submit"> -->
  
  <script>
    const Inpt = document.createElement('input')
    Inpt.setAttribute('type', 'text')
    Inpt.setAttribute('id', 'input_text')
    const Inps = document.createElement('input')
    Inps.setAttribute('type', 'submit')
    Inps.setAttribute('value', 'add')
    Inps.setAttribute('id', 'input_submit')
    document.body.appendChild(Inpt)
    document.body.appendChild(Inps)

    const UL = document.createElement('ul')
    document.body.appendChild(UL)

    Inps.addEventListener('click', function () {
      if (Inpt.value == "") {
        alert('You have to input any text :(')
        Inpt.value = ""
      } else {
        const li = document.createElement('li')
        li.innerText = '' + Inpt.value
        UL.appendChild(li)
        Inpt.value = ""
      }
    })
 

  </script>  
</body>
</html>
```