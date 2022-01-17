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

<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">

  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Volume Calculator</title>
</head>

<body>

  <div class="formelement">
    <h1><small>Volume Calculator For Cylinder And Cone</small></h1>
  </div>
  <div class="container">
    <div class="content">
      <h1>Volume Of Cylinder</h1>
      <form>
        <div class=formelement>
          <lable for="aedit">Height:</lable>
          <input type="number" min="0" value="0" step="any" id="aedit" placeholder="0" /><label><small>
              Meters</small></label>
        </div><br>
        <div class=formelement>
          <lable for="bedit">Radius:</lable>
          <input type="number" min="0" value="0" step="any" id="bedit" placeholder="0" /><label><small>
              Meters</small></label>
        </div><br>
        <div class=formelement>
          <lable for="cedit">Volume:</lable>
          <input type="number" min="0" value="0" step="any" id="cedit" placeholder="0" readonly="0" /><label><small>
              Meters³</small></label>
        </div><br><br>
        <div class=formelement>
          <input type="button" class="button" value="CALCULATE" id="calbutton1" />
          <input type="Reset" class="button" onclick="" value="RESET">
        </div>
        <br>
        <div class=formula>
          Formula is
          Volume V = π X Radius² X Height
        </div><br>
      </form>
    </div>

    <div class="content2">
      <h1>Volume of Cone</h1>
      <form>
        <div class="formelement">
          <lable for="radiusedit">Radius:</lable>
          <input type="number" min="0" value="0" step="any" id="radiusedit" placeholder="0" /><label><small>
              Meters</small></label>
        </div><br>
        <div class="formelement">
          <lable for="heightedit">Height:</lable>
          <input type="number" min="0" value="0" step="any" id="heightedit" placeholder="0" /><label><small>
              Meters</small></label>
        </div><br>
        <div class="formelement">
          <lable for="volumeedit">Volume:</lable>
          <input type="number" min="0" value="0" name="avol" step="any" id="volumeedit" placeholder="0"
            readonly="0" /><label><small> Meters³</small></label>
        </div><br><br>
        <div class="formelement">
          <input type="button" class="button" value="CALCULATE" id="calbutton2" />
          <input type="Reset" class="button" value="RESET">
        </div><br>
        <div class="formula">
          Formula is:
          Volume V = π X Radius² X Height / 3
        </div>
        
        <br>
      </form>

    </div>
  </div>
  <div class="fbox">
    <div class="footer">
      <center>
       
      </center>
    </div>
  </div>
</body>
<script type="text/javascript">
  var button;
  button = document.querySelector("#calbutton1");
  button.addEventListener("click", function () {
    var atext, btext, ctext;
    var aval, bval, cval;
    atext = document.querySelector("#aedit");
    btext = document.querySelector("#bedit");
    ctext = document.querySelector("#cedit");

    aval = parseInt(atext.value);
    bval = parseInt(btext.value);
    cval = 3.14 * aval * aval * bval;
    ctext.value = "" + cval;
  });
</script>
<script type="text/javascript">
  var button;
  button = document.querySelector("#calbutton2");
  button.addEventListener("click", function () {

    var radiustext, heighttext, volumetext;
    var aval, bval, cval;

    radiustext = document.querySelector("#radiusedit");
    heighttext = document.querySelector("#heightedit");
    volumetext = document.querySelector("#volumeedit");

    aval = parseInt(radiustext.value);
    bval = parseInt(heighttext.value);
    cval = 3.14 * aval * aval * bval / 3;
    volumetext.value = "" + cval;


  });

</script>
<style>
 
  /Background Region/

  body {
    background-color: #7f5a83;
    background-image: url(./background.jpg);
    background-repeat: no-repeat;
    background-attachment: fixed;
    position: sticky;
    background-size: cover;
  }

  .container {
    width: 1080px;
    margin-left: auto;
    margin-right: auto;
  }

  / Box Region/

  .content {
    display: block;
    width: 100%;
    background-color: white;
    opacity: 60%;
    min-height: 500px;
    margin-top: 50px;
    margin-bottom: 50px;
    box-shadow: inset 0 0 15px black;
    backdrop-filter: blur(9px);
    border-radius: 10px;
    border: 1px solid whitesmoke;
  }

  .content2 {
    display: block;
    width: 100%;
    background-color: white;
    opacity: 60%;
    min-height: 500px;
    margin-top: 50px;
    margin-bottom: 50px;
    box-shadow: inset 0 0 15px black;
    backdrop-filter: blur(9px);
    border-radius: 10px;
    border: 1px solid whitesmoke;
  }

  .fbox {
    display: block;
    width: 100%;
    background-color: white;
    opacity: 60%;
    min-height: 100px;
    margin-top: 0px;
    margin-bottom: 0px;
    box-shadow: inset 0 0 15px black;
    backdrop-filter: blur(9px);
    border-radius: 10px;
    border: 1px solid whitesmoke;
  }

  .button {
    background-color: orangered;
    border: none;
    border-radius: 25px;
    color: white;
    padding: 15px 32px;
    text-align: center;
    display: inline-block;
    font-size: 16px;
    margin: 4px 2px;
    cursor: pointer;
  }

  /Text Region/
  * {
    box-sizing: border-box;
    font-family: Century Gothic, sans-serif;
  }

  h1 {
    text-align: center;
    padding-top: 50px;
    color: rgb(36, 23, 23);
  }

  .formelement {
    text-align: center;
    font-size: x-large;
    margin-top: 5px;
    margin-bottom: 5px;

  }

  .formula {
    text-align: center;
    font-size: large;
    margin-top: 5px;
    margin-bottom: 5px;
  }

  .footer p {
    margin: 0;
    line-height: 26px;
    font-size: 15px;
    color: #990099;
  }

  .footer p a {
    background: linear-gradient(to right, #f27121, #e94057, #8a2387);
    color: transparent;
    -webkit-background-clip: text;
    background-clip: text;
    text-decoration: none;
  }

  /Scroll Bar Configuration/

  ::-webkit-scrollbar {
    width: 5px;
  }

  ::-webkit-scrollbar-track {
    box-shadow: inset 0 0 5px grey;
    border-radius: 3px;
  }

  ::-webkit-scrollbar-thumb {
    background: #d86939;
    border-radius: 3px;
  }
</style>

</html>

## OUTPUT:

![](1.png)

![](2.png)

![](3.png)


## Result:

Thus a website is designed to perform mathematical calculations in the client side.
