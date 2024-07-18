# calculator
# Ex.08 Design of a Standard Calculator

## AIM:
To design a standard calculator

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        #calculator-container {
            background-color:black;
            text-align: center;
            border: 1px solid greenyellow;
            padding: 20px;
            border-radius: 10px;
        }

        input {
            width: 85%;
            padding: 10px;
            margin: 5px 0;
        }

        button {
            width: 50px;
            height: 48px;
            font-size: 16px;
            margin: 5px;
        }
    </style>
</head>
<body>
    <div id="calculator-container">
        <h2><font color= "orange"></fontcolor>SYED ADIL BASHA</h2>
        <h3>212221043008</h3>
        <h2> STANDARD CALCULATOR</h2>

        <input type="text" id="display" disabled>

        <br>
 <button onclick="appendToDisplay('(')">(</button>
 <button onclick="appendToDisplay(')')">)</button>
 <button onclick="appendToDisplay('.')">.</button>
    <button onclick="apprndToDisplay('+')">+</button>
 
            
  <br>

       
        <button onclick="appendToDisplay('7')">7</button>
        <button onclick="appendToDisplay('8')">8</button>
        <button onclick="appendToDisplay('9')">9</button>
        <button onclick="appendToDisplay('-')">-</button>
 
        

        <br>

        <button onclick="appendToDisplay('4')">4</button>
        <button onclick="appendToDisplay('5')">5</button>
        <button onclick="appendToDisplay('6')">6</button>
        <button onclick="appendToDisplay('*')">*</button>
        

        <br>
 
        <button onclick="appendToDisplay('1')">1</button>
        <button onclick="appendToDisplay('2')">2</button>
        <button onclick="appendToDisplay('3')">3</button>
        <button onclick="appendToDisplay('/')">/</button>

        
 <br>
    <button onclick="calculate()">=</button>
    <button onclick="appendToDisplay('0')">0</button>
 
    <button onclick="clearDisplay()">C</button>
    <button onclick="appendToDisplay('%')">%</button>
    </div>

    <script>
        function clearDisplay() {
            document.getElementById('display').value = '';
        }

        function appendToDisplay(value) {
            document.getElementById('display').value += value;
        }

        function calculate() {
            try {
                document.getElementById('display').value = eval(document.getElementById('display').value);
            } catch (error) {
                document.getElementById('display').value = 'Error';
            }
        }
    </script>
</body>
</html>
```

## OUTPUT:
![Screenshot (181)](https://github.com/SYEDADILBASHA1/Calc/assets/134796157/417efcb8-c58f-4ac5-be83-0e188950b62c)

## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
