# js_axios_cat&dog

- 야옹이 사진 불러오기

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

  <button>야옹아 이리온</button>

  <script src="https://cdn.jsdelivr.net/npm/axios/dist/axios.min.js"></script>
  <script>
      console.log('고양이는 야옹')
      const catImageSearchURL = 'https://api.thecatapi.com/v1/images/search'
      const btn = document.querySelector('button')
      btn.addEventListener('click', function() {
        axios.get(catImageSearchURL)
          .then((response) => {
            // console.log(response.data)
            console.log(response.data[0].url)
            imgElem = document.createElement('img')
            imgElem.setAttribute('src', response.data[0].url)
            document.body.appendChild(imgElem)
            
          })
          .catch((error) => {
            console.log('실패했다옹')
          })
  
        console.log('야옹야옹')
      })

  </script>
  
</body>
</html>
```

- 야옹이 연습 더하기

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
  <div id="cat-container"></div>
  <button id="cat_get_button">hello!! cat</button>
  <script src="https://cdn.jsdelivr.net/npm/axios/dist/axios.min.js"></script>
  <script>
    const catSearchUrl = "https://api.thecatapi.com/v1/images/search"
    const catButton = document.querySelector("#cat_get_button")

    catButton.addEventListener('click', () => {
      axios({
        method: 'get',
        url: catSearchUrl,

      })
      .then(response => {
        console.log(response)
        return response.data
      })
      .then(responseBody => {
        console.log(responseBody)
        console.log(responseBody[0].url)
        const catImgElem = document.createElement('img')
        catImgElem.setAttribute('src', responseBody[0].url)

        const catContainer = document.querySelector('#cat-container')
        catContainer.childNodes.forEach(element => element.remove())
        catContainer.appendChild(catImgElem)
      })
      .catch(error => {
        console.log(error)
      })
    })
  </script>
  
</body>
</html>
```

- 멍뭉이 불러오기

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
  <button>hello Doggy!!</button>
  <script src="https://cdn.jsdelivr.net/npm/axios/dist/axios.min.js"></script>
  <script>
    const dogImageSearchURL = "https://dog.ceo/api/breeds/image/random"
    const dogBtn = document.querySelector('button')
    dogBtn.addEventListener('click', function() {
      axios({
        method: 'get',
        url: dogImageSearchURL
      })
      .then((response) => {
        const imgSrc = response.data.message
        return imgSrc
        
      })
      .then((imgSrc) => {
        const imgTag = document.createElement('img')
        imgTag.setAttribute('src', imgSrc)
        document.body.appendChild(imgTag)
      })
      .catch((error) => {
        console.log(error)
      })
    })
  </script>
</body>
</html>
```