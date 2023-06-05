# js_change_color_switch

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Document</title>
</head>
<body>
  <ul class="switcher">
    <li id="grayButton"></li>
    <li id="whiteButton"></li>
    <li id="navyButton"></li>
  </ul>
  
  <h1>Theme Switcher</h1>
  
  <p>테마를 바꿔봅시다.</p>

  <script>

 
    const grayBtn = document.querySelector('#grayButton')
    const whiteBtn = document.querySelector('#whiteButton')
    const navyBtn = document.querySelector('#navyButton')
    const body = document.querySelector('body')

    // 1. li#grayButton 클릭시 background-color는 gray, color는 white로 변경
    grayBtn.addEventListener('click', () => {
      body.style.backgroundColor = 'gray'
      body.style.color = 'white'
    })

    // 2. li#whiteButton 클릭시 background-color는 white, color는 black으로 변경
    whiteBtn.addEventListener('click', () => {
      body.style.backgroundColor = 'white'
      body.style.color = 'black'
    })

    // 3. li#navyButton 클릭시 background-color는 navy, color는 white로 변경
    navyBtn.addEventListener('click', () => {
      body.style.backgroundColor = 'navy'
      body.style.color = 'white'
    }) 

  
  </script>
</body>
</html>
```