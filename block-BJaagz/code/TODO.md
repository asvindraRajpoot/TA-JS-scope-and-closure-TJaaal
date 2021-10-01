1. Implement `forEach` array method using Array.reduce

- `forEach` accepts two parameter array and callback
- It does not return anything
- It should work exactly like array `forEach` method

```js
function forEach(array,cb) {

  
  array.reduce((acc,cv)=>{

    cb(cv); 

  },0)

}

forEach(['Sam', 'Jon', 'Arya'], (name, i, arr) =>
  console.log(name + name, i, arr)
);
```

2. Implement `map` array method using Array.reduce

- `map` accepts two parameter array and callback
- It returns same size of array
- It should work exactly like array `map` method

```js
function map(arr,cb) {
  // Your code goes here
  let final=[];
  arr.reduce((acc,cv)=>{
    acc=cb(cv);
    
    final.push(acc);
  },0)
   return final;



}

map(['Sam', 'Jon', 'Arya'], (name) => name + name); // ['SamSam', 'JonJon', 'AryaArya']
```

3. Implement `filter` array method using Array.reduce

- `filter` accepts two parameter array and callback
- It returns same size or smaller array
- It should work exactly like array `filter` method

```js
function filter(arr,cb) {
  // Your code goes here
  let final=[];
   arr.reduce((acc,cv)=>{
  
    if(cb(cv)){
       final.push(cv);
   };
  

   

   },0)
  return final;

}
filter(['Sam', 'Jon', 'Arya'], (name) =>
  name.startsWith('S')
); // ['Sam']
```
