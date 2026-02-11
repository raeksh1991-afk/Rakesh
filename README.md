<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Promise Day - For Vandana</title>

<style>
body{
    margin:0;
    font-family: Arial, sans-serif;
    background: linear-gradient(135deg,#ff758c,#ff7eb3);
    color:white;
    text-align:center;
}

.container{
    padding:50px 20px;
}

h1{
    font-size:3em;
}

.heart{
    font-size:60px;
    animation: beat 1s infinite;
}

@keyframes beat{
    0%{transform:scale(1);}
    50%{transform:scale(1.2);}
    100%{transform:scale(1);}
}

.promise-box{
    background:white;
    color:#ff4f81;
    padding:25px;
    margin:30px auto;
    max-width:500px;
    border-radius:15px;
    box-shadow:0 5px 15px rgba(0,0,0,0.2);
    font-size:18px;
    line-height:1.6;
}

button{
    background:#fff;
    color:#ff4f81;
    border:none;
    padding:12px 25px;
    font-size:16px;
    border-radius:25px;
    cursor:pointer;
}

button:hover{
    background:#ffe6ee;
}

footer{
    margin-top:40px;
}
</style>
</head>

<body>

<div class="container">
    <div class="heart">❤️</div>
    <h1>Happy Promise Day Vandana</h1>

    <div class="promise-box" id="promise">
        Vandana,  
        I promise to stand by you,  
        to respect you,  
        and to love you more every day.  
        — Rakesh
    </div>

    <button onclick="newPromise()">Click for My Promises</button>

    <footer>
        Forever yours, Vandana ❤️  
        — Rakesh
    </footer>
</div>

<script>
const promises = [
"Vandana, I promise to never leave your side. — Rakesh",
"I promise to make you smile every day. — Rakesh",
"I promise to support your dreams. — Rakesh",
"I promise to be honest and loyal. — Rakesh",
"I promise to love you forever. — Rakesh"
];

function newPromise(){
    const random = promises[Math.floor(Math.random()*promises.length)];
    document.getElementById("promise").innerText = random;
}
</script>

</body>
</html>
