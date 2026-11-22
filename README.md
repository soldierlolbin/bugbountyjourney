# Web Application Layout

No two web applications are identical. Businesses create web applications for a multitude of uses and audiences. Web applications are designed and programmed differently, and back-end infrastructure can be set up in many different ways. It is important to understand the various ways web applications can run behind the scenes, the structure of a web application, its components, and how they can be set up within a company's infrastructure.

Web application layouts consist of many different layers that can be summarized with the following three main categories:

| Category | Description |
| :--- | :--- |
| **Web Application Infrastructure** | Describes the structure of required components, such as the database, needed for the web application to function as intended. Since the web application can be set up to run on a separate server, it is essential to know which database server it needs to access. |
| **Web Application Components** | The components that make up a web application represent all the components that the web application interacts with. These are divided into the following three areas: UI/UX, Client, and Server components. |
| **Web Application Architecture** | Architecture comprises all the relationships between the various web application components. |

---

## Web Application Infrastructure

Web applications can use many different infrastructure setups. These are also called models. The most common ones can be grouped into the following four types:

* Client-Server
* One Server
* Many Servers - One Database
* Many Servers - Many Databases

---

## Web Application Components

Each web application can have a different number of components. Nevertheless, all of the components of the models mentioned previously can be broken down into:

* **Client**
* **Server**
  * Webserver
  * Web Application Logic
  * Database
* **Services (Microservices)**
  * 3rd Party Integrations
  * Web Application Integrations
* **Functions (Serverless)**

---

## Web Application Architecture

The components of a web application are divided into three different layers (AKA Three-Tier Architecture).

| Layer | Description |
| :--- | :--- |
| **Presentation Layer** | Consists of UI process components that enable communication with the application and the system. These can be accessed by the client via the web browser and are returned in the form of HTML, JavaScript, and CSS. |
| **Application Layer** | This layer ensures that all client requests (web requests) are correctly processed. Various criteria are checked, such as authorization, privileges, and data passed on to the client. |
| **Data Layer** | The data layer works closely with the application layer to determine exactly where the required data is stored and can be accessed. |

---

## URL Encoding

An important concept to learn in HTML is URL Encoding, or percent-encoding. For a browser to properly display a page's contents, it has to know the charset in use. In URLs, for example, browsers can only use ASCII encoding, which only allows alphanumeric characters and certain special characters. Therefore, all other characters outside of the ASCII character set have to be encoded within a URL. URL encoding replaces unsafe ASCII characters with a `%` symbol followed by two hexadecimal digits.

For example, the single-quote character `'` is encoded to `%27`, which can be understood by browsers as a single quote. URLs cannot have spaces in them and will replace a space with either a `+` (plus sign) or `%20`. Some common character encodings are:

| Character | Encoding |
| :--- | :--- |
| `space` | `%20` |
| `!` | `%21` |
| `"` | `%22` |
| `#` | `%23` |
| `$` | `%24` |
| `%` | `%25` |
| `&` | `%26` |
| `'` | `%27` |
| `(` | `%28` |
| `)` | `%29` |

---

## Cascading Style Sheets (CSS)

CSS (Cascading Style Sheets) is the language used alongside HTML to format and set the style of HTML elements. Like HTML, there are several versions of CSS, and each subsequent version introduces a new set of capabilities that can be used for formatting HTML elements. Browsers are updated alongside it to support these new features.

### Example

At a fundamental level, CSS is used to define the style of each class or type of HTML element (`body` or `h1`), such that any element within that page would be represented as defined in the CSS file. This could include the font family, font size, background color, text color and alignment, and more.

```css
body {
  background-color: black;
}

h1 {
  color: white;
  text-align: center;
}

p {
  font-family: Helvetica;
  font-size: 10px;
}
```

As previously mentioned, this is why we may set unique IDs or class names for certain HTML elements so that we can later refer to them within CSS or JavaScript when needed.

**Syntax:** CSS defines the style of each HTML element or class between curly brackets `{}` within which the properties are defined with their values (i.e., `element { property: value; }`).

Each HTML element has many properties that can be set through CSS, such as `height`, `position`, `border`, `margin`, `padding`, `color`, `text-align`, `font-size`, and hundreds of other properties. All of these can be combined and used to design visually appealing web pages.

CSS can be used for advanced animations for a wide variety of uses, from moving items all the way to advanced 3D animations. Many CSS properties are available for animations, like `@keyframes`, `animation`, `animation-duration`, `animation-direction`, and many others. You can read about and try out many of these animation properties online.

### Usage

CSS is often used alongside JavaScript to make quick calculations, dynamically adjust the style properties of certain HTML elements, or achieve advanced animations based on keystrokes or the mouse cursor location.

---

## JavaScript

JavaScript is one of the most used languages in the world. It is mostly used for web development and mobile development. JavaScript is usually used on the front end of an application to be executed within a browser. Still, there are implementations of back-end JavaScript to develop entire web applications, like Node.js.

While HTML and CSS are mainly in charge of how a web page looks, JavaScript is usually used to control any functionality that the front-end web page requires. Without JavaScript, a web page would be mostly static and would not have much functionality or interactive elements.

### Example

Within the page source, JavaScript code is loaded with the `<script>` tag, as follows:

```html
<script type="text/javascript">
  // JavaScript code
</script>
```

A web page can also load remote JavaScript code with `src` and the script's link as follows:

```html
<script src="./script.js"></script>
```

An example of basic use of JavaScript within a web page is the following:

```javascript
document.getElementById("button1").innerHTML = "Changed Text!";
```

The above example changes the content of the `button1` HTML element. From here on, there are many more advanced uses of JavaScript on a web page. The following shows an example of what the above JavaScript code would do when linked to a button click:

> Original Text → **Changed Text!**

As with HTML, there are many sites available online to experiment with JavaScript; one example is **JSFiddle**, which can be used to test JavaScript, CSS, and HTML and save code snippets. JavaScript is an advanced language, and its syntax is not as simple as HTML or CSS.

### Usage

Most common web applications heavily rely on JavaScript to drive all needed functionality on the web page, like updating the web page view in real time, dynamically updating content in real time, accepting and processing user input, and many other potential functionalities.

JavaScript is also used to automate complex processes and perform HTTP requests to interact with the back-end components and send and retrieve data, through technologies like AJAX.
