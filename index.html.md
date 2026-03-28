<!DOCTYPE html>  
<html lang="fr">  
<head>  
<meta charset="UTF-8">  
<title>Zone 212</title>  
  
<style>  
* {  
    margin: 0;  
    padding: 0;  
    box-sizing: border-box;  
}  
  
body {  
    background: black;  
    color: white;  
    font-family: Arial, sans-serif;  
    overflow: hidden;  
}  
  
/* BACKGROUND IMAGE */  
.bg {  
    position: fixed;  
    width: 100%;  
    height: 100%;  
    background: url('sabre.jpg') center/cover no-repeat;  
    opacity: 0.25;  
    z-index: -1;  
    animation: zoom 20s infinite alternate;  
}  
  
@keyframes zoom {  
    0% { transform: scale(1); }  
    100% { transform: scale(1.1); }  
}  
  
/* CONTAINER */  
.container {  
    display: flex;  
    flex-direction: column;  
    align-items: center;  
    justify-content: center;  
    height: 100vh;  
}  
  
/* LOGO */  
.logo {  
    width: 260px;  
    margin-bottom: 30px;  
    animation: fadeDown 1.5s ease;  
}  
  
/* TEXT */  
h1 {  
    font-size: 80px;  
    letter-spacing: 8px;  
    animation: glow 2s infinite alternate;  
}  
  
/* COMING SOON animation */  
@keyframes glow {  
    from {  
        text-shadow: 0 0 10px white, 0 0 20px white;  
    }  
    to {  
        text-shadow: 0 0 30px white, 0 0 60px white;  
    }  
}  
  
/* FADE ANIMATION */  
@keyframes fadeDown {  
    from {  
        opacity: 0;  
        transform: translateY(-50px);  
    }  
    to {  
        opacity: 1;  
        transform: translateY(0);  
    }  
}  
  
/* LINE */  
.line {  
    width: 200px;  
    height: 3px;  
    background: white;  
    margin-top: 20px;  
    animation: expand 2s ease;  
}  
  
@keyframes expand {  
    from { width: 0; }  
    to { width: 200px; }  
}  
  
</style>  
  
</head>  
  
<body>  
  
<div class="bg"></div>  
  
<div class="container">  
    <img src="logo.png" class="logo">  
    <h1>COMING SOON</h1>  
    <div class="line"></div>  
</div>  
  
</body>  
</html>  
