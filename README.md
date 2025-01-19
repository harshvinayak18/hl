<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body,html{
            margin:0;
            padding:0;
            height:100%;
        }
        .container{
            background-color:blue;
            display:flex;
            align-items:center;
            justify-content:center;
            height:100%;

        }
        .input{
            background-color:white;
            padding: 50px 100px;
            text-align: center;
            border: 5px solid black;
            border-radius: 20px;
        
        }
        pr {
            font-size:200%;

        }
        .input {
            height: 50px ;
            width:250px;
            border-radius:200px;
        }
        button{
            background-color: rgb(212, 255, 0);
            height:50px;
            <br><br><hr>
    <a href="qrcode.html">
        <button>Generate Qr</button>
      </a>
      <a href="Generate Qr.html">
        <button>Generate Qr</button>
      </a>
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="input">
            <p>Qr Code Generate</p>
            <input type="text" id="inputtext" placeholder="English"
            <button onclick="generate()">Generate Qr</button>
            
        </div>
        <div class="qr">
            <div class="img">
                <img src="" id="imgqr"><br><br>
            </div>
        </div>
    </div>
    <script>
        //string concatentaion
        let inputtext=document.getElementById("inputtext");
        let inputtext=document.getElementsById("imgqr");
        function generate() {
            imgqr.src="https://api.qrserver.com/v1/create-qr-code/?size=150x150&data="+inputtext.value;
        }
    </script>
    </body>
</html>
