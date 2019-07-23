<!DOCTYPE html>
<html lang="en-us">
<head>
<meta charset="utf-8">
<title>****</title>
<script>
/* Input: First function sends list of numbers and multiplier to second function
* Processing: Second function multiplies numbers in list by the given multiplier
* Output: New list containing product of the calculations is displayed for user
*/
function testArray() {
var list = [5, 6, 18, 2];
var multiplier = 3;
var products = multiply(list, multiplier);

document.getElementById('output').innerHTML = products;
}

function multiply(list, multiplier) {
var products = [];
for(i = 0; i < list.length; i++) {
products += list[i] * multiplier + ", ";
}
return products;
}
</script>
</head>

<body>
<input type='button' onclick='testArray()' value='Click Me' />

<div id='output'></div>
</body>
</html>
