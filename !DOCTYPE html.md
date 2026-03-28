<!DOCTYPE html>  
<html lang="fr">  
<head>  
<meta charset="UTF-8">  
<meta name="viewport" content="width=device-width, initial-scale=1.0">  
<title>Zone 212</title>  
  
<style>  
* {  
    margin: 0;  
    padding: 0;  
    box-sizing: border-box;  
}  
  
body {  
    height: 100vh;  
    background: url('fond.jpg') center/cover no-repeat;  
    display: flex;  
    justify-content: center;  
    align-items: center;  
    font-family: Arial, sans-serif;  
    color: white;  
    overflow: hidden;  
}  
  
/* fond sombre */  
body::before {  
    content: "";  
    position: absolute;  
    width: 100%;  
    height: 100%;  
    background: rgba(0,0,0,0.7);  
}  
  
/* contenu */  
.container {  
    position: relative;  
    text-align: center;  
    animation: fadeIn 2s ease;  
}  
  
.logo {  
    width: 220px;  
    margin-bottom: 30px;  
    animation: zoom 1.5s ease;  
}  
  
h1 {  
    font-size: 70px;  
    letter-spacing: 6px;  
    animation: glitch 1s infinite;  
}  
  
/* animations */  
@keyframes fadeIn {  
    from {opacity: 0;}  
    to {opacity: 1;}  
}  
  
@keyframes zoom {  
    from {transform: scale(0);}  
    to {transform: scale(1);}  
}  
  
@keyframes glitch {  
    0% {text-shadow: 3px 3px red;}  
    50% {text-shadow: -3px -3px blue;}  
    100% {text-shadow: 3px 3px red;}  
}  
</style>  
</head>  
  
<body>  
  
<div class="container">  
    <img src="logo.png" class="logo">  
    <h1>COMING SOON</h1>  
</div>  
  
</body>  
</html>  
