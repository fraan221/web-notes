# HTML

## 1. Elements

### Create your first web page by learning about basic elements and tags.

**HTML** = **H**yper**T**ext **M**arkup **L**anguage
It was created by a developer named **Tim Berners-Lee** in 1991.

HTML marks up every piece of content on a web page and defines its type.

HTML is just one piece used to build a web page.

Most web pages use:

1. **HTML:** Create the website skeleton.
2. **CSS:** Modify the website appearance.
3. **JavaScript:** Make it interactive.

The programs we write will be files with the extensions `.html`

#### Elements

An element usually consists of an opening tag, the content, and a closing tag.

A tag is enclosed in angle brackets

```html
<p>Hello World!</p>
```

- `<p>` is the opening tag
- `Hello World!` is the content
- `</p>` is the closing tag

The `<p>` tag tells the browser that the content inside is "paragraph" text

Example of a Basic HTML program that displays a message in the browser

```html
<body>
  <p>👋 I'm a new web developer!</p>
</body>
```

The `<body>` element defines an HTML document's "body" and it's where any content that
we want to display to the user will be held.

> There can only be one <body> element in a file.

#### Indentation

Indenting in HTML code isn't required, but doing is good practice because it makes
your code easier to read and visualize the nesting levels.

The recommend indentation is two `spaces`.

#### Headings

If we want to add a headline to our website that displays a news article.
We use a `<h1>` heading element to display the message and `<p>` for paragraph element

```html
<body>
  <h1>Breaking News 🚨</h1>
  <p>Florida man once evaded arrest by cartwheeling now running for mayor.</p>
</body>
```

There are six levels of heading, from `<h1>` to `<h6>`:

```html
<h1>Heading level 1</h1>
<h2>Heading level 2</h2>
<h3>Heading level 3</h3>
<h4>Heading level 4</h4>
<h5>Heading level 5</h5>
<h6>Heading level 6</h6>
```

> Only one `<h1>` element should be used in a file.

##### Line Break

The `br` break tag adds a line break.

Example

```html
<body>
  <h1>Breaking News</h1>
  <p>
    Florida man robs convenience store with an alligator.<br />Leaves a baby
    Crocs behind.
  </p>
</body>
```

A self-closing tag doesn't need to be closed manually by a closing tag.
It does not have a separate closing `</tag>`

#### Text Formating

Text formatting elements is used to bold sentences, italicize new words,
underline important phrases, and more.

They make default texts look fancier.

Here are common ones:

- `<b>` element to **bold** text
- `i` element to _italicize_ text
- `<u>` element to <u>underline</u> text
- `<s>` element to <s>strikethrough</s> text

Usage

```html
<b>This text is using bold formatting.</b>
<i>This text is using italics formatting.</i>
<u>This text is using underline formatting.</u>
<s>This text is using strikethrough formatting.</s>
```

> The `<b>` element is just for bolding text stylistically;

> HTML also has a `<strong>` element used to convey that the content inside is important, as well as styling it to be bold.

> The tags above are good for learning how to style text with basic HTML, but are no longer best practice.

#### Lists

In HTML exist two types of Lists:

- `<ul>` Unordered lists
- `<ol>` Ordered lists

Also exist `<li>` list item element that goes inside the `<ul>` lists and `<ol>` lists.

For Unordered lists, also known as bullet points, start with the `<ul>` tag and wrap
each time in a `<li>` list item element.

Example

```html
<ul>
  <li>🧺 Go to laundromat.</li>
  <li>🖥 Code for 45 min.</li>
  <li>💅 Take a bubble bath.</li>
</ul>
```

For Ordered lists, also known as numbered lists, we use `<ol>` element.

Example

```html
<ol>
  <li>🧺 Go to laundromat.</li>
  <li>🖥 Code for 45 min.</li>
  <li>💅 Take a bubble bath.</li>
</ol>
```

#### Links

Links are integral to the idea of internet. They are how users connect to others
sites and navigate the web.

We can use the `<a>` anchor element. This link tag allow us to add a hyperlink to
a piece of text.

Example

```html
<a href="https://archive.org/web">Internet Archive</a>
```

An `href`, or hyperlink reference, is a reference or pointer to another website
that is linked in our HTML.

