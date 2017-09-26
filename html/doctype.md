## DOCTYPE

Html5 Doctype

```
<!DOCTYPE html>
```

Html4 hard-to-remember doctypes

```
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
```

The point of a doctype is twofold.

First, it's to help validators determine what validation rules an HTML validator needs to use when validating the code

Second, a doctype forces Internet Explorer versions 6, 7, and 8 to go into "standards mode"


Ref from [知乎](https://www.zhihu.com/question/21974902)

早期的HTML版本是基于SGML, 因此需要套用SGML的解析规则。DTD的作用在于定义SGML文档的文档类型以便于浏览器解析。HTML5不再基于SGML, 因此不再需要DTD，而是简化为<!DOCTYPE html>， 用来触发不同的浏览器渲染模式。

为了维持对旧版网页的向后兼容性，现代浏览器一般具有多种渲染模式：标准模式，怪异模式（quirks mode）和近乎标准模式（almost standards mode）。详情请移步[Activating Browser Modes with Doctype](https://hsivonen.fi/doctype/)。Henri Sivonen在文中列出了不同的DOCTYPE声明在不同浏览器下的效果。可以看出<!DOCTYPE html>在 IE 6&7 中会触发近乎标准模式（区别仅为表单元格内部的图片布局采用和怪异模式相同的方式处理），在IE8以后的版本以及所有现代浏览器中都会触发标准模式