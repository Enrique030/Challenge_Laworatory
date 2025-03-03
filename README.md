# Challenge Técnico Laworatory

## Autor: Enrique Cogolludo Fernández

### Puesto: Becario de Desarrollo de Back-end en Laworatory

#### Objetivo

Desarrollar una página web que funcione como informe de ventas, mostrando datos extraídos de una base de datos MySQL. (Opcionalmente, se podría considerar cómo generar un PDF a partir de esta información, aunque no es obligatorio para la prueba).

#### Tarea propuesta

Crear un proyecto / archivo PHP que tome datos dinámicos desde una BBDD MySQL, los organice en una estructura PHP HTML bien maquetada y los muestre de manera clara y ordenada.

1. **Documento de toma de requisitos**
    - Crear un documento inicial de toma de requisitos, esto nos indica cuál es tu visión de la documentación.

2. **Crear datos**:
    - Crear una BBDD MySQL con los datos de la empresa y de las ventas, los campos mínimos que deberá tener son:
        - Tablas
            - **Tabla empresas**
                - id (INT, PRIMARY KEY, AUTO_INCREMENT)
                - nombre
            - **Tabla ventas**
                - id (INT, PRIMARY KEY, AUTO_INCREMENT)
                - id de empresa (INT, FOREIGN KEY -> empresas.id)
                - número de factura
                - fecha de la venta
                - comprador
                - artículos vendidos
                - valor total

        Adicionalmente, deberás crear al menos 20 registros en la tabla para poder mostrarlos en el informe.

3. **Obtener los datos**
    - Para obtener los datos, deberás conectarte a la BBDD, leer y procesar la respuesta. Puedes usar PDO o MySQLi para la conexión a la base de datos. Recuerda implementar un manejo de errores adecuado.

4. **Organizar y maquetar el informe**:
    - Estructurar los datos en un archivo PHP combinado con HTML que sean la base de generación del informe.
    - Se valora que puedas aplicar estilos CSS para mejorar la presentación. En este caso, preferiríamos que no utilizaras ningún framework.
    - El informe debe ser visualmente claro, con encabezados bien definidos y estructura ordenada.
    - Los datos deben mostrarse de forma intuitiva y bien alineados.

##### Requisitos de la prueba

**Obligatorios**

- Documento de toma de requisitos.
- Correcta conexión y extracción de datos desde MySQL.
- Organización lógica de la información en HTML.

**Extras valorables**

- Uso de CSS para mejorar la presentación.
- La gestión de errores y formatos de respuesta.
- Documentación técnica funcional.