> This can also be used to point to an email or phone number using a `mailto:`, `tel:`, or `sms:` parameter.

```html
<a href="mailto:frankie@gmail.com">📧</a>
<a href="tel:212-555-2368">🤙</a>
<a href="sms:320-250-HTML">💬</a>
```

#### Images

The `<img>` image element is another self-closing tag, so it doesn't have a closing tag.

```html
<p>Here's a cute pic:</p>
<img src="https://i.redd.it/5unn16axx1v81.jpg" />
```

- `src` attribute, which stands for "source", specifies the file path of the image
- `"https://i.redd.it/5unn16axx1v81.jpg"` is the image path

---

## 2. Structure

### Learn more about HTML structure, attributes, and classes vs id.

#### HTML Structure

The `<!DOCTYPE html>` is the document type declaration that appears at the top of a **.html** file and tells the browser that our file is written in HTML5.

The `<!DOCTYPE html>` doesn't have a closing tag, while `<html>` does.

Inside `<html>`, there should be two elements:

- `<head>` contains all the info for your browser that's not visible on the page.
- `<body>` contains all of the content that you will end up seeing on the page.

The `<title>` element goes in the `<head>` and assigns text to the browser tab.

##### Parents & Children

The elements in HTML files are arranged much like a family tree.
Most individual elements can be parents with one or more child elements.

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My Website</title>
  </head>
  <body>
    <p>Well, <i>howdy</i> there!</p>
  </body>
</html>
```

- `<head>` and `<body>` are children of `<html>`.
- `<title>` is the child of `<head>`.
- `<i>` is child of `<p>` and grandchild of `<body>`.

##### Siblings

Elements can also be siblings if they share a direct parent element.

```html
<body>
  <ul>
    <li>🍄 Mario</li>
    <li>🐢 Luigi</li>
  </ul>
</body>
```

The two <li> elements are siblings because both are children of the same parent, the <ul> element.

#### Comments

Inline comments:

```html
<!-- I am a comment. -->
```

Multi-line comments:

```html
<!--
    I am a multi-line comment.
-->
```

It isn't recommend that you be excessive with comments. They should be used sparingly and removed when no longer needed

#### Attributes

Attributes are additional settings that we can use to customize an element.

Examples

```html
<ol type="a">
  <li>Power ⚡</li>
  <li>Courage 🔥</li>
  <li>Wisdom 🦉</li>
</ol>
```

```html
<ol type="i">
  <li>Power ⚡</li>
  <li>Courage 🔥</li>
  <li>Wisdom 🦉</li>
</ol>
```

##### Attributes in Image Tag

`img` can use `alt` attribute to make our images more accessible.

```html
<img
  alt="pixel girl using a laptop"
  src="https://www.codedex.io/images/tier1.png"
/>
```

##### Attribute in Anchor Tag

`a` tag can use `target` attribute to make the link open in a new browser tab.

```html
<a href="https://www.codedex.io/" target="_blank">Codédex</a>
```

#### Classes and IDs

An element can be assigned multiple `class` values in the form of a space-separated list.

```html
<p class="first-value second-value third-value">Hello, World</p>
```

Each element can only have one `id` value with no spaces. Every `id` value should be unique in the entire page.

```html
<p id="value">Hello, World</p>
```

The `id` value can be used to link to another part of the same page. This can be matched with an `<a>` anchor element's `href` attribute via a `#` hashtag symbol, followed by the identifier used for the `id`.

```html
<a href="#bsas">Link to Buenos Aires</a>

<h2 class="city" id="bsas">Buenos Aires</h2>
```

One `id` can be assigned to a single element, a `class` can be assigned to many.

```html
<h2 class="city" id="medellin">Medellín 🇨🇴</h2>
<h2 class="city" id="lisbon">Lisbon 🇵🇹</h2>
<h2 class="city" id="bali">Bali 🇮🇩</h2>
```

Note: The values for the `class` and `id` attributes must always be lowercase. If their name is made of multiple words, they should be separated by dashes `-`.

#### Division Element

The `<div>` element is kind of like a generic container with no particular meaning. This element and the `class` and `id` attributes can go hand in hand.

Example

