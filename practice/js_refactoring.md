# javascript refactoring

```jsx

    /* 
      1. 해당 코드를 template string 을 활용하여 리팩토링하시오.
      2. 해당 코드를 arrow function 으로 리팩토링하시오.
      3. 해당 코드의 메서드 introduce 를 function 키워드 없이 리팩토링하시오.
      4. 해당 코드를 key, value를 한번씩만 작성하도록 리팩토링하시오.
    */

    // 1
    const name = 'Tom'
    console.log('Hi, my name is' + name)
    // template string 활용
    console.log(`Hi, my name is ${name}`)

    
    // 2 - 확인차 x, y를 정해주고 console.log 해주면서 비교해주었다.
    x = 3
    y = 5
    function add(x, y) {
      return x + y
    }
    console.log(add(x, y))
    // arrow function 활용
    const add1 = (x, y) => `${x + y}`
    console.log(add1(x, y))
    

    // 3 - console.log 해주면서 비교해주었다.
    const tom = {
      name: 'Tom',
      introduce: function () {
        console.log('Hi, my name is' + this.name)
      }
    }
    tom.introduce()

    // introduce를 function 키워드 없이 리펙토링
    const tomy = {
      name1 : 'Tomy',
      introduce1() {
        console.log(`Hi, my name is ${this.name1}`)
      }
    }
    tomy.introduce1()
    // console.log(tomy.map(introduce1 => introduce1))

    // 4
    const url = 'https://test.com'
    const data = { message: 'Hello World!' }

    const request = { url: url, data: data }
    console.log(request)
    // console.log(request.url, request.data.message)
    // 값들을 확인하는 방법

    // key, value를 한번씩만 작성하도록 리팩토링
  
    const request1 = {url1: url, data1:data }
    const {url1, data1} = request1
    console.log(request1)

```