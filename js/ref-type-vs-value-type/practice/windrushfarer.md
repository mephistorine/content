🛠 При копировании можно изменить и добавить поля, но вот удалить без мутации нельзя

```js
const dog = {
  name: "Barbos",
  color: "black",
}

const puppy = {
  ...dog,
  // Можно выставить значение undefined, но это не удаление
  color: undefined,
}

// А это удалит поле, хоть delete считается мутирование
// Но использование его на копии изменит только puppy, dog не будет изменен
delete puppy.color
```

🛠 Популярные в веб-разработке библиотеки React и Redux сильно завязаны на иммутабельности данных и практически построены на этом.
