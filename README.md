# Azureresume
My azure resume (Written in mark down language)

-Frontend contains folder contains the website

-main.js contains the visitor counter

-meabdirahman contains my picture

-Project inspiration came from A Cloud Guru

-The file called Main.js, whuch can be found in under the frontend folder contains the visitor counter 

```js
const getVisitCount = () => {
    let count = 30;
    fetch(functionApi)
    .then(response => {
        return response.json()
    })
    .then(response => {
        console.log("Website called function API.");
        count = response.count;
        document.getElementById('counter').innerText = count;
    }).catch(function(error) {
        console.log(error);
      });
    return count;
}
```

-CI/CD workflow with Github. 

First command
```js
git add -A
```

Second command, followed by a message under the 
```js
git commit -m "Message inserted here"
```

Third command
```js
git push
```

