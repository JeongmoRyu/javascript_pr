# js snake game

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Document</title>
</head>
<body>
  <script>

    
    // 아래에 Monster 와 Snake class를 생성합니다.
    class Monster {
      constructor(snakename) {
        this.name = snakename
        this.health = 100
      }
    }
    class Snake extends Monster{
      constructor(snakename, health) {
        super(snakename) 
      }
      bite(another) {
      return another.health -= 10
    }
    }

    // 아래 코드는 확인용 입니다.
    const conda = new Snake({ name: 'anaconda' })
    const boa = new Snake({ name: 'boaconda' })

    console.log(anaconda.health)  // 100
    boaconda.bite(anaconda)
    console.log(anaconda.health)  // 90

  </script>
</body>
</html>
```