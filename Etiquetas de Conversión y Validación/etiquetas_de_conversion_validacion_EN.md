# Conversion and Validation Tags (f:)

These tags are used to convert and validate input data:

1. `<f:convertDateTime>`: Converts text strings to date objects and vice versa. Example:

    ```xhtml
    <f:convertDateTime pattern="dd/MM/yyyy" timeZone="America/New_York" />
    ```

2. `<f:convertNumber>`: Converts text strings to numbers and vice versa. Example:

    ```xhtml
    <f:convertNumber pattern="#,##0.00" />
    ```

3. `<f:validateLength>`: Validates the length of a text string. Example:

    ```xhtml
    <f:validateLength minimum="2" maximum="10" />
    ```

4. `<f:validateRegex>`: Validates a text field using a regular expression. Example:

    ```xhtml
    <f:validateRegex pattern="[A-Za-z]+" />
    ```

6. `<f:validateRequired>`: Marks a field as required. Example:

    ```xhtml
    <f:validateRequired />
    ```

7. `<f:validateDoubleRange>`: Validates a number within a double value range. Example:

    ```xhtml
    <f:validateDoubleRange minimum="0.0" maximum="100.0" />
    ```

8. `<f:validateLongRange>`: Validates a number within a long value range. Example:

    ```xhtml
    <f:validateLongRange minimum="0" maximum="100" />
    ```