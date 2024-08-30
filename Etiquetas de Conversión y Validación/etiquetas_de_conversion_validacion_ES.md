# Etiquetas de Conversión y Validación (f:)

Estas etiquetas se utilizan para convertir y validar los datos de entrada:

1. `<f:convertDateTime>`: Convierte cadenas de texto en objetos de fecha y viceversa. Ejemplo:

    ```xhtml
    <f:convertDateTime pattern="dd/MM/yyyy" timeZone="America/New_York" />
    ```

2. `<f:convertNumber>`: Convierte cadenas de texto en números y viceversa. Ejemplo:

    ```xhtml
    <f:convertNumber pattern="#,##0.00" />
    ```

3. `<f:validateLength>`: Valida la longitud de una cadena de texto. Ejemplo:

    ```xhtml
    <f:validateLength minimum="2" maximum="10" />
    ```

4. `<f:validateRegex>`: Valida un campo de texto utilizando una expresión regular. Ejemplo:

    ```xhtml
    <f:validateRegex pattern="[A-Za-z]+" />
    ```

6. `<f:validateRequired>`: Marca un campo como requerido. Ejemplo:

    ```xhtml
    <f:validateRequired />
    ```

7. `<f:validateDoubleRange>`: Valida un número dentro de un rango de valores double. Ejemplo:

    ```xhtml
    <f:validateDoubleRange minimum="0.0" maximum="100.0" />
    ```

8. `<f:validateLongRange>`: Valida un número dentro de un rango de valores long. Ejemplo:

    ```xhtml
    <f:validateLongRange minimum="0" maximum="100" />
    ```