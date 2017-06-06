# Sass: Nest CSS with Sass

Sass allows nesting of CSS rules, which is a useful way of organizing a style sheet.

Normally, each element is targeted on a different line to style it, like so:
```css
    nav {
      background-color: red;
    }

    nav ul {
      list-style: none;
    }

    nav ul li {
      display: inline-block;
    }
```
For a large project, the CSS file will have many lines and rules. This is where nesting can help organize your code by placing child style rules within the respective parent elements:
```css
    nav {
      background-color: red;

      ul {
        list-style: none;

        li {
          display: inline-block;
        }
      }
    }
```
Use the nesting technique shown above to re-organize the CSS rules for both children of .blog-post element. For testing purposes, the h1 should come before the p element.

# Solution:
```html

<style>
  .blog-post {
    h1 {
      text-align: center;
      color: blue;
    }
      p {
          font-size: 20px;
        }
    }
  }
</style>

<div class="blog-post">
  <h1>Blog Title</h1>
  <p>This is a paragraph</p>
</div>
```
