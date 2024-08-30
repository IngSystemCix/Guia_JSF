# Composition Tags (cc:)

These tags are used in the creation of custom composite components:

1. `<cc:attribute>`: Defines an attribute that can be configured in the composite component. For example:
    ```xhtml
    <cc:attribute name="color" type="String" default="red" />
    ```

2. `<cc:facet>`: Defines a dynamic content space in the composite component. For example:
    ```xhtml
    <cc:facet name="header">
      <h1>Header content</h1>
    </cc:facet>
    ```

3. `<cc:implementation>`: Defines the implementation of a composite component. For example:
    ```xhtml
    <cc:implementation>
      <h2>Component content</h2>
      <p>This is the content of the composite component.</p>
    </cc:implementation>
    ```

4. `<cc:interface>`: Defines the public interface of a composite component. For example:
    ```xhtml
    <cc:interface>
      <cc:attribute name="title" type="String" />
      <cc:facet name="footer" />
    </cc:interface>
    ```