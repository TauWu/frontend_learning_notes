# Javascript Basic

Js 基础知识

## Try it

- **click-to-show-time** :moon: [source](../../code/javascript/basic/try-it/click-to-show-time.html)

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>Try it Page</title>
        <script>
        function displayDate(){
            document.getElementById("demo").innerHTML=Date();
        }
        </script>
    </head>
    <body>
        <h1>Here is the first javascript program.</h1>
        <p id="demo">Click button and change here.</p>
        <button type="button" onclick="displayDate()">Show datetime</button>
    </body>
</html>
```

- **write-html-stream** :moon: [source](../../code/javascript/basic/try-it/write-html-stream.html)

```html
<!DOCTYPE html>
<html>
    <head> 
        <meta charset="utf-8"> 
        <title>Try it - Write HTML stream</title> 
    </head>
    <body>
        <p>
            JavaScript 能够直接写入 HTML 输出流中：
            </p>
            <script>
            document.write("<h1>这是一个标题</h1>");
            document.write("<p>这是一个段落。</p>");
            </script>
            <p>
            您只能在 HTML 输出流中使用 <strong>document.write</strong>。
            如果您在文档已加载后使用它（比如在函数中），会覆盖整个文档。
        </p>
    </body>
</html>
```

- **action** :moon: [source](../../code/javascript/basic/try-it/action.html)

```html
<!DOCTYPE html>
<html>
    <head> 
        <meta charset="utf-8">
        <title>Try it - Action</title>
    </head>
    <body>
        <h1>Try it - Action</h1>
        <p>
        JavaScript 能够对事件作出反应。比如对按钮的点击：
        </p>
        <button type="button" onclick="alert('Welcome!')">Click me!</button>
    </body>
</html>
```

- **change-html-content** :moon: [source](../../code/javascript/basic/try-it/change-html-content.html)

```html
<!DOCTYPE html>
<html>
    <head> 
        <meta charset="utf-8"> 
        <title>Try it - Change HTML content</title> 
    </head>
    <body>
        <h1>Change HTML content</h1>
        <p id="demo">
        JavaScript 能改变 HTML 元素的内容。
        </p>
        <script>
        function myFunction()
        {
            x=document.getElementById("demo");  // 找到元素
            x.innerHTML="Hello JavaScript! I changed this element.";    // 改变内容
        }
        </script>
        <button type="button" onclick="myFunction()">点击这里</button>
    </body>
</html>
```

- **change-html-src** :moon: [source](../../code/javascript/basic/try-it/change-html-src.html)

```html
<!DOCTYPE html>
<html>
    <head> 
        <meta charset="utf-8"> 
        <title>Try it - Change HTML src</title> 
    </head>
    <body>
        <script>
        function changeImage()
        {
            element=document.getElementById('myimage')
            if (element.src.match("bulbon"))
            {
                element.src="/images/pic_bulboff.gif";
            }
            else
            {
                element.src="/images/pic_bulbon.gif";
            }
        }
        </script>
        <img id="myimage" onclick="changeImage()" src="/images/pic_bulboff.gif" width="100" height="180">
        <p>点击灯泡就可以打开或关闭这盏灯</p>
    </body>
</html>
```

- ****