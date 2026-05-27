# Ex09 Event Registration Web Application
## Date:27-05-2026

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```

    <!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1"/>
<meta charset="utf-8" />
<link rel="stylesheet" href="globals.css">
<link rel="stylesheet" href="style.css">
</head>
<body>
<div class="frame" ><img class="bg" src="img/bg-1.png" />
<img class="sec-logo" src="img/sec-logo-01as-1.png" />
<img class="img" src="img/sec-logo-1.png" />
<div class="rectangle" ></div>
<div class="text-wrapper" >LOGIN</div>
<div class="div" ></div>
<div class="text-wrapper-2" >REGISTER</div></div>
</body>
</html>

.frame {
  background-image: url(./img/frame-1.png);
  background-size: cover;
  background-position: 50% 50%;
  width: 100%;
  min-width: 304px;
  min-height: 536px;
  position: relative;
}

.frame .bg {
  position: absolute;
  top: 0;
  left: 0;
  width: 304px;
  height: 536px;
  aspect-ratio: 1.37;
}

.frame .sec-logo {
  position: absolute;
  top: 45px;
  left: 10px;
  width: 294px;
  height: 60px;
  aspect-ratio: 4.97;
  object-fit: cover;
}

.frame .img {
  position: absolute;
  top: 124px;
  left: 76px;
  width: 118px;
  height: 114px;
  aspect-ratio: 1.04;
  object-fit: cover;
}

.frame .rectangle {
  position: absolute;
  top: 292px;
  left: 62px;
  width: 145px;
  height: 59px;
  background-color: #262222;
}

.frame .text-wrapper {
  position: absolute;
  top: 307px;
  left: 90px;
  width: 90px;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #ffffff;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}

.frame .div {
  position: absolute;
  top: 394px;
  left: 37px;
  width: 195px;
  height: 47px;
  background-color: #372f2f;
}

.frame .text-wrapper-2 {
  position: absolute;
  top: 406px;
  left: 60px;
  width: 147px;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #ffffff;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}


    <!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1"/>
<meta charset="utf-8" />
<link rel="stylesheet" href="globals.css">
<link rel="stylesheet" href="style.css">
</head>
<body>
<div class="frame" ><img class="disco-lights-shiny" src="img/disco-lights-shiny-backgound-1302-8483-1.png" />
<div class="text-wrapper" >BOOK EVENT</div>
<p class="welcome-address-lamp" ><br/>Welcome Address<br/>Lamp Lighting<br/>Guest Introduction<br/>Book Introduction<br/>Book Release<br/>Chief Guest Speech<br/>Vote of Thanks<br/>National Anthem</p></div>
</body>
</html>

.frame {
  background-color: #121d55;
  width: 100%;
  min-width: 331px;
  min-height: 536px;
  position: relative;
}

.frame .disco-lights-shiny {
  position: absolute;
  top: 0;
  left: 0;
  width: 331px;
  height: 536px;
  aspect-ratio: 1;
  object-fit: cover;
}

.frame .text-wrapper {
  position: absolute;
  top: 42px;
  left: 53px;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #000000;
  font-size: 32px;
  letter-spacing: 0;
  line-height: normal;
}

.frame .welcome-address-lamp {
  position: absolute;
  top: 100px;
  left: 43px;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #000000;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}


    <!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1"/>
<meta charset="utf-8" />
<link rel="stylesheet" href="globals.css">
<link rel="stylesheet" href="style.css">
</head>
<body>
<div class="frame" ><img class="design" src="img/design-congratulatory-background-award-event-using-lights-concept-clean-simple-mesmeris-1101825-23073-1.png" />
<img class="bg" src="img/bg-2.png" />
<div class="text-wrapper" >FOR DETAILS</div>
<div class="CONTACT" >CONTACT : 9363741740<br/>EMAIL:sec@gmail.com</div>
<div class="ADDRESS-SAVVETHA" >ADDRESS:<br/>SAVVETHA ENGINEERING<br/>COLLEGE</div></div>
</body>
</html>

.frame {
  background-color: #ad91e2;
  width: 100%;
  min-width: 331px;
  min-height: 536px;
  position: relative;
}

.frame .design {
  position: absolute;
  top: 0;
  left: 0;
  width: 331px;
  height: 536px;
  aspect-ratio: 1;
  object-fit: cover;
}

.frame .bg {
  position: absolute;
  top: 0;
  left: 0;
  width: 331px;
  height: 536px;
  aspect-ratio: 1.37;
  object-fit: cover;
}

.frame .text-wrapper {
  position: absolute;
  top: 65px;
  left: 39px;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #000000;
  font-size: 32px;
  letter-spacing: 0;
  line-height: normal;
}

.frame .CONTACT {
  position: absolute;
  top: 150px;
  left: 35px;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #000000;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}

.frame .ADDRESS-SAVVETHA {
  position: absolute;
  top: 312px;
  left: 19px;
  font-family: "Inter-Regular", Helvetica;
  font-weight: 400;
  color: #000000;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}


```



## OUTPUT:
![alt text](<Screenshot 2026-05-26 214039.png>)


## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
