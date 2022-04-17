# Loading
Loading anime
<!doctype html>
<html lang=en>
<head>
   
    <title>Loading Text Animation</title>
    <link rel="stylesheet" type="text/css" href="css/stylesheet.css">
</head>
<body>
    <div class="loader"><span>Loading</span></div>
</body>
</html>





body
{
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    font-family: sans-serif; 
    background: linear-gradient(red, orange, yellow, green, blue, purple);


    
}
.loader 
{
    position: relative;
    font-size: 2em;
    background: #fff;
    color:  #000;
    text-transform: uppercase;
    font-weight: bold;
    letter-spacing: .5em;
    padding: 10px;
}
.loader span
{
   color: whitesmoke;
   mix-blend-mode: difference;
}
.loader:before
{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 80px;
    height: 100%;
    background: linear-gradient(red, orange, yellow, green, blue, purple);
    animation: animate 4s linear infinite;
}
@keyframes animate
{
    0%
    {
        left: 0;
    }
    50%
    {
        left: calc(100% - 80px);
    }
    100%
    {
        left: 0;
    }
}
