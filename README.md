# Jquery-starter

### Table of Contents

| No. | Questions |
| --- | --------- |
|   | **Jquery basics** |
|1  | [What is JavaScript?](#What-is-JavaScript) |
|2  | [What is jQuery and Why use jQuery?](#What-is-jQuery-and-Why-use-jQuery) |
|3  | [Install jQuery OR import jQuery?](#Install-OR-Import-jQuery) |
|4  | [The Document Object Model(DOM)](#The-Document-Object-Model(DOM)) |
|5  | [jQuery Selectors](#jQuery-Selectors) |
|6  | [jQuery Methods](#jQuery-Methods) |
|7  | [jQuery Events](#jQuery-Events) |
|8  | [jQuery Effects](#jQuery-Effects) |
|9 | [jQuery UI](#jQuery-UI) |
|10 | [Where not to use jQuery?](#Where-not-to-use-jQuery) |

1. ### What is JavaScript?
-> To make web pages dynamic we use javascript. <br>
-> It's basically a scripting language. <br>
-> Adding validation at front end.<br>
-> call any api to fetch data.
```javascript
<!DOCTYPE html>
<html>

<head>
    <script>
        function changeColor() {
            document.getElementById("myDiv").style.backgroundColor = 'green';
        }
    </script>
    <style>
        #myDiv {
            width: 100px;
            height: 100px;
            background-color: red;
        }
    </style>
</head>

<body>
    <div id="myDiv">My div object</div>
    <button onclick="changeColor()">click me</button>
</body>

</html>
```


2. ### What is jQuery and Why use jQuery?
-> JQuery is lightweight 
-> Supported by all the browser
-> Easy to Use
-> large support community
-> Save development time.
```javascript
<!DOCTYPE html>
<html>

<head>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script>
        function changeColor() {
            $('#myDiv').css('backgroundColor', 'blue')
        }
    </script>
    <style>
        #myDiv {
            width: 100px;
            height: 100px;
            background-color: red;
        }
    </style>
</head>

<body>
    <div id="myDiv">My div object</div>
    <button onclick="changeColor()">click me</button>
</body>

</html>
```
#javascript api call
```javascript
function loadDoc() {
  var xhttp;
  if (window.XMLHttpRequest) {
    // code for modern browsers
    xhttp = new XMLHttpRequest();
    } else {
    // code for IE6, IE5
    xhttp = new ActiveXObject("Microsoft.XMLHTTP");
  }
  xhttp.onreadystatechange = function() {
    if (this.readyState == 4 && this.status == 200) {
      document.getElementById("demo").innerHTML = this.responseText;
    }
  };
  xhttp.open("GET", "ajax_info.txt", true);
  xhttp.send();
}
```
#jquery api call
```javascript
$.ajax({
    method: "GET",
    url: "test.js" })
  .done(function() {
    alert( "success" );
  })
  .fail(function() {
    alert( "error" );
  })
```

3. ### Install OR Import jQuery?

4. ### The Document Object Model(DOM)?

5. ### jQuery Selectors?

6. ### jQuery-Methods?

7. ### jQuery Events?

8. ### jQuery Effects?

9. ### jQuery UI?

10. ### Where not to use jQuery?
