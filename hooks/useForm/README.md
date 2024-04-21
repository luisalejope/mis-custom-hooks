# useForm Hook

Ejemplo de uso

```
const initialForm = {
    name: "",
    email: "",
    password: ""
}

const {values, onInputChange, onReset} = useForm(initialForm);
```

initialform es una constante que puede tener cualquier nombre y contener un solo objeto con disitintos atributos

#Nota
No olvidar que usar el atributo name en la etiqueta input para que el hook funcione correctamente
