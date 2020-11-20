# to-d0-list
Todo list exercise - Udemy Bootcamp course
This is a file to generate help for my coding exercise:

The code so far is the following:

let todos = [];

while (true) {
  let promptIn = prompt("What would you like to do ?");
  if (promptIn === "new") {
    let newTodo = prompt("Add a new todo");
    todos.push(newTodo);
  } else if (promptIn === "list") {
    for (let todo of todos) {
      console.log(todo);
    }
  } else if (promptIn === "delete") {
    let index = prompt("Which Item would you like to delete");
    todos.splice(index, 1);
  } else if (promptIn === "quit") {
    prompt("OK, quitting");
  }
}
