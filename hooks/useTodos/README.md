# useForm Hook

Ejemplo de uso

```
const {todos, totalTodos, pendingTodos, handleDeleteTodo, handleNewTodo, handleUpdateTodo} = useTodos()
```

Es un hook para hacer Todos. Se debe usar en conjunto con el reducer todoReducer.js

## todos

Devuelve un arreglo de Todos con el siguiente formato
```
todos = [
    {
        id: Number,
        desc: String,
        done: Bool
    }
    ...
]
```

## totalTodos / pendingTodos

Devuelven un dato de tipo Number que hace referencia a la cantidad de Todos que existen y los Todos que estan pendientes por resolver.

## handleDeleteTodo

Es una funcion que recibe como parametro el id del todo que quieres eliminar.

Ejemplo de uso

```
<button
    onClick={()=>handleDeleteTodo(3)}
>
    Eliminar
</button>
```

## handleNewTodo

Es una funcion que recibe como parametro un string que hace referencia a la descripcion del Todo

Ejemplo de uso

```
handleNewTodo('Salir a correr')
```


## handleUpdateTodo

Es una funcion que recibe como parametro un objeto ya existente que debe tener las siguientes propiedades con el cambio que requieras exclusivamente en la propiedad desc y done. El id no se debe cambiar.

```
const updatedTodo = {
        id: Number,
        desc: String,
        done: Bool
    }
```

Ejemplo de uso

```
handleUpdateTodo(updatedTodo)
```


#Nota
Todo: se debe colocar la condicional de que no se debe cambiar el id
