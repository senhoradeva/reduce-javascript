# dicas-javscript-1
Dicas marotas Javscript

#Reduce 
```jsx
const numbers = [2, 7, 3, 1];

const result = numbers.reduce((prev, number) => {
  return prev + number;
}, 0);

console.log('A soma dos valores é:', result); // A soma dos valores é: 12
```

--Mais um exemplo de reduce 

```jxx

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