```html
<div class="page-section" id="about-me">
  <h2>About Me</h2>
  <p>Ness is an aspiring web developer!</p>
</div>

<div class="page-section" id="social-media">
  <h2>Social:</h2>
  <ul>
    <li>GitHub</li>
    <li>Twitter</li>
    <li>LinkedIn</li>
  </ul>
</div>
```

The `<div>` element is used to group content and be labeled by the `class` and `id` attributes.

---

## 3. Forms

### Take input from the user with forms.

Creating a Form in HTML

```html
<form action="" method="">
  <!-- More code will go here -->
</form>
```

Common attributes in the `<form>` element:

- The `action` attribute that says where the form data should go after it is submitted.
- The `method` attribute for how the form data is processed.

#### Inputs

The `<input>` element is used as an interactive control for entering data.
A `type` attribute is used to determine the kind of input to use.

##### Most Common `types` of Input

- `text` value

```html
<form>
  <input type="text" />
</form>
```

- `submit` value

```html
<form>
  <input type="submit" />
</form>
```

**Note:** The `<input>` element uses a closing-self tag.

[The complete list of Input Types](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/input#input_types)

##### Input types: Email & Password

Examples

```html
# Email
<input type="email" />
# This tells the form to expect a text input with the typical email syntax
(including the @ symbol). # Password
<input type="password" />
#Dots will replace the text that would otherwise appear in the text box:
```

### Input Validation

The `email` type checks if the submitted input is a valid email address.
The `password` type can also validate the data in it, using `minlenght` and `maxlenght` attribute we can check the validation of a password enters the user.

```html
<input type="password" minlength="4" maxlength="10" />
```

**Note:** The `minlenght` and `maxlenght` can also be assigned for more types of inputs.

### Required data

The `required` attribute makes the element marked to be submitted no matter what.

```html
<form method="dialog">
  Name: <input type="text" required /> <br /><br />
  Favorite Color: <input type="text" />
  <input type="submit" />
</form>
```

**Note:** In this example, if we not include any value to `name` input we can't send the form. Because the input of `name` has the `required` attribute inside.

##### Input types: Number, Checkbox & Radio

**Number:**

```html
<input type="number" />
```

The `type` number also has attributes to use:

Setting this attribute in the input makes the buttons arrows "Up" and "Down" change the value from 1 to the number selected (In this case 2).

```html
<input type="number" step="2" />
```

Using this attribute makes the input how high or low can go.

```html
<input type="number" min="1" max="42" />
```

**Checkbox:**

The `checkbox` type renders as a box that is ticked off to mark the input as "finished" or "complete."

```html
<h3>Favorite Movie Genres</h3>
<input type="checkbox" /> Action<br />
<input type="checkbox" /> Sci-Fi<br />
<input type="checkbox" /> Rom-Com<br />
<input type="checkbox" /> K-Drama<br />
<input type="checkbox" /> Documentary<br />
```

**Radio:**

Like with checkboxes, radio buttons are lists of options. However, only one option can be selected.

```html
<h3>Which do you think?</h3>
<input type="radio" name="option" /> Yanny
<br />
<input type="radio" name="option" /> Laurel
```

##### Textareas

The `<textarea>` element renders as a plain, mini-text editor on the web page.

```html
<textarea
  id="data-entry"
  rows="7"
  cols="42"
  placeholder="Enter some data here!"
></textarea>
```

Textarea attributes:

- `rows`: The amount of visible rows, or text lines (defaulting at 2).
- `cols`: The number of visible columns in average character widths (defaulting at 20).
- `placeholder`: Some default text meant to explain what kind of data should be entered.

The `required` attribute can be applied to the `<textarea>`element, too.

##### Form Labels

The `<label>` can be used in forms to associate pieces of text with form controls and inputs.

```html
<form>
  <label>Book Title: </label><input type="text" /> <br /><br />
  <label>Author: </label><input type="text" /> <br /><br />
  <input type="submit" />
</form>
```

Associate label with form inputs

```html
<form>
  <label for="title">Book Title: </label><input type="text" id="title" />
  <br /><br />
  <label for="author">Author: </label><input type="text" id="author" />
  <br /><br />
  <input type="submit" />
</form>
```

Implicitly association

```html
<form>
  <label>Book Title: <input type="text" /></label>
  <label>Author: <input type="text" /></label>
</form>
```

---

## 4. Semantic HTML

### Improve the foundation of any web page with semantic elements.
