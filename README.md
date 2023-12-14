<!DOCTYPE html> 
<html lang="en"> 
<head> 
    <meta charset="UTF-8"> 
    <meta http-equiv="X-UA-Compatible" content="IE=edge"> 
    <meta name="viewport" content= 
        "width=device-width, initial-scale=1.0"> 
    <title>Percentage Calculator</title> 
    <link rel="stylesheet" href="style.css" type="text/css" /> 
</head> 
<body> 
    <h1>Percentage Calculator</h1> 
    <div> 
        <!-- Defines a field for entering a number-->
        <h2> What is <input type="number" id="percent" />% of 
            <input type="number" id="num" />? 
        </h2> 
        <!-- onclick event is to call the function when 
            user click on the button-->
        <button onclick="percentage_1()">Calculate</button><br> 
            <!-- Read-only input field to display 
            output and cannot be modified -->
        <input type="text" id="value1" readonly /> 
    </div> 
    <div> 
        <!-- Defines a field for entering a number -->
        <h2><input type="number" id="num1" /> 
            is what Percent of 
            <input type="number" id="num2" />? 
        </h2> 
        <!-- onclick event is to call the function 
            when user click on the button -->
        <button onclick="percentage_2()">Calculate</button> 
          <br> 
        <!-- Read-only input field to display 
            output and cannot be modified -->
        <input type="text" id="value2" readonly /> 
    </div>
    <script type="text/javascript" src="script.js"></script> 
</body> 
</html> 
