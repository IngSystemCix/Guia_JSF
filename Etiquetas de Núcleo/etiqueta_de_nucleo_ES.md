# Etiquetas de Núcleo (h:)

Estas etiquetas son parte del núcleo de JSF y permiten la creación de componentes básicos de la interfaz de usuario.

1. **Formularios y Contenedores**
   - `<h:form>`: Define un formulario que puede contener otros componentes JSF.
     ```xml
     <h:form id="myForm">...</h:form>
     ```
   - `<h:panelGrid>`: Organiza componentes en una cuadrícula.
     ```xml
     <h:panelGrid columns="2">
         <h:outputText value="Nombre:" />
         <h:inputText value="#{bean.name}" />
     </h:panelGrid>
     ```
   - `<h:panelGroup>`: Agrupa componentes en un solo contenedor.
     ```xml
     <h:panelGroup>
         <h:outputText value="Hola, " />
         <h:outputText value="#{bean.name}" />
     </h:panelGroup>
     ```

2. **Entradas de Usuario**
   - `<h:inputText>`: Crea un campo de entrada de texto.
     ```xml
     <h:inputText value="#{bean.property}" />
     ```
   - `<h:inputSecret>`: Crea un campo de entrada de texto que oculta los caracteres (campo de contraseña).
     ```xml
     <h:inputSecret value="#{bean.password}" />
     ```
   - `<h:inputTextarea>`: Crea un área de texto.
     ```xml
     <h:inputTextarea value="#{bean.description}" rows="5" cols="30" />
     ```
   - `<h:inputHidden>`: Crea un campo de entrada oculto.
     ```xml
     <h:inputHidden value="#{bean.hiddenValue}" />
     ```
   - `<h:inputFile>`: Crea un campo de entrada para subir archivos.
     ```xml
     <h:inputFile value="#{bean.file}" />
     ```
   - `<h:selectOneMenu>`: Crea un menú desplegable para selección única.
     ```xml
     <h:selectOneMenu value="#{bean.selectedOption}">
         <f:selectItems value="#{bean.options}" />
     </h:selectOneMenu>
     ```
   - `<h:selectManyCheckbox>`: Crea un grupo de casillas de verificación para selección múltiple.
     ```xml
     <h:selectManyCheckbox value="#{bean.selectedOptions}">
         <f:selectItems value="#{bean.options}" />
     </h:selectManyCheckbox>
     ```
   - `<h:selectOneRadio>`: Crea un grupo de botones de opción para selección única.
     ```xml
     <h:selectOneRadio value="#{bean.selectedOption}">
         <f:selectItems value="#{bean.options}" />
     </h:selectOneRadio>
     ```
   - `<h:selectBooleanCheckbox>`: Crea una casilla de verificación para selección verdadero/falso.
     ```xml
     <h:selectBooleanCheckbox value="#{bean.selected}" />
     ```

3. **Botones y Enlaces**
   - `<h:commandButton>`: Crea un botón que puede enviar un formulario o invocar una acción.
     ```xml
     <h:commandButton value="Enviar" action="#{bean.submit}" />
     ```
   - `<h:commandLink>`: Crea un enlace que puede enviar un formulario o invocar una acción.
     ```xml
     <h:commandLink value="Haz clic aquí" action="#{bean.action}" />
     ```

4. **Etiquetas y Mensajes**
   - `<h:outputLabel>`: Crea una etiqueta de texto.
     ```xml
     <h:outputLabel value="Nombre de usuario:" for="username" />
     ```
   - `<h:message>`: Muestra un mensaje de validación asociado con un componente específico.
     ```xml
     <h:message for="username" />
     ```
   - `<h:messages>`: Muestra todos los mensajes de validación en la página.
     ```xml
     <h:messages />
     ```

5. **Salida de Texto e Imagen**
   - `<h:outputText>`: Crea una salida de texto simple.
     ```xml
     <h:outputText value="#{bean.message}" />
     ```
   - `<h:graphicImage>`: Muestra una imagen en la página.
     ```xml
     <h:graphicImage value="path/to/image.jpg" />
     ```
   - `<h:outputFormat>`: Formatea y muestra texto dinámico.
     ```xml
     <h:outputFormat value="Hola {0}, tienes {1} nuevos mensajes.">
         <f:param value="#{bean.name}" />
         <f:param value="#{bean.messageCount}" />
     </h:outputFormat>
     ```
   - `<h:outputLink>`: Crea un enlace a una URL externa.
     ```xml
     <h:outputLink value="https://example.com">Visitar sitio web</h:outputLink>
     ```

6. **Scripts y Estilos**
   - `<h:outputScript>`: Salida de código JavaScript.
     ```xml
     <h:outputScript library="js" name="script.js" />
     ```
   - `<h:outputStylesheet>`: Salida de hojas de estilo CSS.
     ```xml
     <h:outputStylesheet library="css" name="styles.css" />
     ```

7. **Tablas de Datos**
   - `<h:dataTable>`: Crea una tabla de datos, permitiendo la iteración sobre colecciones.
     ```xml
     <h:dataTable value="#{bean.items}" var="item">
         <h:column>#{item.name}</h:column>
     </h:dataTable>
     ```
