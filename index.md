<!DOCTYPE html>
<html>
  <title>Interpolation</title>
  <head>
    <style>
      .main{
        text-align: center;
        padding: 70px;
      
      }
      .button{
        width: 250px;
        height: 50px;
        font-size: 18px;
      }
    </style>
  </head>
<body>

<div class="main">
  x1: <input type="text" name="x1" id="x1">
  y1: <input type="text" name="y1" id="y1"><br>
  x2: <input type="text" name="x2" id="x2">
  y2: <input type="text" name="y2" id="y2"><br>
  x3: <input type="text" name="x1" id="x3">
  y3: <input type="text" name="x3" id="y3" readonly><br>
  <button type="submit" class="button" onclick="myFunction()">Hesapla</button>

<p>Değerleri girin ve interpolasyonu hesaplayın.</p>
</div>

<script>
function myFunction() {
  var x1 = document.getElementById("x1").value;
  var y1 = document.getElementById("y1").value;
  var x2 = document.getElementById("x2").value;
  var y2 = document.getElementById("y2").value;
  var x3 = document.getElementById("x3").value;

  var answer = ((x2-x3)/(x2-x1))*y1 + ((x1-x3)/(x1-x2))*y2
  document.getElementById("y3").value = answer;
}
</script>

</body>
</html>
