<!DOCTYPE html>
<html>
<head>
  <title>SSC MCQ Test</title>
  <style>
    body { font-family: Arial; padding: 20px; }
    .question { margin-bottom: 15px; }
    button { padding: 10px 15px; }
  </style>
</head>
<body>

<h2>SSC Practice MCQ</h2>

<form id="quiz">

<div class="question">
1. भारत की राजधानी क्या है?<br>
<input type="radio" name="q1" value="0"> मुंबई<br>
<input type="radio" name="q1" value="1"> नई दिल्ली<br>
<input type="radio" name="q1" value="0"> कोलकाता
</div>

<div class="question">
2. 2 + 2 = ?<br>
<input type="radio" name="q2" value="0"> 3<br>
<input type="radio" name="q2" value="1"> 4<br>
<input type="radio" name="q2" value="0"> 5
</div>

<button type="button" onclick="check()">Submit</button>
</form>

<p id="result"></p>

<script>
function check(){
  let score = 0;
  if(document.querySelector('input[name="q1"]:checked')?.value=="1") score++;
  if(document.querySelector('input[name="q2"]:checked')?.value=="1") score++;
  document.getElementById("result").innerHTML = "Score: " + score;
}
</script>

</body>
</html>
