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

Cosmos DB

Create a Azure Cosmos DB account

- Create Azure Cosmos DB Account - Core (SQL)

- Choose serverless option in this case as it is cheaper, less configuration and can easily be turned off :) 

- Click Data Explorer tap on the left and choose to create a new container.
 
```js
Database id - Azureresume
Container id - Counter
Partition key - /id
```
Under counter is item, here will sql query be typed for visitor counter

```js
{
    "id": "1"
    "count": 0,
}
```
- Click safe

```js
Output : (should be similar to this)
{
    "id": "1",
    "count": 0,
    "_rid": "L9o3ANHa68cBAAAAAAAAAA==",
    "_self": "dbs/L9o3AA==/colls/L9o3ANHa68c=/docs/L9o3ANHa68cBAAAAAAAAAA==/",
    "_etag": "\"d200d372-0000-4700-0000-62d5211a0000\"",
    "_attachments": "attachments/",
    "_ts": 1658134810
}
```

