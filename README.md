grace-trader
index.html
style.css
script.js
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>GraceTrader</title>
<link rel="stylesheet" href="style.css">
</head>
<body>

<div class="card">
  <img src="logo.jpg" class="logo">

  <h1>Grace TRADER</h1>
  <p>Join our <b>Premium Forex Channel</b> & get</p>

  <ul>
    <li>✅ 100% Accurate Signals</li>
    <li>✅ Daily Profits Assured 💸</li>
    <li>✅ Professional Risk Management 📈</li>
  </ul>

  <div class="timer">
    Offer Ends In: <span id="time">00:00:10</span>
  </div>

  <a href="https://t.me/YOURCHANNEL" class="btn">JOIN WHATSAPP NOW</a>

  <small>Ads managed by AdzMind Agency</small>
</div>

<script src="script.js"></script>
</body>
</html>
body{
  background:#000;
  font-family:Arial;
  display:flex;
  justify-content:center;
  align-items:center;
  height:100vh;
  color:white;
}

.card{
  background:#0b0b0b;
  padding:25px;
  border-radius:20px;
  text-align:center;
  width:90%;
  max-width:360px;
  box-shadow:0 0 25px #00ffc3;
}

.logo{
  width:120px;
  border-radius:50%;
  border:4px solid #00ffc3;
}

h1{color:#00ffc3;}

ul{list-style:none;padding:0;}

.btn{
  display:block;
  background:linear-gradient(90deg,#00ffc3,#007bff);
  padding:14px;
  color:black;
  text-decoration:none;
  border-radius:10px;
  margin-top:15px;
  font-weight:bold;
}let time = 10;
setInterval(()=>{
  if(time > 0){
    time--;
    document.getElementById("time").innerText = "00:00:" + (time<10?"0":"") + time;
  }
},1000);