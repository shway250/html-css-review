# HTML/CSS Review

This is a review of your working knowledge of HTML and CSS. Note that this review is designed to help you recall and familiarize yourself with technical concepts.

## Getting Started

* Fork and clone this repository
* Answer the following questions by...
  * Opening this file in Sublime
  * Answering the questions via Markdown. Feel free to refer to this [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* Commit your changes
* Make a pull request for submission

---

## HTML

1.) Create a valid, empty HTML page with the necessary tags.

```html
<!DOCTYPE html>
<html>
<head>
	<title></title>
</head>
<body>

</body>
</html>
```

2.) What are the differences between these tags?

```html
<!-- Tag 1 -->
<img src="images/me.jpg" alt="My profile image">

<!-- Tag 2 -->
<div></div>
```

```
Explain here.
```
The img tag is a self closing tag, whereas an opening div tag requires a closing div tag.
---

## CSS

1.) Compare and contrast the following ways to add CSS to HTML elements.

```html
<!-- Inline CSS -->
<div style="background-color: red;"></div>

<!-- Internal style sheet -->
<style type="text/css">
  div {
    background-color: red;
  }
</style>

<!-- External style sheet (not shown) -->
<link rel="stylesheet" type="text/css" href="css/style.css">
```

```
Explain here
```
Inline CSS can be useful for adding style to a single element, but it makes programatic styling very difficult because you can only change one element at a time. An internal stylesheet solves some of these probems since you can apply styles to multiple types of tags, or classes, but it can cluster up your html file. The external style sheet allows you to style programatically, and easily change styles responsively using javascript (which is also possible with the internal style sheet, but the external style sheet is preferred).

2.) Below are some different CSS selectors. Use CSS comments to describe what each selector will do.

```css
/* this will curve the border of the div 50% the way to being a circle*/
div {
  border-radius: 50%;
}

/* this will make p tags with the class "header" have a font size of 18px */
.header p {
  font-size: 18px;
}

/* this will make elements with the class "footer" be flush with the bottom of the page and make their position absolute (so always on the bottom of the page) */
.footer {
  position: absolute;
  bottom: 0;
}

/* this will make elements with the class "splash-image" be the background image for the page. The image will cover the whole of the background.*/
.splash-image {
  background-image: url("../images/ocean.jpg");
  background-size: cover;
  width: 100%;
}
/* This will make elements with the class "ninja" disapear when the mouse hovers over them. The color: black tag won't do anything since display is set to none. */
.ninja:hover {
  display: none;
  color: black;
}
```


---

## Licensing
1. All content is licensed under a CC-BY-NC-SA 4.0 license.
2. All software code is licensed under GNU GPLv3. For commercial use or alternative licensing, please contact legal@ga.co.
