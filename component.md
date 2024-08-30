# Crear componentes en JSF

> We need to create a file called `head.xhtml` in order to create this component and include it in `index.xhtml`

```xhtml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml"
      xmlns:f="http://xmlns.jcp.org/jsf/core"
      xmlns:h="http://xmlns.jcp.org/jsf/html">
<f:view>
    <meta charset="UTF-8"/>
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <meta name="author" content="IngSystemCix"/>
    <meta name="description" content="JSF"/>
    <meta name="keywords" content="JSF, JavaServer Faces"/>
    <h:outputStylesheet library="css" name="style.css"/>
    <h:outputScript library="js" name="script.js"/>
    <title>JSF</title>
</f:view>
</html>
```

```xhtml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml"
      xmlns:h="http://xmlns.jcp.org/jsf/html"
      xmlns:ui="http://xmlns.jcp.org/jsf/facelets"
      xmlns:f="http://xmlns.jcp.org/jsf/core">
<f:view>
    <h:head>
        <ui:include src="../component/head.xhtml"/>
    </h:head>
    <h:body>
        <header>

        </header>
        <main>

        </main>
        <footer>

        </footer>
    </h:body>
</f:view>
</html>
```