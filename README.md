# dicas-javscript-1
Dicas marotas Javscript

#Reduce 
```jsx
const numbers = [2, 7, 3, 1];

const result = numbers.reduce((prev, number) => {
  return prev + number;
}, 0);

console.log('A soma dos valores é:', result);
```
