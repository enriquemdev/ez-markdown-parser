# EzMarkdownParser

EzMarkdownParser is a very simple Python package that converts Markdown text to HTML strings with its htmlify function. It is designed to handle basic Markdown elements such as paragraphs, headings, list items, bold text, and links. 

This parser was made for cs50w project #1 Wiki on 2024, so it only supports the tags required by the project specifications, wich are mentioned above.

## Installation

Install EzMarkdownParser using pip:

```bash
pip install ez-markdown-parser
```

## Usage

```python
from ez_markdown_parser import EzMarkdownParser

md_text = """
# Heading 1
This is a paragraph with some **bold text** and a [link](https://example.com).

## Heading 2
- List item 1
- List item 2
"""

parser = EzMarkdownParser()
html_text = parser.htmlify(md_text)
print(html_text)
```

## Features

- Convert Markdown headings to HTML `<h1>` to `<h6>` tags.
- Process list items (`* ` and `-`) and convert them to HTML `<li>` tags.
- Wrap paragraphs with HTML `<p>` tags.
- Recognize and convert double asterisk (`**`) for bold text.
- Recognize and convert links in the format `[text](URL)`.

## Limitations

- The parser is not complete nor optimized yet, it doesnt support advanced markdown features. Use it with caution.

## Contributing

Contributions are welcome, as long as the project remains fun enough! 
If you find an issue or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is dedicated to the public domain. You are free to use, modify, and distribute the code without any restrictions. See the UNLICENSE file for more details.