# Core Tags (h:)

These tags are part of the JSF core and allow the creation of basic user interface components.

1. **Forms and Containers**
   - `<h:form>`: Defines a form that can contain other JSF components.
     ```xhtml
     <h:form id="myForm">...</h:form>
     ```
   - `<h:panelGrid>`: Organizes components in a grid.
     ```xhtml
     <h:panelGrid columns="2">
         <h:outputText value="Name:" />
         <h:inputText value="#{bean.name}" />
     </h:panelGrid>
     ```
   - `<h:panelGroup>`: Groups components into a single container.
     ```xhtml
     <h:panelGroup>
         <h:outputText value="Hello, " />
         <h:outputText value="#{bean.name}" />
     </h:panelGroup>
     ```

2. **User Inputs**
   - `<h:inputText>`: Creates a text input field.
     ```xhtml
     <h:inputText value="#{bean.property}" />
     ```
   - `<h:inputSecret>`: Creates a text input field that hides the characters (password field).
     ```xhtml
     <h:inputSecret value="#{bean.password}" />
     ```
   - `<h:inputTextarea>`: Creates a text area.
     ```xhtml
     <h:inputTextarea value="#{bean.description}" rows="5" cols="30" />
     ```
   - `<h:inputHidden>`: Creates a hidden input field.
     ```xhtml
     <h:inputHidden value="#{bean.hiddenValue}" />
     ```
   - `<h:inputFile>`: Creates a file upload input field.
     ```xhtml
     <h:inputFile value="#{bean.file}" />
     ```
   - `<h:selectOneMenu>`: Creates a dropdown menu for single selection.
     ```xhtml
     <h:selectOneMenu value="#{bean.selectedOption}">
         <f:selectItems value="#{bean.options}" />
     </h:selectOneMenu>
     ```
   - `<h:selectManyCheckbox>`: Creates a group of checkboxes for multiple selection.
     ```xhtml
     <h:selectManyCheckbox value="#{bean.selectedOptions}">
         <f:selectItems value="#{bean.options}" />
     </h:selectManyCheckbox>
     ```
   - `<h:selectOneRadio>`: Creates a group of radio buttons for single selection.
     ```xhtml
     <h:selectOneRadio value="#{bean.selectedOption}">
         <f:selectItems value="#{bean.options}" />
     </h:selectOneRadio>
     ```
   - `<h:selectBooleanCheckbox>`: Creates a checkbox for true/false selection.
     ```xhtml
     <h:selectBooleanCheckbox value="#{bean.selected}" />
     ```

3. **Buttons and Links**
   - `<h:commandButton>`: Creates a button that can submit a form or invoke an action.
     ```xhtml
     <h:commandButton value="Submit" action="#{bean.submit}" />
     ```
   - `<h:commandLink>`: Creates a link that can submit a form or invoke an action.
     ```xhtml
     <h:commandLink value="Click me" action="#{bean.action}" />
     ```

4. **Labels and Messages**
   - `<h:outputLabel>`: Creates a text label.
     ```xhtml
     <h:outputLabel value="Username:" for="username" />
     ```
   - `<h:message>`: Displays a validation message associated with a specific component.
     ```xhtml
     <h:message for="username" />
     ```
   - `<h:messages>`: Displays all validation messages on the page.
     ```xhtml
     <h:messages />
     ```

5. **Text and Image Output**
   - `<h:outputText>`: Creates a simple text output.
     ```xhtml
     <h:outputText value="#{bean.message}" />
     ```
   - `<h:graphicImage>`: Displays an image on the page.
     ```xhtml
     <h:graphicImage value="path/to/image.jpg" />
     ```
   - `<h:outputFormat>`: Formats and displays dynamic text.
     ```xhtml
     <h:outputFormat value="Hello {0}, you have {1} new messages.">
         <f:param value="#{bean.name}" />
         <f:param value="#{bean.messageCount}" />
     </h:outputFormat>
     ```
   - `<h:outputLink>`: Creates a link to an external URL.
     ```xhtml
     <h:outputLink value="https://example.com">Visit website</h:outputLink>
     ```

6. **Scripts and Styles**
   - `<h:outputScript>`: Outputs JavaScript code.
     ```xhtml
     <h:outputScript library="js" name="script.js" />
     ```
   - `<h:outputStylesheet>`: Outputs CSS stylesheets.
     ```xhtml
     <h:outputStylesheet library="css" name="styles.css" />
     ```

7. **Data Tables**
   - `<h:dataTable>`: Creates a data table, allowing iteration over collections.
     ```xhtml
     <h:dataTable value="#{bean.items}" var="item">
         <h:column>#{item.name}</h:column>
     </h:dataTable>
     ```
