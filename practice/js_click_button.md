# js click button

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <style>
    section {
      height: 50vh;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .myInputs {
      display: block;
      outline: none;
      width: 200px;
      margin: 15px;
      padding: 15px 10px;
      text-align: center;
      border: 2px solid black;
      border-radius: 5px;
    }
 
    .myInputs:focus {
      /* focus 발생시 변경될 속성 */
      border-color: green;
    }

    .myButton{
      display: block;
      background: none;
      outline: none;
      margin: 15px auto;
      padding: 10px 10px;
      text-align: center;
      border: 2px solid #55b2cf;
      border-radius: 5px;
      cursor: pointer;
      transition: 0.5s;
    }

    .myButton:hover {
      color: white;
      background-color: #55b2cf;
    }

  </style>
</head>
<body>
  <section>
    <div>
      <input class="myInputs" type="text" placeholder="Where to input" id="input">
      <button class="myButton" id="button">Check Input</button>
    </div>
  </section>
  
  <script>
    const InP = document.querySelector('#input')
    const Btn = document.querySelector('#button')

    Btn.addEventListener('click', function(event) {
      if (InP.value == 'I have a exam today') {
        alert('You are the best!! Good Luck :)')
      } else {
        alert('try again :)')
      }
    })

  </script>
</body>
</html>
```