<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Mustasim 🎂</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    min-height:100vh;
    font-family:Arial,Helvetica,sans-serif;
    color:#fff;
    background:
        radial-gradient(circle at 15% 20%,#243b78 0%,transparent 35%),
        radial-gradient(circle at 85% 80%,#72285f 0%,transparent 35%),
        #070b17;
    overflow-x:hidden;
}

.page{
    display:none;
    min-height:100vh;
    padding:25px 15px;
    align-items:center;
    justify-content:center;
}

.page.active{
    display:flex;
    animation:pageIn .7s ease;
}

@keyframes pageIn{
    from{
        opacity:0;
        transform:translateY(30px) scale(.97);
    }
    to{
        opacity:1;
        transform:translateY(0) scale(1);
    }
}

.bg{
    position:fixed;
    inset:0;
    overflow:hidden;
    pointer-events:none;
    z-index:-1;
}

.glow{
    position:absolute;
    width:250px;
    height:250px;
    border-radius:50%;
    filter:blur(70px);
    opacity:.25;
    animation:glowMove 12s infinite alternate;
}

.g1{
    background:#477cff;
    top:-80px;
    left:-80px;
}

.g2{
    background:#ff4fa3;
    bottom:-100px;
    right:-80px;
    animation-delay:3s;
}

.g3{
    background:#ffd45c;
    top:40%;
    left:45%;
    width:140px;
    height:140px;
    animation-delay:6s;
}

@keyframes glowMove{
    from{transform:translate(0,0) scale(1)}
    to{transform:translate(80px,50px) scale(1.25)}
}

.card{
    width:100%;
    max-width:760px;
    padding:38px 25px;
    text-align:center;
    border-radius:30px;
    background:rgba(12,21,42,.82);
    border:1px solid rgba(255,255,255,.13);
    box-shadow:0 25px 80px rgba(0,0,0,.45);
    backdrop-filter:blur(15px);
}

.wishCard{
    text-align:left;
}

.badge{
    display:inline-block;
    padding:8px 15px;
    border-radius:50px;
    background:rgba(255,255,255,.07);
    border:1px solid rgba(255,255,255,.1);
    color:#b9c9ff;
    font-size:11px;
    letter-spacing:2px;
    margin-bottom:18px;
}

h1{
    font-size:clamp(40px,10vw,76px);
    margin-bottom:15px;
}

h2{
    color:#ffd866;
    font-size:clamp(25px,6vw,42px);
    margin-bottom:18px;
}

p{
    color:#e1e7f7;
    line-height:1.85;
    font-size:16px;
    margin:14px 0;
}

button{
    border:0;
    outline:0;
    cursor:pointer;
    margin:8px 4px;
    padding:15px 25px;
    border-radius:50px;
    color:white;
    font-weight:bold;
    font-size:14px;
    background:linear-gradient(135deg,#4c7cff,#7758ff);
    box-shadow:0 12px 30px rgba(74,117,255,.25);
    transition:.25s;
}

button:hover{
    transform:translateY(-3px);
}

button:active{
    transform:scale(.95);
}

.gold{
    background:linear-gradient(135deg,#ffd866,#ffab4d);
    color:#171d32;
}

.password{
    display:flex;
    justify-content:center;
    gap:10px;
    margin:27px 0;
}

.password input{
    width:60px;
    height:65px;
    border-radius:17px;
    border:1px solid #526ba5;
    background:rgba(0,0,0,.28);
    color:white;
    text-align:center;
    font-size:28px;
    outline:none;
}

.password input:focus{
    border-color:#ffd866;
    transform:translateY(-4px);
}

.count{
    font-size:130px;
    font-weight:900;
    color:#ffd866;
    animation:pulse 1s infinite;
}

@keyframes pulse{
    50%{transform:scale(1.12)}
}

.options{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:13px;
    margin-top:25px;
}

.options button{
    margin:0;
    background:rgba(54,77,132,.55);
    border:1px solid rgba(255,255,255,.1);
}

.progress{
    width:100%;
    height:7px;
    background:rgba(255,255,255,.08);
    border-radius:20px;
    margin-bottom:25px;
    overflow:hidden;
}

.progressBar{
    height:100%;
    border-radius:20px;
    background:linear-gradient(90deg,#557dff,#ffd866);
}

.mini{
    color:#aab7d8;
    font-size:13px;
}

.cakeArea{
    margin:25px auto;
}

.candle{
    font-size:65px;
    cursor:pointer;
    transition:.3s;
}

.candle:hover{
    transform:scale(1.15);
}

.cake{
    font-size:150px;
    cursor:pointer;
    transition:.5s;
}

.cake:hover{
    transform:scale(1.08);
}

.cake.cut{
    transform:rotate(-7deg) scale(.88);
}

.balloons{
    height:390px;
    width:100%;
    position:relative;
    margin-top:20px;
}

.balloon{
    position:absolute;
    width:68px;
    height:90px;
    border-radius:50%;
    cursor:pointer;
    animation:float 3s ease-in-out infinite alternate;
}

.balloon:after{
    content:"";
    position:absolute;
    left:50%;
    top:88px;
    width:2px;
    height:90px;
    background:rgba(255,255,255,.7);
}

.b1{left:4%;top:30px;background:#5e82ff}
.b2{left:24%;top:190px;background:#ff679d;animation-delay:.5s}
.b3{left:45%;top:45px;background:#ffd45c;animation-delay:1s}
.b4{left:65%;top:190px;background:#55ca8b;animation-delay:1.5s}
.b5{left:83%;top:55px;background:#a86eff;animation-delay:2s}

@keyframes float{
    from{transform:translateY(0) rotate(-4deg)}
    to{transform:translateY(-25px) rotate(4deg)}
}

.balloon.pop{
    animation:pop .4s forwards;
}

@keyframes pop{
    to{
        transform:scale(1.8);
        opacity:0;
    }
}

.finalName{
    font-size:clamp(55px,15vw,120px);
    font-weight:900;
    background:linear-gradient(135deg,#fff,#ffd866,#ff8cae);
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
}

.modal{
    position:fixed;
    inset:0;
    z-index:1000;
    display:none;
    align-items:center;
    justify-content:center;
    padding:20px;
    background:rgba(0,0,0,.7);
}

.modal.show{
    display:flex;
}

.modalBox{
    width:100%;
    max-width:420px;
    padding:32px 23px;
    border-radius:28px;
    text-align:center;
    background:#132445;
    border:1px solid rgba(255,255,255,.13);
    box-shadow:0 25px 80px rgba(0,0,0,.6);
    animation:modalIn .45s ease;
}

@keyframes modalIn{
    from{
        opacity:0;
        transform:scale(.7) translateY(30px);
    }
    to{
        opacity:1;
        transform:scale(1) translateY(0);
    }
}

.modalIcon{
    font-size:65px;
}

.modalTitle{
    font-size:28px;
    font-weight:bold;
    margin:10px 0;
}

.confetti{
    position:fixed;
    top:-25px;
    width:9px;
    height:15px;
    z-index:3000;
    animation:fall linear forwards;
}

@keyframes fall{
    to{
        transform:translateY(110vh) rotate(720deg);
        opacity:0;
    }
}

@media(max-width:560px){

    .card{
        padding:30px 18px;
    }

    .options{
        grid-template-columns:1fr;
    }

    .password input{
        width:55px;
        height:60px;
    }

    .balloon{
        width:55px;
        height:76px;
    }

    .balloon:after{
        top:74px;
    }
}
</style>
</head>

<body>

<div class="bg">
    <div class="glow g1"></div>
    <div class="glow g2"></div>
    <div class="glow g3"></div>
</div>


<!-- POPUP -->

<div class="modal" id="modal">
    <div class="modalBox">
        <div class="modalIcon" id="modalIcon">🎉</div>
        <div class="modalTitle" id="modalTitle">Amazing!</div>
        <p id="modalText"></p>
        <button onclick="closeModal()">CONTINUE →</button>
    </div>
</div>


<!-- 1 PASSWORD -->

<section class="page active" id="page1">

<div class="card">

<div class="badge">🔐 PRIVATE BIRTHDAY EXPERIENCE</div>

<h1>Hey Mustasim 👀</h1>

<h2>A Surprise Is Waiting 🎁</h2>

<p>
Someone prepared a little birthday journey for you... ✨<br>
But first, you need the secret code 🔐
</p>

<div class="password">

<input id="p1" maxlength="1" inputmode="numeric">
<input id="p2" maxlength="1" inputmode="numeric">
<input id="p3" maxlength="1" inputmode="numeric">
<input id="p4" maxlength="1" inputmode="numeric">

</div>

<button onclick="unlock()">
UNLOCK 🔓
</button>

<p class="mini">Hint: the secret code has 4 numbers 👀</p>

</div>

</section>


<!-- 2 COUNTDOWN -->

<section class="page" id="page2">

<div class="card">

<div class="badge">ACCESS GRANTED 🔓</div>

<h2>Get Ready Mustasim! 🎉</h2>

<div class="count" id="count">3</div>

<p>
Your birthday experience is loading... ✨🎂
</p>

</div>

</section>


<!-- 3 INTRO -->

<section class="page" id="page3">

<div class="card">

<div class="badge">WELCOME ✨</div>

<h1>Happy Birthday 🎂</h1>

<h2>Mustasim! 🥳</h2>

<p>
Welcome to your little birthday adventure 💙✨
</p>

<p>
There are some tasks 🎯, wishes 💌,
a cake 🎂, balloons 🎈 and one BIG final surprise 🌟
waiting for you.
</p>

<button class="gold" onclick="showPage(4)">
START THE JOURNEY 🚀
</button>

</div>

</section>


<!-- 4 TASK 1 -->

<section class="page" id="page4">

<div class="card">

<div class="progress">
<div class="progressBar" style="width:20%"></div>
</div>

<div class="badge">TASK 01 🎯</div>

<h2>Easy One 😎</h2>

<p>
What are we celebrating today? 👀🎉
</p>

<div class="options">

<button onclick="wrong()">Monday 📚</button>

<button onclick="taskCorrect(5)">
Birthday 🎂
</button>

<button onclick="wrong()">Homework 📝</button>

<button onclick="wrong()">Nothing 😂</button>

</div>

</div>

</section>


<!-- 5 WISH 1 -->

<section class="page" id="page5">

<div class="card wishCard">

<div class="badge">WISH 01 💌✨</div>

<h2>Happy Birthday Mustasim! 🎂🥳</h2>

<p>
🎉✨ Today is your special day, Mustasim!
I hope your day is filled with smiles 😊,
good vibes 💙 and beautiful memories 📸.
</p>

<p>
🌟 May every new step bring something exciting,
every challenge teach you something valuable 📚,
and every achievement give you another reason to smile 🏆.
</p>

<p>
🎈 Keep enjoying the little moments,
keep learning new things 🚀 and keep moving forward.
</p>

<button onclick="showPage(6)">
NEXT TASK 🎯
</button>

</div>

</section>


<!-- 6 TASK 2 -->

<section class="page" id="page6">

<div class="card">

<div class="progress">
<div class="progressBar" style="width:40%"></div>
</div>

<div class="badge">TASK 02 🧠</div>

<h2>Remember The Code 🔐</h2>

<p>
What was the secret password that opened this website? 👀
</p>

<input
id="answer"
maxlength="4"
inputmode="numeric"
placeholder="Enter 4 digits"
style="
width:190px;
padding:16px;
border-radius:15px;
border:1px solid #526ba5;
background:rgba(0,0,0,.3);
color:white;
font-size:21px;
text-align:center;
outline:none;
">

<br>

<button onclick="checkAnswer()">
CHECK 🔍
</button>

</div>

</section>


<!-- 7 WISH 2 -->

<section class="page" id="page7">

<div class="card wishCard">

<div class="badge">WISH 02 🌟</div>

<h2>A New Chapter Begins 🚀</h2>

<p>
Mustasim 💙, may the coming days bring you
new experiences 🌍, new ideas 💡 and lots of reasons
to be proud of yourself 🏆.
</p>

<p>
✨ May you keep discovering what you enjoy,
keep improving your skills 📚 and make memories
that you will look back on with a smile 😊.
</p>

<p>
🌈 Keep your goals clear, your mindset positive
and your journey your own.
</p>

<button onclick="showPage(8)">
NEXT 🎁
</button>

</div>

</section>


<!-- 8 TASK 3 -->

<section class="page" id="page8">

<div class="card">

<div class="progress">
<div class="progressBar" style="width:60%"></div>
</div>

<div class="badge">TASK 03 🎁</div>

<h2>Choose Your Gift 👀</h2>

<p>
One of these boxes contains the next surprise 🎁
</p>

<div class="options">

<button onclick="giftWrong()">🎁 BOX 1</button>
<button onclick="giftWrong()">🎁 BOX 2</button>
<button onclick="giftCorrect()">🎁 BOX 3</button>
<button onclick="giftWrong()">🎁 BOX 4</button>

</div>

</div>

</section>


<!-- 9 WISH 3 -->

<section class="page" id="page9">

<div class="card wishCard">

<div class="badge">WISH 03 💙✨</div>

<h2>Keep Being You 😎</h2>

<p>
🌟 There is something special about being yourself.
Keep your own personality, your own ideas
and your own way of enjoying life.
</p>

<p>
💪 Small progress is still progress.
One step at a time can take you surprisingly far 🚀.
</p>

<p>
😊 So today, enjoy your day, laugh a little louder,
make some memories and have a genuinely amazing birthday! 🎉
</p>

<button class="gold" onclick="showPage(10)">
FINAL TASK 🏆
</button>

</div>

</section>


<!-- 10 FINAL TASK -->

<section class="page" id="page10">

<div class="card">

<div class="progress">
<div class="progressBar" style="width:80%"></div>
</div>

<div class="badge">FINAL TASK 🏆</div>

<h2>One Last Question 👀</h2>

<p>
What should Mustasim do on his birthday? 🎂
</p>

<div class="options">

<button onclick="wrong()">Study all day 📚</button>

<button onclick="taskCorrect(11)">
Enjoy The Day 🎉
</button>

<button onclick="wrong()">Do Homework 📝</button>

<button onclick="wrong()">Sleep 😂</button>

</div>

</div>

</section>


<!-- 11 CAKE INTRO -->

<section class="page" id="page11">

<div class="card">

<div class="badge">ALL TASKS COMPLETE 🏆</div>

<h1>You Did It! 🎉</h1>

<h2>Now... Cake Time! 🎂</h2>

<p>
The tasks are complete ✨
but the real birthday moment is just beginning...
</p>

<button class="gold" onclick="showPage(12)">
LET'S CUT THE CAKE 🎂
</button>

</div>

</section>


<!-- 12 CAKE -->

<section class="page" id="page12">

<div class="card">

<div class="badge">BIRTHDAY CAKE 🎂</div>

<h2>Make A Wish, Mustasim! ✨</h2>

<p>
First tap the candle 🕯️<br>
Then tap the cake 🎂
</p>

<div class="cakeArea">

<div class="candle" id="candle" onclick="blowCandle()">
🕯️
</div>

<div class="cake" id="cake" onclick="cutCake()">
🎂
</div>

</div>

<p id="cakeMessage">
Your wish is waiting... 🌟
</p>

<button
id="cakeNext"
style="display:none"
onclick="showPage(13)">
NEXT SURPRISE 🎈
</button>

</div>

</section>


<!-- 13 BALLOONS -->

<section class="page" id="page13">

<div class="card">

<div class="badge">BALLOON SURPRISE 🎈</div>

<h2>Pop Them All! 🎈</h2>

<p id="balloonText">
Every balloon hides a little birthday message 💌
</p>

<div class="balloons">

<div class="balloon b1"
onclick="popBalloon(this,'🌟 May your dreams keep getting bigger and brighter!')">
</div>

<div class="balloon b2"
onclick="popBalloon(this,'😊 May you always have plenty of reasons to smile!')">
</div>

<div class="balloon b3"
onclick="popBalloon(this,'🚀 May exciting opportunities find you everywhere!')">
</div>

<div class="balloon b4"
onclick="popBalloon(this,'💙 May your best memories always be ahead!')">
</div>

<div class="balloon b5"
onclick="popBalloon(this,'🎂 And finally... HAPPY BIRTHDAY MUSTASIM! 🥳')">
</div>

</div>

<button
id="balloonNext"
class="gold"
style="display:none"
onclick="showPage(14)">
FINAL SURPRISE 🌟
</button>

</div>

</section>


<!-- 14 BIG WISH -->

<section class="page" id="page14">

<div class="card wishCard">

<div class="badge">THE BIG FINAL WISH 💌🌟</div>

<h2>Dear Mustasim 💙</h2>

<p>
🎂🥳 Happy Birthday once again!
I hope this little journey made your day
a little more fun and memorable ✨.
</p>

<p>
🌟 May your future be filled with amazing opportunities,
good memories 📸, exciting experiences 🚀
and plenty of moments that make you genuinely happy 😊.
</p>

<p>
💪 Keep learning, keep growing, keep trying new things
and always give yourself a chance to discover
what you are capable of.
</p>

<p>
🎈 May every year bring new adventures,
new achievements 🏆 and countless reasons to celebrate.
</p>

<p>
💙 Most importantly, enjoy the people and moments
that make life special. Those memories are priceless. ✨
</p>

<h2 style="text-align:center">
HAPPY BIRTHDAY MUSTASIM! 🎂🥳🎉
</h2>

<button class="gold" onclick="showPage(15)">
ONE LAST SURPRISE 🎁
</button>

</div>

</section>


<!-- 15 FINAL -->

<section class="page" id="page15">

<div class="card">

<div class="badge">FINAL PAGE ✨</div>

<div class="finalName">
MUSTASIM
</div>

<h2>Happy Birthday! 🎂</h2>

<p>
🎉 The birthday journey is complete! 🎉
</p>

<p>
🎂 🎈 🥳 ✨ 💙 🌟 🎁
</p>

<p>
Thank you for completing every little surprise.
Now go enjoy your special day! 😎🔥
</p>

<button class="gold" onclick="replay()">
REPLAY ↻
</button>

</div>

</section>


<script>

/* ================= PAGE SYSTEM ================= */

function showPage(number){

    document.querySelectorAll(".page").forEach(function(page){
        page.classList.remove("active");
    });

    document.getElementById("page"+number).classList.add("active");

    window.scrollTo({
        top:0,
        behavior:"smooth"
    });

    if(number===2){
        startCountdown();
    }
}


/* ================= POPUP ================= */

let nextPage=null;

function popup(icon,title,text,page=null){

    document.getElementById("modalIcon").innerHTML=icon;
    document.getElementById("modalTitle").innerHTML=title;
    document.getElementById("modalText").innerHTML=text;

    nextPage=page;

    document.getElementById("modal").classList.add("show");
}

function closeModal(){

    document.getElementById("modal").classList.remove("show");

    if(nextPage!==null){

        let target=nextPage;
        nextPage=null;

        setTimeout(function(){
            showPage(target);
        },200);
    }
}


/* ================= PASSWORD ================= */

const passwordInputs=[
    document.getElementById("p1"),
    document.getElementById("p2"),
    document.getElementById("p3"),
    document.getElementById("p4")
];

passwordInputs.forEach(function(input,index){

    input.addEventListener("input",function(){

        input.value=input.value.replace(/[^0-9]/g,"");

        if(input.value && index<3){
            passwordInputs[index+1].focus();
        }
    });

    input.addEventListener("keydown",function(e){

        if(e.key==="Backspace" && !input.value && index>0){
            passwordInputs[index-1].focus();
        }

        if(e.key==="Enter"){
            unlock();
        }
    });

});


function unlock(){

    const code=
        document.getElementById("p1").value+
        document.getElementById("p2").value+
        document.getElementById("p3").value+
        document.getElementById("p4").value;

    if(code==="0019"){

        confetti();

        popup(
            "🔓",
            "ACCESS GRANTED!",
            "Welcome to Mustasim's special birthday experience! 🎉✨",
            2
        );

    }else{

        popup(
            "🔒",
            "WRONG CODE!",
            "Try the secret code again 👀<br><br>Hint: <b>0019</b>",
            null
        );
    }
}


/* ================= COUNTDOWN ================= */

let countdownTimer;

function startCountdown(){

    clearInterval(countdownTimer);

    let number=3;

    document.getElementById("count").innerHTML=number;

    countdownTimer=setInterval(function(){

        number--;

        if(number>0){
            document.getElementById("count").innerHTML=number;
        }

        if(number===0){

            clearInterval(countdownTimer);

            document.getElementById("count").innerHTML="🎉";

            setTimeout(function(){
                showPage(3);
            },800);
        }

    },1000);
}


/* ================= TASKS ================= */

function taskCorrect(page){

    confetti();

    popup(
        "🎉",
        "CORRECT!",
        "Nice one! Another birthday surprise has been unlocked ✨",
        page
    );
}

function wrong(){

    popup(
        "😅",
        "NOT QUITE!",
        "No worries! Try another answer 👀✨",
        null
    );
}


/* ================= CODE TASK ================= */

function checkAnswer(){

    const value=document.getElementById("answer").value.trim();

    if(value==="0019"){

        confetti();

        popup(
            "🧠",
            "PERFECT!",
            "You remembered the secret code! 🔐🔥",
            7
        );

    }else{

        popup(
            "🤔",
            "TRY AGAIN!",
            "Think back to the very first screen 👀",
            null
        );
    }
}


/* ================= GIFT ================= */

function giftCorrect(){

    confetti();

    popup(
        "🎁",
        "YOU FOUND IT!",
        "The correct gift box contained the next surprise! 🎉",
        9
    );
}

function giftWrong(){

    popup(
        "📦",
        "EMPTY BOX!",
        "Oops 😂 Try