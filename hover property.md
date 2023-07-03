I learned that if two or more elements have same structure like same childs with same class name and everthing exactly. So I have a thought that when you hover over a element
if the property changes then the property of other element should change having same class name but it do not happens

run this code and check : <br>

HTML

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <div class="first">
        <div class="f_child">aaa</div>
        <div class="s_child">bbb</div>
      </div>
      <div class="first">
        <div class="f_child">aaa</div>
        <div class="s_child">bbb</div>
      </div>
    </div>
  </body>
</html>
```
CSS 

```
*{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

.container{
    height: 100vh;
    width: 100vw;
    background-color: red;
    display: flex;
    justify-content: space-between;
}


.first
{
    padding: 10px;
  margin: 20px;
  background-color: blue;
  width: 100%;
  display: flex;
  flex-direction: column;
}

.f_child{
    height: 50%;
    background-color: green;
    margin: 10px 0;
}
.s_child{
    height: 50%;
    background-color: green;
}

.first:hover{
    background-color: black;
}

.first .f_child:hover{
    background-color: brown;
}
```
