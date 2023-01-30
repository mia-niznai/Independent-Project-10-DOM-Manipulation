# Independent-Project-10-DOM-Manipulation #

[Source](https://www.w3schools.com/js/js_htmldom.asp)

## DOM MANIPULATION ##

### Task 1: Change the content of the `<p>` element with id="demo".###

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

### Task 2: Find an element in the DOM, usign the element id.###

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

### Task3: Find all `<p>` elements by Tag Name. ###

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

---
___

### Task 4: Find the element with id="main", and then find all the `<p>` elements inside "main".

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

### Task 5: Use `getElementsByClassName()` to return a list of all elements with class = "intro". ###

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

### Task 6: Use `querySelectorAll()` method to find all `<p>` elements with class="intro". ###

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

### Task 7: Finds the form element with id="frm1", in the forms collection, and displays all element values. ###