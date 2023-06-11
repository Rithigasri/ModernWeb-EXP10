# EXPERIMENT 10: CREATE A GLIDING BOX USING CSS ANIMATION
## AIM:
To create a gliding box using CSS animation.
## ALGORITHM:
1. Create an HTML document with a head and body section.
2. In the head section, set the meta tags for character encoding, compatibility, and viewport. Also, link an external CSS file using the <link> tag.
3. Add a title for the document.
4. Define CSS styles to set the background color, margins, and positioning for the body. Create a container div with specified dimensions, border-radius, and flexbox properties for vertical centering. Style the box div with a box-shadow effect and cursor pointer, and add a hover animation to create a shadow wave effect.
5. Close all the open HTML tags to complete the structure of the document.
## PROGRAM:
### shadow.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="shadow.css"/>
    <title>Document</title>
</head>

<body>
    <div class="container">
       
        <center>
            <div class="box">
                <h4 style="color:white;padding-top: 10px;"> How I recreated a Polaroid camera with CSS gradients only</h4>
            </div>
        </center>
    </div>
</body>
</html>
```
### shadow.css
```
body{
    background-color: white;
    margin-top: 100px;
    margin-left:250px;
}
.container
{
    background-color: black;
    width:1000px;
    height:500px;
    border-radius: 25px;
    display: flex;
    flex-direction: column;
    justify-content: center;
}
.box
{
    width: 200px;
    height:100px;
    box-shadow: blue 0px 0px 0px 2px inset,black 10px -10px 0px -3px, green 10px -10px, black 20px -20px 0px -3px, yellow 20px -20px, black 30px -30px 0px -3px, orange 30px -30px,black 40px -40px 0px -3px, red 40px -40px;
    cursor: pointer;
}
.box:hover
{
    animation: shadow-wave 1s ease infinite;
}

@keyframes shadow-wave {
    0%{
        box-shadow: blue 0px 0px 0px 2px inset,black 10px -10px 0px -3px, green 10px -10px, black 20px -20px 0px -3px, yellow 20px -20px, black 30px -30px 0px -3px, orange 30px -30px,black 40px -40px 0px -3px, red 40px -40px;
    }
    20% {
        
        box-shadow: red 0px 0px 0px 2px inset,black 10px -10px 0px -3px, blue 10px -10px, black 20px -20px 0px -3px, green 20px -20px, black 30px -30px 0px -3px, yellow 30px -30px,black 40px -40px 0px -3px, orange 40px -40px;
 
      }
    40% {
        
        box-shadow: orange 0px 0px 0px 2px inset,black 10px -10px 0px -3px, red 10px -10px, black 20px -20px 0px -3px, blue 20px -20px, black 30px -30px 0px -3px, green 30px -30px,black 40px -40px 0px -3px,yellow 40px -40px;
    }
    60% {
      
        box-shadow: yellow 0px 0px 0px 2px inset,black 10px -10px 0px -3px, orange 10px -10px, black 20px -20px 0px -3px, red 20px -20px, black 30px -30px 0px -3px, blue 30px -30px,black 40px -40px 0px -3px, green 40px -40px;
    }
    80% {

        box-shadow: green 0px 0px 0px 2px inset,black 10px -10px 0px -3px, yellow 10px -10px, black 20px -20px 0px -3px, orange 20px -20px, black 30px -30px 0px -3px, red 30px -30px,black 40px -40px 0px -3px, blue 40px -40px;
    }
    100% {
      
        box-shadow: blue 0px 0px 0px 2px inset,black 10px -10px 0px -3px, green 10px -10px, black 20px -20px 0px -3px, yellow 20px -20px, black 30px -30px 0px -3px, orange 30px -30px,black 40px -40px 0px -3px, red 40px -40px;
    }
    
}
```
## OUTPUT:
![image](https://github.com/Rithigasri/ModernWeb-EXP10/assets/93427256/9f6d91f9-30e1-4c3a-a823-50fd5bb4061d)

## RESULT:
Thus, a gliding box is created using CSS animation.
