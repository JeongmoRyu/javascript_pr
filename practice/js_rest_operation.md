# js rest operation

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Document</title>
</head>
<body>
  <script>

    const myFile = {
      name: 'profile',
      extension: 'jpg',
      size: 20000
    }
    function fileSummary(file) {
        console.log(`The file ${file.name}.${file.extension} is size of ${file.size} bytes.`)
    }
    fileSummary(myFile)


    const data = {
      username: 'myName',
      password: 'myPassword',
      email: 'my@mail.com',
    }

    const username = data.username
    const password = data.password
    const email = data.email
    
    function Data(data) {
      console.log(`I typed my username, password and email as ${username} ${password} and ${email}`)
    }
    Data(data)


    function addNumbers(a,b,c,d,e) {
      const numbers = [a, b, c, d, e];
      return numbers.reduce((sum, number) => { 
        return sum + number
      }, 0)
    }
    const Num = addNumbers(1, 2, 3, 4, 5)
    console.log(Num)
    

    const defaultColors = ['red', 'green', 'blue'];
    const favoriteColors = ['navy', 'black', 'gold', 'white']
    const palette = defaultColors.concat(favoriteColors);
    console.log(palette)
    // concat 리스트 합치기

    const info1 = { name: 'Ryu', age: 30 }
    const info2 = { isMarried: true, balance: 300000 }
    const fullInfo = Object.assign(info1, info2)
    console.log(fullInfo)
    // 리스트를 합칠 때 객체가 같은 속성을 가질 때 더 뒤 순위에 위치한 객체의 값으로 덮어쓴다.
  </script>
</body>
</html>
```