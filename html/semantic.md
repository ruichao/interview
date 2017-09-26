## Semantic markup

### New HTML5 markup tags

* header
* footer
* nav
* section
* article
* aside

Works great in IE9 above, Firefox, Chrome, Opera and Safari.

Fallback

```
<!-- [if lte IE 8]>
<script>
  document.creatElement("header");
  document.creatElement("footer");
  document.creatElement("nav");
  document.creatElement("section");
  document.creatElement("article");
  document.creatElement("aside");
</script>
<![endif] -->
```


### old tag with new meaning

* dl 

In previous versions of HTML, the `<dl>` element defines a definition list. Now in HTML5 `<dl>` defines a description list.

