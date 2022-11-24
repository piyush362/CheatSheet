## Here are the possible ways to make an API call in javascript:

1. XMLHttpRequest - Old school
2. fetch
3. Axios
4. jQuery


# XMLHttpRequest
````
    let request = new XMLHttpRequest();
    request. open ( ("GET" , "https: // jsonplaceholder. typicode. com/users");
    request. send();
    request. onload = ( )
        console. log(request);
        if (request. status E 200) {
            console. log (JSON. parse(request. response));
        } else {
            console. log(`error ${request. status} ${request. statusText}`)
```

# Fetch : there are two method

## method 1: 

```
    fetch( 'https://jsonplaceholder. typicode. com/users')
   .then( response => {
     return response. json();
   })
    then( users => {
     console. log( (users);
   });

```

## Method 2: By using Async and Await

```
    async function getUsers()
     let response = await fetch('https://jsonplaceholder typicode. com/users');
     let data = await response. json()
    return data;
    }
    getUsers(). then((data) => console. log(data));

```

# Axios 

```
    axios. get('https://jsonplaceholder. typicode. com/users')
     .then(response
                        {
         console. log(response. data);
     })
     catch((error) =>  console. error(error));

```
