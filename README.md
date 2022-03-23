# M1C2
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>flexbox assignment</title>
    <link rel="stylesheet" href="./flex.css" />
</head>

<style>

body {
      margin: 0;
      padding: 0;
    } 
    
    .flexOne{
        margin: 0;
        display: flex;
    }
    
    .flexOne .square{
        margin: 5px;
        background-color: aqua;
        height: 150px;
        width: 150px;
    }

    .flexTwo {
        margin: 0;
        display: flex;
        flex-direction: column;
    }

    .flexTwo .square {
        margin: 5px;
        background-color: green;
        height: 150px;
        width: 150px;
    }

    .flexThree {
        margin: 0;
        display: flex;
        flex-direction: row-reverse;
    }

    .flexThree .square {
        margin: 5px;
        background-color: red;
        height: 150px;
        width: 150px;
    }
    
    .flexFour {
        margin: 0;
        display: flex;
        flex-wrap: wrap;
    }

    .flexFour .square {
        margin: 5px;
        background-color: #3d8b6d;
        height: 150px;
        width: 350px;
    }

    .flexFive {
        margin: 0;
        width: 350px;
        display: flex;
    }

    .flexFive .item {
        background-color: #0b6643;
        height: 100px;
        margin: 2px;
        width: 100px;
    }

    #grow  {
        flex-grow: 2;
    }

    .flexSix {
        margin: 5px;
        height:400px;
        width: 500px;
        background-color: #f1f1f1;
        display: flex;
        flex-direction: column;
    }
    
    .flexSix > .one > .square {
        width: 100px;
        height:100px;
        background-color: red;
        margin-bottom: 5px;
    }  

    .flexSix > .two > .square {
        width: 100px;
        height:100px;
        background-color: red;
        margin-bottom: 5px;
    }

    .flexSix > .three > .square {
        width: 100px;
        height:100px;
        background-color: red;
    }
    
    .flexSix > .one  {
    background-color: aqua;
    display: flex;
    justify-content: space-around;
    }

    .flexSix > .two {
    background-color: #d6d6d6;
    display: flex;
    justify-content: space-between;
    }

    .flexSix > .three {
        background-color: aqua;
        display: flex;
        justify-content: space-evenly;
    }

    .flexSeven {
        margin: 10px;
        background-color: lightgrey;
        height: 400px;
        width: 500px;
        display:flex;
        justify-content: space-between;
    }

    .flexSeven > .one {
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    .flexSeven > .one > .square {
        width: 100px;
        height:100px;
        background-color: red;
    }

    .flexSeven > .two {
        display: flex;
        flex-direction: column;
        justify-content: flex-end;
    }

    .flexSeven > .two > .square {
        width: 100px;
        height:100px;
        background-color: red;
    }

    .flexSeven > .three {
        display: flex;
        flex-direction: column;
        justify-content: flex-start;
    }

    .flexSeven > .three > .square {
        width: 100px;
        height:100px;
        background-color: red;
    }

    .fleSeven > .four {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }

    .flexSeven > .four > .square {
        width: 100px;
        height:100px;
        background-color: red;
        margin: 20px;
    }


    .flexEight {
        margin: 5px;
        background-color: #eeeeee;
        height: 300px;
        width: 400px;
        display:flex;
        justify-content: space-between;
    }

    .flexEight > .one {
        display: flex;
        align-items: center;
    }

    .flexEight > .one > .square {
        width: 100px;
        height:100px;
        background-color: red;
    }

    .flexEight > .two {
        display: flex;
        justify-content: flex-end;
    }

    .flexEight > .two > .square {
        width: 100px;
        height:100px;
        background-color: red;
    }

    .flexEight > .three {
        display: flex;
        justify-content: flex-start;
    }   

    .flexEight > .three > .square {
        width: 100px;
        height:100px;
        background-color: red;
    }
    
    .flexNine {
        width: 450px;
        height: 250px;
        background-color: #eeeeee;
        display: flex;
        align-items: flex-start;
        justify-content: space-evenly;
    }

    
    .flexNine > .square {
        background-color: red;
        height: 100px;
        width: 100px;
    }
    
    #special {
        align-self: flex-end;
    }

</style>

<body>
    <div class="flexOne">
        <div class="square"></div>
        <div class="square"></div>
        <div class="square"></div>
    </div>

    <div class="flexTwo">
        <div class="square"></div>
        <div class="square"></div>
        <div class="square"></div>
    </div>

    <div class="flexThree">
        <div class="square">1</div>
        <div class="square">2</div>
        <div class="square">3</div>
    </div>

    <div class="flexFour">
        <div class="square"></div>
        <div class="square"></div>
        <div class="square"></div>
        <div class="square"></div>
    </div>

    <div class="flexFive">
        <div class="item"></div>
        <div class="item" id="grow"></div>
        <div class="item"></div>
    </div>

    <div class="flexSix">
        <div class="one">
            <div class="square"></div>
            <div class="square"></div>
            <div class="square"></div>
        </div>
        <div class="two">
            <div class="square"></div>
            <div class="square"></div>
            <div class="square"></div>
        </div>
        <div class="three">
            <div class="square"></div>
            <div class="square"></div>
            <div class="square"></div>
        </div>
    </div>

    <div class="flexSeven">
        <div class="one">
            <div class="square"></div>
            <div class="square"></div>
            <div class="square"></div>
        </div>
        <div class="two">
            <div class="square"></div>
            <div class="square"></div>
            <div class="square"></div>
        </div>
        <div class="three">
            <div class="square"></div>
            <div class="square"></div>
            <div class="square"></div>
        </div>
        <div class="four">
            <div class="square"></div>
            <div class="square"></div>
            <div class="square"></div>
        </div>
    </div>

    <div class="flexEight">
        <div class="one">
            <div class="square"></div>
        </div>
        <div class="two">
            <div class="square"></div>
        </div>
        <div class="three">
            <div class="square"></div>
        </div>
    </div>

    <div class="flexNine">
        <div class="square"></div>
        <div class="square"></div>
        <div class="square" id="special"></div>
        <div class="square"></div>
    </div>

</body>
</html>
