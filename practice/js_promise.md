# js promise

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
    
    console.log('Hi')
    const myPromise = new Promise((resolve, reject)=>{

      setTimeout(function () {
        resolve(console.log('My name is Ryu'))
      }, 2000)

    })
    myPromise.then((message) =>{
      console.log('Bye')
    })

  </script>
</body>
</html>
```