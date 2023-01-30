# Independent-Project-10-DOM-Manipulation #

[Source](https://www.w3schools.com/js/js_htmldom.asp)

## DOM MANIPULATION ##

___
---

### The DOM Programming Interface ###

#### Task 1: Change the content of the `<p>` element with id="demo".####

```
<!DOCTYPE html>
<html>
<body>

<h2> Let's practice! </h2>
< p id = "demo"> </p>

<script>
document.getElementById("demo").innerHTML = "Here I can add whatever new content I want."
</script>

</body>
</html>
```
___
---

### Finding HTML Element by Id ###

#### Task 2: Find an element in the DOM, usign the element id.####

```
<!DOCTYPE html>
<html>
<body>

<h2> JavaScript HTML DOM </h2>

<p id="intro"> Finding HTML Elements by Id </p>
<p> This example demonstrates the <b>getElementById</b> method. </p>
<p id = "demo"></p>

<script>
const element = document.getElementById("intro");

document.getElementById("demo").innerHTML = "The text from the intro paragraph is: " + element.innerHTML;
</script>
</body>
</htm>
```
___
---

### Finding HTML Elements by Tag Name ###

#### Task3: Find all `<p>` elements by Tag Name. ####

```
<!DOCTYPE html>
<html>
<body>

<h2> JavaScript HTML DOM </h2>

<p> Finding HTML elements by Tag Name. </p>
<p> This example demonstrates the <b>getElementsByTagName</b> method.</p>

<p id="demo"></p>

<script>
const element = getElementByTagName("p");
document.getElementById("demo").innerHTML = "The text in this paragraph (index 0) is: " + element[0].innerHTML;

</script>

</body>
</html>

```

___

#### Task 4: Find the element with id="main", and then find all the `<p>` elements inside "main". ####

```
<!DOCTYPE html>
<html>
<body>

<h2> JavaScript HTML DOM </h2>

<div id = "main">
<p> Finding HTML elements by Tag Name </p>
<p> This example demonstrates the <b>getElementsByTagName</b> method.</p>
</div>

<p id = "demo"> </p>

<script>
const x = document.getElementById("main");
const y = x.getElementsByTagName("p");

document.getElementById("demo").innerHTML = "The first paragraph (index 0) inside "main" is: " + y[0].innerHTML;

</script>

</body>
</html>

```
___
---


### Finding HTML Elements by Class Name ###

#### Task 5: Use `getElementsByClassName()` to return a list of all elements with class = "intro". ####

```
<!DOCTYPE html>
<html>
<body>

<h2> JavaScript HTML DOM </h2>

<p> Finding HTML Elements By Class Name. </p>
<p class = "intro"> Hello, World! </p>
<p class = "intro"> This example demonstrates the <b>getElementsByClassName</b> method.</p>

<p id = "demo"></p>

<script>
const x = document.getElementsByClassName("intro");
document.getElementById("demo").innerHTML = "The first paragraph (index 0) with class = "intro" is: " + x[0].innerHTML;
</script>

</body>
</html>
```

___
---

### Finding HTML Elements by CSS Selectors ###

#### Task 6: Use `querySelectorAll()` method to find all `<p>` elements with class="intro". ####

```
<!DOCTYPE html>
<html>
<body>

<h2> JavaScript HTML DOM </h2>

<p> Finding HTML Elements by Query Selector </p>
<p class = "intro"> Hello, world! </p>
<p class = "intro"> This example demonstrates the <b>querySelectorAll</b> method. </p>

<p id = "demo"></p>

<script>

const x = document.querySelectorAll(".intro")
document.getElementById("demo").innerHTML = "The first paragraph (index 0) with class intro is: " + x[0].innerHTML

</script>

</body>
</html>

```

___
---

### Finding HTML Elements by HTML Object Collections ###

#### Task 7: Finds the form element with id="frm1", in the forms collection, and displays all element values. ####

```
<!DOCTYPE html>
<html>
<body>

<h2> JavaScript HTML DOM </h2>
<p> Finding HTML Elements using <b>document forms</b>.</p>

<form id = "frm1" action = "/action_page.php">
    First name: <input type = "text" name = "fname" value = "Donald"> <br>
    Last name: <input type = "text" name = "lname" value = "Duck"> <br><br>
    <input type: "submit" value="Submit">
    </form>

<p> These are the values for each element in the form: </p>

<p id= "demo"> </p>

<script>
const x = document.forms("frm1");
let text = "";
for (let i=0; i < x.length; i++){
    text += x.elements.value + "</br>";
}
document.getElementById("demo").innerHTML = text;
</script>

</body>
</html>

```

___
---

### JavaScript HTML DOM - Changing HTML ###

#### Task 8: Modify the content of an HTML element `<p>` by using the innerHTML property. ####

```
<!DOCTYPE html>
<html>
<body>

<h2> JavaScript can Change HTML </h2>

<p id = "p1"> Hello, World! </p>

<script>
document.getElementById("p1").innerHTML = "new text";

</script>

<p> The paragraph above was changed by a script. </p>
</body>
</html>

```

#### Task 9: Change the content of the `<h1>` element. ####

```
<!DOCTYPE html>
<html>
<body>

<h2 id = "id01"> Old heading </h2>

<script>
const element = document.getElementById("id01");
element.innerHTML = "new heading";
</script>

</body>
</html>

```

---
___

### Changing the Value of an Attribute ###

#### Task 10: Change the value of the src attribute of an `<img>` element.

```
<!DOCTYPE html>
<html>
<body>

<h2> JavaScript HTML DOM </h2>
<img id = "image" scr= "smile.gif" width = "160" height = "120">

<script>
document.getElementById("image").src = "landscape.jpg";
</script>

<p> The original image was smiley.gif, but the script has changed it to landscape.jpg.</p>

</body>
</html>

```
___
---

###
