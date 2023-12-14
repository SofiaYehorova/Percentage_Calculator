<!DOCTYPE html>
<html lang="uk">
<head>
<meta charset="UTF-8">
<title>Калькулятор- «Точка беззбитковості»</title>
<style type="text/css">
calculator {
width: 300px;
margin: auto;
padding: 20px;
background-color: #f3f3f3;
border-radius: 20px;
box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.1);
}
display {
width: 100%;
height: 50px;
text-align: right;
margin-bottom: 10px;
padding-right: 10px;
box-sizing: border-box;
border: none;
background-color: #fff;
font-size: 20px;
border-radius: 10px;
}
button {
width: 66px;
height: 40px;
margin: 5px;
display: inline-block;
background-color: #007BFF;
color: white;
text-align: center;
line-height: 40px;
cursor: pointer;
border-radius: 5px;
font-size: 18px;
transition: background-color 0.3s ease;
}
</head>
<body>
 </head>
<body>
<div id="calculator">
<input type="text" id="display" disabled>
<div id="buttons">
<div class="btn-group" role="group" aria-label="Basic example">
  <button type="button" class="btn btn-primary">Left</button>
  <button type="button" class="btn btn-primary">Middle</button>
  <button type="button" class="btn btn-primary">Right</button>
</div>
