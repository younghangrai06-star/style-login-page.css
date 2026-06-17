@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap");
*{
    margin: 0;
    Padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}
body{
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;

    background-image: url("landscape.jpg");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
}

header{
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 20px 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 99;
}
.logo{
    font-size:2em ;
    color: #fff;
    user-select: none;
}
.navigation a{
    position: relative;
    font-size: 1.1em;
    color: #fff;
    text-decoration: none;
    font-weight: 500;
    margin-left: 40px;
}
.navigation a::after{
    content: '';
    position: absolute;
    left: 0;
    bottom: -6px;
    width: 100%;
    height: 3px;
    background: #fff;
    border-radius: 5px;
    transform-origin: right;
    transform: scaleX(0);
    transition: transform 0.5s; 
}
    transform-origin: left;
    transform: scaleX(1);
}
.navigation .btnLogin-popup{
    width: 130px;
    height: 50px;
    background: transparent;
    border: 2px solid #fff;
    outline: none;
    border-radius: 6px;
    cursor: pointer;
    font-size: 1.1em;
    color: #fff;
    font-weight: 500;
    margin-left: 40px;
    transition: 0,5s;

}
.navigation .btnLogin-popup:hover{
    background: #fff;
    color: red;  
}
.wrapper{
    position: relative;
    width: 400px;
    height: 450px;
    background:transparent;
    border: 2px solid  rgba(255,255,255,0.1);;
    border-radius: 20px;
    backdrop-filter: blur(20px);
    box-shadow: 0 15px 35px rgba(0,0,0,0.5);
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
}

.wrapper .form-box{
    width: 100%;
    padding: 40px;
}
.form-box h2{
    font-size: 2em;
    color: #ffffff;
    text-align: center;
}

.input-box{
    position: relative;
    width: 100%;
    height: 50px;
    border-bottom: 2px solid #0091ff;
    margin-top: 30px 0;
}
.input-box label{
    position: absolute;
    top: 50%;
    left: 5px;
    color: #172c3b;
    font-size: 1em;
    font-weight: 500;
    pointer-events: none;
    transform: translateY(-50%);
    transition: 0.5s;
}

.input-box input:focus ~ label,
.input-box input:valid ~ label{
    top: -5px;
    color: #162938;
    font-size: 0.75em;
}

.input-box input:{
    width: 100%;
    height: 100%;
    background: transparent;
    border: none;
    outline: none;
    color: #162938;
    font-size: 1em;
    font-weight: 600;
    padding: 0 35px 0 5px;
   
}
.input-box .icon{
    position: absolute;
    right: 8px;
    top: 50%;
    transform: translateY(-50%);
    font-size: 1.2em;
    color: #192935;
    cursor: pointer;
    line-height: 50px;
}

.remember-forgot{
    font-size: 0.9em;
    color: #ffffff;
    font-weight: 500;
    margin: -15px 0 15px;
    display: flex;
    justify-content: space-between;
}
.remember-forgot label input{
    accent-color: #0091ff;
    margin-right: 3px;
}
.remember-forgot a{
    color: #ffffff;
    text-decoration: none;
}
.remember-forgot a:hover{
    text-decoration: underline;
}

.btn{
    width: 100%;
    height: 45px;
    background: #056ef7;
    border: none;
    outline: none;
    border-radius: 6px;
    color: #fff;
    font-size: 1.1em;
    font-weight: 500;
    cursor: pointer;
}

.login-register{
    margin-top: 20px;
    font-size: 0.9em;
    color: #ffffff;
    text-align: center;
    font-weight: 500;
    margin-top: 20px 0 10px;
}

.login-register p a{
    color: #f3f3f3;
    text-decoration: none;
    font-weight: 600;
}

.login-register p a:hover{
    text-decoration: underline;
}
.glass-container{
    width:400px;
    padding:40px;
    border-radius:20px;
    backdrop-filter:blur(15px);
    background:rgba(255,255,255,0.15);
    border:1px solid rgba(255,255,255,0.3);
    box-shadow:0 8px 32px rgba(0,0,0,0.3);
}

.glass-container h2{
    color:#fff;
    text-align:center;
    margin-bottom:25px;
    font-size:36px;
}

.input-box{
    margin-bottom:20px;
}

.input-box label{
    display:block;
    color:#fff;
    margin-bottom:8px;
    font-size:14px;
}

.input-box input{
    width:100%;
    padding:12px;
    border:none;
    outline:none;
    border-radius:8px;
    background:rgba(255,255,255,0.25);
    color:#fff;
    font-size:16px;
}

.input-box input::placeholder{
    color:#eee;
}

.login-btn{
    width:100%;
    padding:12px;
    border:none;
    border-radius:8px;
    background:#0d6efd;
    color:white;
    font-size:18px;
    cursor:pointer;
    margin-top:15px;
}

.login-btn:hover{
    background:#0b5ed7;
}

.register-link{
    text-align:center;
    margin-top:20px;
    color:#fff;
}

.register-link a{
    color:#fff;
    font-weight:bold;
}
.close-icon{
    position: absolute;
    top: 0px;
    right: 0px;
    font-size: 1.5em;
    color: #ffffff;
    cursor: pointer;
    background: rgba(255, 255, 255, 0.2);
    font-size: 2em;
    display: flex;
    justify-content: center;
    border-bottom-left-radius: 10px;
    z-index: 1;
  
}
.close-icon:hover{
    color: #000000;
}
.close-icon ion-icon{
    pointer-events: none;
}
