# AbstractMark
Next level generation of markdown, allowing user to add styling, classes and more into their markdown.

<div align = "center">

![AbstractMark Logo](https://drive.google.com/uc?export=view&id=1PSOt4T7CVOBgtbCWa0m3YBYjojlFZX-U)

</div>

## Table of Contents
- [Introduction](#introduction)
- [Syntax](#syntax)
- [License](#license)

## Introduction
AbstractMark is next level markup language extended from markdown that supports styling, classes and more. AbstrackMark allows user to create a well-designed website using an easy-to-read, easy-to-write plain text format, then convert it to valid HTML or markdown file. AbstrackMark is still on developments progress. AbstractMark will be implemented on various programming language soon (contributors needed). File extension for AbstractMark will be `.abstrackmark` and `.am`. 

## Syntax
- Blockquote
    ```
    > blockquote
    ```
- Bold
    ```
    **Bold text**
    ```
- Code
    - Inline code
        ```
        `inline code`
        ```
    - Fenced code block
        ````
        ```
        {
            "type": "fenced code block"
        }
        ```
        ````
- Class
    - Define class
        
        Syntax:
        ```
        ---define
        className :
            styles here
        ---
        ```
        
        Example:
        ```
        ---define
        box :
            color: blue;
            background-color: red;
        ---
        ```
    - Use class:
        Syntax:
        ```
        Element {!className}
        ```
        Example:
        ```
        ## Hello World {!className}
        ```
- Heading
    ```
    # h1
    ## h2
    ### h3
    #### h4
    ##### h5
    ###### h6
    ```
- Heading ID
    ```
    # My heading {#custom-id}
    ```
- Horizontal Rule
    ```
    ---
    ```
- Image
    ```
    ![alt text](image.jpg)
    ```
- Link
    ```
    [title](https://example.com)
    ```
- Italic
    ```
    _italicized text_
    ```
- Ordered List
    ```
    1. First item
    2. Second item
    3. Third item
    ```
- Style

    Syntax:
    ```
    element {styles}
    ```

    Example:
    ```
    ## Hello World {color: blue;}
    ```
- Table
    ```
    | Syntax | Description |
    | ----- | ----- |
    | Header | Title |
    | Paragraph | Text |
    ```
- Task List
    ```
    - [x] Lorem ipsum
    - [ ] Lorem ipsum
    - [ ] Lorem ipsum
    ```
- Unordered List
    ```
    - First item
    - Second item
    - Third item
    ```

## License
AbstractMark is distributed under MIT License