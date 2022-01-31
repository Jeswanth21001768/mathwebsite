# Web Page for Mathematical Calculations

## AIM:

To design a static website with validation to perform mathematical calculations in client side.

## DESIGN STEPS:

### Step 1:

Requirement collection.

### Step 2:

Creating the layout using HTML and CSS.

### Step 3:

Write javascript to perform the calculations.

### Step 4:

Include regularexpression based input validation.

### Step 5:

Validate the layout in various browsers.

### Step 6:

Validate the HTML code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Volume</title>
    <style>
        * {
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}
body {
  background-color:rgb(18, 233, 233);
}
.container {
  width: 1080px;
  margin-left: auto;
  margin-right: auto;
}
.content {
  display: block;
  width: 100%;
  background-color: #32f142;
  min-height: 500px;
  margin-top: 150px;
}
.content2{
    display: block;
    width: 100%;
    background-color: #f1ee24;
    min-height: 500px;
    margin-top: 150px;
    margin-bottom: 150px;
}
h1{
    text-align: center;
    padding-top: 50px;
    color: rgb(36, 23, 23);
}
.formelement{
    text-align: center;
    font-size:xx-large;
    margin-top: 5px;
    margin-bottom: 5px;

}
.by{
    text-align: center;
    color: rgb(238, 12, 12);
}
    </style>
</head>
<body>
    <div class="container">
        <div class="content">
            <h1><B>Area of Triangle</B></h1>
            <form>
                <div class=formelement>
                    <lable for="aedit">Base:</lable>
                    <input type="text" id="aedit" value="0">
                </div><br>
                <div class=formelement>
                    <lable for="bedit">Height:</lable>
                    <input type="text" id="bedit" value="0">
                </div><br>
                <div class=formelement>
                    <input type="button" value="Calculate Area" id="calbutton">
                </div><br>
                <div class=formelement>
                    <lable for="cedit">Area:</lable>
                    <input type="text" id="cedit" readonly="0">
                </div><br>
                <div class=formelement>
                    Formula : Area = (Base*Height)/2
                </div>
            </form>
        </div>
        <script type="text/javascript">
            var button;
            button=document.querySelector("#calbutton");
            button.addEventListener("click",function(){
                var atext,btext,ctext;
                var aval,bval,cval;
                atext=document.querySelector("#aedit");
                btext=document.querySelector("#bedit");
                ctext=document.querySelector("#cedit");

                aval=parseInt(atext.value);
                bval=parseInt(btext.value);
                cval=0.5*aval*bval;
                ctext.value=""+cval;
            });
        </script>
        <div class="content2">
            <h1><B>Volume of Cone</B></h1>
            <form>
                <div class="formelement">
                  <lable for="radiusedit">Radius:</lable>
                  <input type="text" id="radiusedit" value=" ">
                </div><br>
                <div class="formelement">
                  <lable for="heightedit">Height:</lable>
                  <input type="text" id="heightedit" value=" ">
                </div><br>
                <div class="formelement">
                  <input type="button" value="Calculate Volume" id="calbutton">
                </div><br>
                <div class="formelement">
                  <lable for="volumeedit">Volume:</lable>
                  <input type="text" id="volumeedit" readonly="0">
                </div><br>
                <div class="formelement">
                Formula : Volume=(π*Radius<sup>2</sup>*Height)/3
                </div><br>
                
            </form>
    
            </div>
        </div>
        <script type="text/javascript">
          var button;
          button=document.querySelector("#calbutton");
          button.addEventListener("click",function(){
            
              var radiustext,heighttext,volumetext;
              var aval,bval,cval;
    
              radiustext=document.querySelector("#radiusedit");
              heighttext=document.querySelector("#heightedit");
              volumetext=document.querySelector("#volumeedit");
      
              aval=parseInt(radiustext.value);
              bval=parseInt(heighttext.value);
              cval=3.14*aval*aval*bval/3;
              ctext.value=""+cval;
        
      
            });
                  
        </script>     

      <p class="by"><B>Developed by : jeswanth </B></p>
</body>
</html>
```


## OUTPUT:
![](1.jpg)
![](2.jpg)



## Result:

Thus a website is designed to perform mathematical calculations in the client side.

