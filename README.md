# Week-3-Notes
Week 3 Notes 
05/23/22 Notes
Loops
Loops means do it again and again… The idea in a loop is being able to do it multiple of times, but not having it to write the code multiple of times. 
Make sure to include a JavaScript file in the assignments. 
The Loops have to have a start and end point. They have to have something that makes them go from the start point to the end point if not they will go forever.
•	Do Loop – Always happens one time whether if it’s true or not. The check whether is true is at the bottom of the loop. 
Do
Alert (“asdf”)
Dfsdkfjsdfsdf
Dfksdfjsdkfsd
Sdfsdjkfsjdkfsd
3 while (exit !=4) 
A do loop can always be replaced by a while loop, however be careful if you only want to run it one time you would want to a do loop. 

•	While Loop – check at beginning and won’t always runs one time. 
•	For Loop -  Can be replace with a while or a do loop. A for when you know the number of times. ( Initial condition; keep going until whatever number; incremental changes
Va i = 1;
For (i =1; <<7;i++)
If you have no curly brackets it will only work for one statement.
Add { 
} for every statement. 






<!DOCTYPE html>
<!--Sanyerlis Camacaro 052322 Class Notes-->

<html>

<head>
    <!--links my javascript file to the html file-->
    <script src="codeloop.js"></script>
<!--links my css to my html-->
<link href="styleloop.css" rel="stylesheet" type="text/css" />
<!--this is where the title for the website goes-->
<title>
    UAT Space Page
</title>
</head>
</html>

<body>

    <br>

    <br>
    <br>
    <br>
<h2>CountDown Timer</h2>
<p id="countdownTimer"> The Countdown stars here...</p>
<br>
<button onclick="simplecount"() ;" class="LoopButtons">Start Simple</button>
<button onclick="simpleDo"() ; " class="LoopButtons">Simple Do</button>
<button button onclick="betterCountdown();" class="LoopButtons">Start</button> 
<button onclick="whileCount();" class="LoopButtons">Start While</button>
<button> Boring </button>
<br>
<br>

<br>

</body>

</html>
body {
    background-color: blueviolet;
    background-image: linear-gradient(90deg, rgb(255, 255, 255),#d42e36);
}

.LoopButtons {
    width: 100px;
    height: 30px;
    background-color: aliceblue;
    border-radius:200px ;
    border-color: blueviolet;
}

function simpleCount() {
    var currTime = 10;
    /*  for (initial condition, ending condition - stop when not true, what to 
after each loop) i++ same as  i = i+1*/
    for (var i = 1; i < 12; i++) {
        setTimeout(function () {
            document.getElementById("countdownTimer").innerHTML = "the time left is
" + currTime;
            currTime = currTime - 1;
        }, 1000 * i);
    }
}
function simpleDo() {
    var currTime = 10;
    var i = 1;
    do {
        setTimeout(function () {
            document.getElementById("countdownTimer").innerHTML = "the time left is
" + currTime;
            currTime = currTime - 1;
        }, 1000 * i);
        i += 1;
    } while (i < 12);
}
function betterCountdown() {
    var currTime = 10;
    for (var i = 1; i <= 11; i++) {
        if (i == 11) {
            setTimeout(function () {
                //code goes here for timer
                document.getElementById("countdownTimer").innerHTML = 
"Blastoff!!!";
            }, 1000 * i);
        } else if (i > 6) {
            setTimeout(function () {
                document.getElementById("countdownTimer").innerHTML =
                    "Warning Less than half way to launch, time left = " + 
currTime;
                currTime = currTime - 1;
            }, 1000 * i);
        } else {
            setTimeout(function () {
                document.getElementById("countdownTimer").innerHTML = "the time 
left is " + currTime;
                currTime = currTime - 1;
            }, 1000 * i);
        }
    }
}
function whileCount() {
    var currTime = 10;
    var i = 1;
    while (i < 12) {
        if (i == 11) {
            setTimeout(function () {
                //code goes here for timer
                document.getElementById("countdownTimer").innerHTML = 
"Blastoff!!!";
            }, 1000 * i);
        } else if (i > 6) {
            setTimeout(function () {
                document.getElementById("countdownTimer").innerHTML =
                    "Warning Less than half way to launch, time left = " + 
currTime;
                currTime = currTime - 1;
            }, 1000 * i);
        } else {
            setTimeout(function () {
                document.getElementById("countdownTimer").innerHTML = "the time 
left is " + currTime;
                currTime = currTime - 1;
            }, 1000 * i);
        }
        i = i + 1;
    }
}
You never break out of a loop. 
Loops are needed no matter what language or network you are using. 
05/25/22 Notes
Conditionals - Decision 

3 Types of conditionals 

If statement 

If ( condition )

{

// statements 

}

Else if (condition)

{

//

}

Else 

There’s no need to have a condition in an else statement. 

Else means if you didn’t hit it in any of the above it’s going to print into the else and print that’s not a valid response. 

Every if statement should have a final else statement, everything should be taken care of. 

Switch statement (Case)

Switch (Var)

Case Val1
//Success
//Statements
Third Condition – Loops
If (sum ==7 double line sum ==11)
Double = means don’t set it to 7 but check to see if it’s 7. Double line means or means if it’s 11 you lose. 
Function to set up two players and then assign a random number 1 to 3.
Rock =1, paper =2, scissors =3 in javascript  
If (playerNum ==1) {
   Console.log(“Rock”);
   Return “Rock”;
}
Else if (playerNum ==2) {
   Console.log(“paper”);
    Return “paper”;
}
Else if (playerNum ==3) {
 Console.log(“scissors”);
 Return “scissors”
} else {
 Console.log(“Error”);
}
}
