# Cars-CSS-HTML
Landing page Frontend
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cars</title>
    <link rel="stylesheet" type="text" href="cars/style.css">
<style>
   *{
       margin: 0;
       padding: 0;
       font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
   }
   header{
       background-image:linear-gradient(rgba(0,0,0,0.5),rgba(0,0,0,0.5)), url(wal.jpg);
       height: 100vh;
       background-size: cover;
       background-position: center;
       
   }
   ul{
       float:right;
   }
  

   ul li{
       list-style: none;
       display: inline-block;
       margin-top: 30px;
   }

ul li a{
    text-decoration: none;
    color: white;
    padding: 5px 20px;
    border-radius: 100px;
    transition: 0.6s ease;
    /* background: linear-gradient(90deg,#03a9f4, #f441a5,#ffeb3b,#03a9f4);
    background-size: 400%; */
    
}   
ul li a:hover{
    animation: animate 8s linear infinite;
    color: black;
    background: linear-gradient(90deg,#03a9f4, #f441a5,#ffeb3b,#03a9f4);
    background-size: 400%;
    z-index: 1;
    
}
.main .logo{
    animation: animate 8s linear infinite;
    color: black;
    background: linear-gradient(90deg,#03a9f4, #f441a5,#ffeb3b,#03a9f4);
    background-size: 400%;
    z-index: 1;
}
@keyframes animate
{
    0%
    {
        background-position: 0%;
    }
    100%
    {
        background-position: 400%;
    }
}
 a:before{
    content: '';
    position: absolute;
    top: -5px;
    bottom: -5px;
    left: -5px;
    right: -5px;
    z-index: -1;
    background: linear-gradient(90deg,#03a9f4, #f441a5,#ffeb3b,#03a9f4);
    background-size: 400%;
    filter: blur(20px);
    opacity: 0;
    transition: 0.5s;
}
 a:hover:before{
    filter: blur(20px);
    opacity: 1;
    animation: animate 8s linear infinite;

}
.logo img{
    float: left;
    width: 150px;
    margin-top: 15px;
    
}
.main{
    max-width: 1200px;
    margin: auto;
}
.title{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
}
.title h1{
    font-size: 200px;
    color:white;
}
.button{
    position: absolute;
    top: 70%;
    left: 50%;
    transform: translate(-50%,-50%);

}
.btn{
    border: 1px solid white;
    padding: 10px 30px;
    color: white;
    text-decoration: none;
    transition: 0.6s ease;
}
.btn:hover{
    color: yellowgreen;
    background-color: rgb(22, 1, 1);
    
}
.aud {
    position: absolute;
    top: 88%;
    left: 50%;
    transform: translate(-50%,-50%);

}
    
#bar1{
    transform: translateY(-4px);
}
#bar3{
    transform: translateY(4px);
}
.change .bar{
    background-color: white;
}
.change #bar1{
    transform: translateY(4px) rotateZ(-45deg);
}
.change #bar3{
    transform: translateY(-6px) rotate(45deg);
}
.change #bar2{
    opacity: 0;
}
</style>
</head>
<body>
    <header>
        <div class="main">
            <div class="logo">
                <img src="lo.jpeg">
            </div>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Services</a></li>
                <li><a href="#">Gallery </a></li>
                <li><a href="#">about</a></li>
                <li><a href="#">Contact us</a></li>
            </ul>

        </div>
        <div class="title"><h1>Cars</h1>
        </div>
        <div class="button"> 
<a href="#" class = "btn" >watch Cars</a>
<a href="#" class = "btn" >Buy Now </a>
        </div>
     <div  class="aud">  
          <audio controls>
            <source src="XXXTENTACION - Look At Me! (Audio)-320.mp3" type="audio/mpeg">
            </div>
            </audio>
            <div id="menu-bar">
            <div id="menu" onclick="onclickmenu()">
            <div id="bar1" class="bar"></div>
            <div id="bar2" class="bar"></div>
            <div id="bar3" class="bar"></div>
        </div>
    </div>
    <script>
        function onclickmenu(){
            document.getElementById("menu").classList.toggle("change");
        }
    </script>
    </header>
</body>
</html>
