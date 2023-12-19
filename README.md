<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aug 15th</title>
    <style>
      body {
        font-family: 'Arial', sans-serif;
        text-align: center;
        padding: 20px;
      }
  
      p {
        font-size: 24px;
        margin: 5px;
        padding: 5px;
        background-color:aqua;
        border-radius: 5px;
      }
  
      p.countdown {
        color: #333;
        
      }
  
      p.message {
        color: #0ae040;
        font-weight: bold;
      }
    </style>
</head>
<body>
    
    <script>
        function countdown(num, callback) {
          if (num >= 0) {
            document.body.innerHTML += '<p>' + num + '</p>';
            setTimeout(function () {
              countdown(num - 1, callback);
            }, 1000);
          } else {
            callback();
          }
        }
        
        countdown(10, function () {
          document.body.innerHTML += '<p>Happy Independence Day All Of You! WD-54 Batch Team😎</p>';
        });
        </script>
  
</body>
</html>
