# Etiquetas de Composición (cc:)

Estas etiquetas son utilizadas en la creación de componentes compuestos personalizados:

1. `<cc:attribute>`: Define un atributo que puede ser configurado en el componente compuesto. Por ejemplo:
    ```xhtml
    <cc:attribute name="color" type="String" default="red" />
    ```

2. `<cc:facet>`: Define un espacio de contenido dinámico en el componente compuesto. Por ejemplo:
    ```xhtml
    <cc:facet name="header">
      <h1>Contenido del encabezado</h1>
    </cc:facet>
    ```

3. `<cc:implementation>`: Define la implementación de un componente compuesto. Por ejemplo:
    ```xhtml
    <cc:implementation>
      <h2>Contenido del componente</h2>
      <p>Este es el contenido del componente compuesto.</p>
    </cc:implementation>
    ```

4. `<cc:interface>`: Define la interfaz pública de un componente compuesto. Por ejemplo:
    ```xhtml
    <cc:interface>
      <cc:attribute name="title" type="String" />
      <cc:facet name="footer" />
    </cc:interface>
    ```