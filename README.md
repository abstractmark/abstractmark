# AbstractMark
Next level generation of markdown, allowing user to add styling, classes and more into their markdown.

<div align = "center">

![AbstractMark Logo](https://drive.google.com/uc?export=view&id=1PSOt4T7CVOBgtbCWa0m3YBYjojlFZX-U)

</div>

## Table of Contents
- [Introduction](#introduction)
- [Syntax](#syntax)
- [License](#license)
- [Code of conducts](#code-of-conduct)
- [Contributing Guidelines](#contributing-guidelines)

## Introduction
AbstractMark is next level markup language extended from markdown that supports styling, classes and more. AbstrackMark allows user to create a well-designed website using an easy-to-read and easy-to-write plain text format, then convert it to valid HTML or markdown file. AbstrackMark is still on development progress. AbstractMark will be implemented on various programming language soon (contributors needed). File extension for AbstractMark will be `.abstrackmark` and `.am`. 

## Implementation
- [JavaScript](https://github.com/abstractmark/javascript) (Still in development progress)

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
    - Define class and tags styles (css standart)
        
        Syntax:
        ```
        ---define
        className{
            styles here
        }
        ---
        ```
        
        Example:
        ```
        ---define
        .box{
            color: blue;
            background-color: red;
        }
        pre{
            padding: 10px;
            background-color: blue;
        }
        ---
        ```
    - Use class on element:
        Syntax:
        ```
        Element {.className}
        ```
        Example:
        ```
        ## Hello World {.className}
        ```
        **NB**: To use multiple classes, split it by space
        Example: 
        ```
        ## Hello World {#headingId} {.class1 class2 class3}
        ```
- External CSS
    ```
    stylesheet = https://cdn.jsdelivr.net/npm/@fire-ui/fire-ui@0.2.3/FireUI.min.css
    ```
- External Script
    ```
    script = https://cdn.jsdelivr.net/npm/@fire-ui/fire-ui@0.2.3/FireUI.min.js
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
- Marquee
    - Left to right
        ```
        ~> Marquee text
        ```
    - Right to left
        ```
        <~ Marquee text
        ```
- Ordered List
    ```
    1. First item
    2. Second item
    3. Third item
    ```
- Strikethrough
    ```
    ~~Strikethrough text~~
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
    Note:
    - To use inline style and class in table, add the inline style or/and class syntax in right side after any of the table syntax and it will be parsed as attribute in table tag.
        Example:
        ```
        | Syntax | Description |
        | ----- | ----- |{!className}{color: blue;}
        | Header | Title |
        | Paragraph | Text |
        ```
    - Inline style and class for table data is not supported now(Maybe will be supported on next update)
- Task List
    ```
    - [x] Lorem ipsum
    - [ ] Lorem ipsum
    - [ ] Lorem ipsum
    ```
- Underline
    ```
    %Underline text%
    ```
- Unordered List
    ```
    - First item
    - Second item
    - Third item
    ```

## Code of Conduct
For the Code of Conduct, please visit [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)

## Contributing Guidelines
Thanks for your interest in contributing to AbstractMark! Please take a moment to review this [document](CONTRIBUTING.md)

## License
AbstractMark is distributed under [MIT License](LICENSE)