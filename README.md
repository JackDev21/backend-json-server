# json-server

## Descripción

"Pequeño servidor json" es un proyecto que utiliza [json-server](https://github.com/typicode/json-server) para crear un servidor JSON simple y rápido. Este servidor se puede utilizar para simular una API REST y realizar operaciones CRUD (Crear, Leer, Actualizar, Eliminar) sobre los datos definidos en el archivo `db.json`.

## Instalación

1. Clona el repositorio o descarga los archivos del proyecto.
2. Navega al directorio del proyecto.
3. Instala las dependencias utilizando npm:

   ```sh
   npm install
   ```

## Uso

Para iniciar el servidor JSON, ejecuta el siguiente comando:

```sh
npm start
```

Esto iniciará el servidor y observará los cambios en el archivo `db.json`. El servidor estará disponible en `http://localhost:3000`.

## Ejemplo de `db.json`

El archivo `db.json` contiene los datos que se utilizarán en el servidor JSON. A continuación se muestra un ejemplo del contenido de `db.json`:

```json
{
  "profesores": [
    {
      "nombre": "Jose",
      "apellido": "Canto",
      "materias": [
        {
          "nombre": "NodeJS desde cero"
        },
        {
          "nombre": "ReactJS desde cero"
        },
        {
          "nombre": "JavaScript desde cero"
        }
      ],
      "id": "6746"
    },
    {
      "id": "84ee",
      "nombre": "Lorena",
      "apellido": "Lopez",
      "materias": [
        {
          "nombre": "Audiología"
        },
        {
          "nombre": "Patologías"
        }
      ]
    }
  ],
  "alumnos": [
    {
      "nombre": "Juan",
      "apellido": "Perez",
      "promedio": 8.5,
      "id": "b3cd"
    },
    {
      "nombre": "Maria",
      "apellido": "Gomez",
      "promedio": 9.5,
      "id": "0f09"
    },
    {
      "id": "0f09",
      "nombre": "Luna",
      "apellido": "Lopez",
      "promedio": 10
    }
  ],
  "cursos": [
    {
      "nombre": "NodeJS desde cero",
      "duración": 7,
      "dificultad": "intermedio",
      "id": "f2d6"
    },
    {
      "nombre": "ReactJS desde cero",
      "duración": 7,
      "dificultad": "alta",
      "id": "0972"
    },
    {
      "nombre": "JavaScript desde cero",
      "duración": 7,
      "dificultad": "baja",
      "id": "6cef"
    }
  ]
}
```

## Pruebas con Postman

Puedes utilizar [Postman](https://www.postman.com/) para realizar operaciones CRUD y practicar con las solicitudes HTTP. A continuación se muestran algunos ejemplos de solicitudes que puedes realizar:

- **GET** `http://localhost:3000/profesores`
- **POST** `http://localhost:3000/profesores`
- **PUT** `http://localhost:3000/profesores/:id`
- **DELETE** `http://localhost:3000/profesores/:id`
