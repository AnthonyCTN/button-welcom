# button-welcom
buton welcom pour ma page d'accueil en css 


  <a href="dubut_pages_affichable.php"><span>Welcome</span></a>



    
    </script>
    
    
    </body>
    </html>
    
    
    <style>
    *{
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body{
        background-color: rgb(5, 5, 5);
      display: flex;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
    }
    
    
    a{
      position: relative;
      background: rgb(22, 21, 21);
      color: white;
      width: 80px;
      height: 80px;
       display: flex;
      align-items: center;
      justify-content: center;
      transition: 0.5s;
      box-shadow: 0 20px 25px blue;
      overflow: hidden;
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      font-size: 1.2em;
    }
    
    
    a::before{
      content:"";
      position: absolute;
      left: 30px;
      width: 15px;
      height: 15px;
      border-top: 4px solid white;
      border-right: 4px solid white;
      transform: rotate(45deg);
      transition: 0.5s;
    }
    
    
    a::after{
      content:"";
      position: absolute;
      width: 15px;
      height: 15px;
      border-top: 4px solid white;
      border-right: 4px solid white;
      transform: rotate(45deg) translate(-100px, 100px);
      transition: 0.5s;
    }
    
    
    a:hover{
      width: 200px;
      transition-delay: 0.25s;
    }
    
    
    a:hover::before{
      transform: rotate(45deg) translate(150px, -150px);
    }
    
    
    a:hover::after{
      transform: rotate(45deg) translate(-50px, 50px);
      transition-delay: 0.75s;
    }
    
    
    a:hover span{
      visibility: visible;
      transition-delay: 0.5s;
      opacity: 1;
      transform: translate(0px);
    }
    
    
    a span{
      visibility: hidden;
      opacity: 0;
      white-space: nowrap;
      transform: translate(-30px);
      transition: 0.5s;
      margin-left: 35px;
    }
    
    
    
    
    </style>
    
    
    
    
    
