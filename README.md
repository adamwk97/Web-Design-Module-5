Link to website -> http://adamwk97.epizy.com

For this week's assignment, I implemented a form using HTML to ask the input of a State and use that input to return if it is a democratic,
republican or swing state. I also used Java to create a "ValidateForm" function to make sure the form works properly and so that users 
cannot enter blanks or incorrect state names. 

As for the wireframe, I simply used relevant images with the American Flag and a democratic map of the United States so as to fit 
the theme of what the website does with the user input. 

My code looks like: 
```
<html>
<head>
<script>
function validateForm() {
    var x = document.forms["myForm"]["state"].value;
    if (x==null || x=="") {
        alert("Please enter a state");
        return false;
    } else if (x=="California" || x=="Oregon || (etc.)){
        System.out.println("Democrat")
    }else if (x=="Florida" || x=="Pennsylvania" || (etc.)){
	      System.out.println("Swing");
  ) else if (x=="Texas"||x=="Oklahoma" || (etc..)){
        System.out.println("Republican")
}
</script>
</head>
<body>
<form name="myForm" action="demo_form.php" onsubmit="return validateForm()" method="post">
State: <input type="text" name="state">
<input type="submit" value="Submit">
</form>
</body>
</html>
```
