<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
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
        <button onclick="percentage_2()">Calculate</button><br>
        <!-- Read-only input field to display 
            output and cannot be modified -->
        <input type="text" id="value2" readonly />
    </div>
    <script type="text/javascript" src="script.js"></script>
</body>
</html>
<style>
    /* A margin and padding are provided 0 
    box-sizing border box is used to include 
    padding and border in the total width 
    and height of the element, and font-family 
    can be specified by the user */
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: 'Courier New', Courier, monospace;
    }
    /* The user display allows you to specify the
    background colour and height. The 
    display:flex property, which is aligned at the
    centre, is used to fill available free space 
    or to shrink them to prevent overflow. */
    body {
        background-color: #F0FFFF;
        background: #images/download.jpeg;
        min-height: 500vh;
        display: flex;
        flex-direction: column;
        flex: auto;
        justify-content: center;
        align-items: center;
    }
    /* font-weight Specifies weight of glyphs 
    in the font, their degree of blackness or 
    stroke */
    h1 {
        font-weight: 900;
        margin-bottom: 12px;
    }
    div {
        width: 480px;
        background-color: #87CEEB;
        margin: 12px 0;
        padding: 24px;
        text-align: center;
        box-shadow: 2px 2px 8px 2px #aaa;
    }
    input[type=number] {
        width: 84px;
        font-size: 18px;
        padding: 8px;
        margin: 0px 8px 8px 8px;
    }
    /* The text-transform:uppercase property 
    causes characters to be raised to uppercase. 
    The button's font-weight, font-size, and 
    cursor type can be customised by the user. */
    button {
        text-transform: uppercase;
        font-weight: 900;
        font-size: 20px;
        margin: 12px 0;
        padding: 8px;
        cursor: pointer;
        letter-spacing: 1px;
    }
    /* The font-weight, font-size, background-color, 
    and border can all be customized by the user. 
    The border-radius property allows you to give 
    an element rounded corners.*/
    input[type=text] {
        font-size: 22px;
        padding: 8px 0;
        font-weight: 900;
        text-align: center;
        background-color: #F0FFFF;
        border: 2px solid #ccc;
        border-radius: 6px;
    }
</style>
<script>
    function percentage_1() {
    // Method returns the element of percent id
    var percent = document.getElementById("percent").value;
    // Method returns the element of num id
    var num = document.getElementById("num").value;
    document.getElementById("value1")
        .value = (num / 100) * percent;
    }
    function percentage_2() {
    // Method returns the element of num1 id
    var num1 = document.getElementById("num1").value;
    // Method returns the elements of num2 id
    var num2 = document.getElementById("num2").value;
    document.getElementById("value2")
        	.value = (num1 * 100) / num2 + "%";
    }
</script>
</body>
</html>
