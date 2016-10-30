---
title: Component Driven Design in Javascript
layout: post
---

I was first introduced to the idea of component driven design when I was learning PHP. What this means essentially is that instead of having all your html in one file _(ala most bootstrap templates / static html sites)_, you would separate the most used sections of your webpage _(header, footer, etc.)_ into their own files, and include them in your other pages. Something like this; 

```php
<!DOCTYPE html>
<html>
    <head>
        <?php include 'head.php' ?>
    </head>
    <body>
        body content
        <footer>
            <?php include 'footer.php' ?>
        </footer>
    </body>
</html>
```

### Benefits 
Now immediately after looking at this example, the most obvious benefit should make itself apparent to you. To define this benefit, I'm going to borrow a term from database design; **Data Integrity**. What this means is that by only having your data in one place _(and not multiple footers spread across multiple files)_, you assure that the same data is presented across the web page. In addition to that, this makes it easier for the developer, because you only have to edit the content once. Really, why wouldn't you be doing this? 

### Drawbacks
Sure, if you're using PHP, this should be the way you structure your files. Anything else is inefficient. However if you weren't planning on using PHP, HTML didn't really have any way of seperating your files into components. 
