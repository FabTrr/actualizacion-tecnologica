# Cómo probar URL's en Postman

Postman es una herramienta de prueba de API que se utiliza para probar las URL's de forma sencilla y eficaz. Para probar una URL en Postman, siga estos pasos:

## Pasos

1. **Cree una nueva colección.** Una colección es un conjunto de solicitudes que se pueden agrupar juntas.

2. **Cree una nueva solicitud.** Una solicitud es una petición HTTP que se envía a una URL.

3. **Especifique la URL.** En el campo **URL**, escriba la URL de la que desea probar.

4. **Seleccione el método HTTP.** El método HTTP determina el tipo de solicitud que se enviará. Los métodos HTTP más comunes son GET, POST, PUT y DELETE.

5. **Especifique los parámetros.** Los parámetros son datos adicionales que se pueden enviar con la solicitud. Para especificar los parámetros, haga clic en la pestaña **Parameters**.

6. **Especifique el cuerpo.** El cuerpo es el contenido de la solicitud. Para especificar el cuerpo, haga clic en la pestaña **Body**.

7. **Envíe la solicitud.** Para enviar la solicitud, haga clic en el botón **Send**.

## Ejemplos

### Ejemplo 1: Probar una URL GET

En este ejemplo, probaremos una URL GET que devuelve una lista de productos.

1. Cree una nueva colección y una nueva solicitud.
2. En el campo **URL**, escriba la siguiente URL:

```
https://api.example.com/products
```

3. Seleccione el método **GET**.
4. No es necesario especificar ningún parámetro.
5. No es necesario especificar ningún cuerpo.
6. Envíe la solicitud.

La respuesta de la solicitud será una lista de productos en formato JSON.

### Ejemplo 2: Probar una URL POST

En este ejemplo, probaremos una URL POST que crea un nuevo producto.

1. Cree una nueva colección y una nueva solicitud.
2. En el campo **URL**, escriba la siguiente URL:

```
https://api.example.com/products
```

3. Selecciona el método **POST**.
4. Crea un parámetro llamado **name** con el valor "Producto nuevo".
5. En el cuerpo, especifica el siguiente JSON:

```
{
  "name": "Producto nuevo",
  "price": 100
}


6. Envía la solicitud.

La respuesta de la solicitud será un código de respuesta 201, que indica que la creación del producto fue exitosa.

## Consejos

* **Utiliza variables.** Las variables permiten almacenar valores que se pueden reutilizar en varias solicitudes.
* **Crea colecciones.** Las colecciones permiten organizar sus solicitudes y ejecutarlas en lotes.
* **Utiliza pruebas.** Las pruebas permiten validar las respuestas de sus solicitudes.
