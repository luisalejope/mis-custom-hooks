# useForm Hook

Ejemplo de uso

```
const initialForm = {
    name: "",
    email: "",
    password: ""
}

const [values, handleInputChange, reset] = useForm(initialForm);
```

initialform es una constante que puede tener cualquier nombre y contener un solo objeto con disitintos atributos
