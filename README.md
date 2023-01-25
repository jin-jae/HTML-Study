# HTML

[HTML 수업 - 생활코딩](https://opentutorials.org/course/2039)

해당 사이트의 내용을 기반으로 개인 스터디를 진행하였고, 진행하면서 중요하다고 생각하는 내용을 직접 정리하였습니다. 궁금하신 분들은 자유롭게 참고해주시면 될 것 같습니다 😊

---

# Hello, HTML

basic start of web programming

## HyperText

Web page link-based

## Markup

Markup grammar based

## Language

some protocols (between computer(especially for web browser) and people)

# Tag

most important protocol

The tag will be applied between an open tag and a close tag.

## <html>

Indicates that this tag contains contexts based on HTML language.

## <head>

Indicates that the head tag contains additional website information (or settings).

### <title>

Sets the title of website

## <body>

Indicates that between body tag contains the contexts of a website.

### <h1>

acronym of heading 1 (Biggest title)

### <h2>

acronym of heading 2

### <strong>

makes text bold (emphasize text)

### <a>

acronym of “anchor”

link another website

really important tag of HyperText

- attributes
- href= link attributes
- title= tooltip
- target= where to open this link

### <ol>

acronym of “ordered list”

used with tag <li> → tagged with <li> inside <ol> means they are orderly listed (with numbering)

### <ul>

acronym of “unordered list”

used with tag <li> → tagged with <li> inside <ul> means they are unorderly listed (just with a dotted list)

### <li>

often used with <ol> and <ul>, to indicate that this is a component of list

### <p>

Between this tag means that it is “one” paragraph.

### <br>

acronym of break

This separates lines, but not a good way to separate paragraphs → instead use CSS

### <img>

Indicates that the following src attributes will contain an image (which contains an image format file)

- attributes
    - src=image file address (can be local or website image address)
    - width=width of image
    - height=height of image
        - Note that if you enter both of them, the image’s ratio can be destroyed. Using only one attribute(width or height) is a better way.
    - title=title of image (appears when the mouse hovers on the image)

### <table>

Indicates that data has a form of a table

- main elements
    - <tr>: between this tag will be “one” record
    - <th>: between this tag will be “one” field that is “HEAD” of table
    - <td>: between this tag will be “one” field
        - rowspan attributes: Merge cells from this cell to N rows down cell
        - colspan attributes: Merg cells from this cell to N columns right cell
- <thead>: <tr> and <th> tag inserted in this tag will be the “HEAD” of the table
- <tbody>: <tr> and <td> tag inserted in this tag will be the “BODY” of the table
- <tfoot>: <tr> and <td> tag inserted in this tag will be the “FOOTER” of the table

### <input>

Allows a user to input some informations in a box (or interact with the website)

- attributes
    - type=
        - ”text”: text field
        - “password”: text field, but all inputs are hidden
        - “button”: this only makes button UI that the user can click (but nothing happens [default])
        - “submit”: button that submits the user’s input
        - “radio”: selection tools, but user can choice only one (between range of same name attributes)
        - “checkbox”: selection tools that can choose multiple options
        - “hidden”: can send information to server, but users cannot see directly on the screen (used with name and value attributes)
        - “file”: upload and send files (used with name)
    - name=”{name}”: data name (when you send information to server using <form>)
    - value=”{value}”: sets default value which already written in the input box
    - checked: (works with “radio” and “checkbox”) default value which already chosen
    - onclick=”{JavaScript}”: (works with “button”) choose what happens when button clicks

### <select>

tags that can make a dropdown box (used with <option> tag)

### <option>

makes options in the <select> tag

- attributes
    - value=”{value}”: selection value (when you send information to server using <form>)

### <textarea>

Write strings (<input> that can write really long string information)

- attributes
    - cols=”{number}”: box column size
    - rows=”{number}”: box row size

### <label>

(mainly for information) sets label values to <input> tags

- attributes
    - for=”{label_name}”: sets label’s name

### <form>

all <input>s can interact with server with <form> tag

- attributes
    - action=”{URL}”: where to send a request based on this information
    - method=
        - “get”: get method
            - get request exposes information to URL (can be dangerous)
        - “post”: post method
            - post request does not expose information to URL
    - enctype=”{enctype}”: (used when input type is “file”) choose encryption type

## Some Useful Websites

[HTML Tag History](http://www.martinrinehart.com/frontend-engineering/engineers/html/html-tag-history.html)

[HTML Study | Advanced Web Ranking](https://www.advancedwebranking.com/seo/html-study/)

# attributes

Tags can only indicate what this tag is, but if you add some attributes, you can do additional things with tags!

# History of HTML

GML → SGML → SGMLguid → HTML (a tag added)

# DOCTYPE

acronym of “Document type declaration”

Informs web browser what this file has been written in. (What protocol has been used)

Now it has been integrated to <!DOCTYPE html>

# HTML as information

## <font> - DO NOT USE

can set some font designs to text

HTML is important for information!

design can be done with CSS, so you should not use HTML <font> tags to apply font attributes

### Why <font> has been excluded from HTML?

HTML tags should deliver information about elements.

<font> tag does not indicate any information about texts, but design.

## <meta>

Website page static scope information.

- attributes
    - charset=”{charset}”: sets character encoding type
    - name=
        - “description”: web page description
        - “keywords”: some main keywords of this page
        - “author”: who wrote the web page
    - content=”{content}”: content (related to name)

## Semantic element

tags only for information

### <header>

Indicates that this is HEADER of the page

### <nav>

Indicates that this is the navigation element of the page

### <section>

Defines sections of the page

### <article>

Defines that this is main texts

### <footer>

Indicates that this is FOOTER of the page(privacy, about, etc.)

### other tags

- <aside>: not related to page
- <details>: not rendered information
- <figure>: additional figure or diagram
- <main>: main contents
- <mark>: highlights or references
- <time>: time

## Search Engine Optimization(SEO)

[SEO 기본 가이드: 기본사항 | Google 검색 센터 | 문서 | Google Developers](https://developers.google.com/search/docs/fundamentals/seo-starter-guide?hl=ko)

### use <title>

the title can be updated

### use <meta name=”description” content=””>

This can be used as a page description

### use understandable URL

URL should be short and understandable

### use <canonical> if a different URL has the same contents

or use Redirection (PHP, JAVA, or Python (server))

### make it easy to move between Sites(use hyperlinks)

if you use Javascript or other methods that are not based on HyperLink, the search engine may not detect all sites

### use <img alt=””> to deliver informations about an image

The search engine will use alt attributes to understand images

### use tags to indicate headings

fonts or bold does not deliver any information.

### use robots.txt

protocols that define (which) search engines should (not) access (which) websites

polite request → not for security purposes

- use sitemap.xml
    - xml file that has <url> tags → which pages that website have
    - The search engine can download xml file and understand what pages are inside the website

### REF) Google Search Engine Algorithm: PageRank Algorithm

Google finds which page has been referenced more (based on hyperlinks)

# Other tags

## <meta name=”viewport” content=”width=device-width”>

settings for mobile web

## <iframe>

import outer web page into my web page

### attributes

- src=”{src}”: which source to input
- frameborder=”{num}”: set frame border
- sandbox: for security (defends javascript code and input submit)

### SECURITY ISSUE!

if you use <iframe>, you should be careful of malicious websites that contains bad javascript code! (use sandbox to prevent these)

# HTML5

## <video>

supports video format

### attributes

- controls: can control video (play, stop…)

## <source>

imports video source

### attributes

- src=”{source}”: video source address

## <input>

### attributes

- type=
    - ”number”: integer number
        - min=”{num}” max=”{num}”: from min to max
    - “date”: date (YYYY-MM-DD)
    - “month”: month (YYYY-MM)
    - “week”: week
    - “time”: (hh:mm AM)
    - “email”: email (example@example.com)
    - “search”: search bar (for accessibilities)
    - “url”: URL
    - “range”: range bar appears
        - min=”{num}” max=”{num}”: from min to max
- placeholder=”{string}”: string to render in the input box
- required: if this input box is empty, the request cannot be sent
- pattern: choose the pattern to be submitted
    - [a-zA-Z]: one letter, alphabet only
    - [0-9]: one letter, number only
    - .: any one letter
    - .+: any (more than) one letter

## References

[Can I use... Support tables for HTML5, CSS3, etc](https://caniuse.com/)
