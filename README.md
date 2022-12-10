# reduce-javascript
Dicas marotas Javscript
<p>A grande missão  reduce é  reduzir um array. Para isso,  itera por cada elemento de uma lista para gerar um único valor.</p>
#Reduce 
```jsx
const numbers = [2, 7, 3, 1];

const result = numbers.reduce((prev, number) => {
  return prev + number;
}, 0);

console.log('A soma dos valores é:', result); // A soma dos valores é: 12
```

#Mais um exemplo de reduce 

```jsx

const people = [
  {
    name: "Ruana",
    occupation: "Desenvolvedora de Software",
    salary: 9000
  },

  {
    name: "Josysclaiton",
    occupation: "Dentista",
    salary: 15000
  },
  {
    name: "Betineuza",
    occupation: "Professora",
    salary: 75000
  }
];

const result = people.reduce((prev, person) => {
    if(person.salary > prev) {
      return person.salary;
    }

    return prev;
}, 0);

console.log('O maior salário é:', result)//O maior salário é: 
75000
```

```jsx
const animals = ['dog', 'cat', 'dog', 'dog', 'cow', 'cow'];

const result = animals.reduce((prev, animal) => {
  prev[animal] = (prev[animal] || 0) + 1;
  return prev;
}, {});

console.log(result); //{dog: 3, cat: 1, cow: 2}

```
