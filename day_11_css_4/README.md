# CSS3 Navigation Bar

navigation bar is built by list `<ul><li></ul>`

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ruet Template</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <link rel="icon" type="image/png" href="ruet.png">
    <style>

       body
       {
          margin:0;
          padding:0;
          background-image:url("bg-header.png");
          font-family: cursive;

       }
      .main
       {
          margin-right: auto;
          margin-left: auto;
          padding-left: 25px;
          padding-right: 25px;

       }
       #horizontal ul
       {
             list-style-type: none;
          border-bottom: 6px solid rgb(17,111,126);
             margin:0px;
             padding: 0px;
             overflow: hidden;

       }
       #horizontal ul li
       {
             float:left;
          padding-right: 11px;
          width:120px;



       }
       #horizontal ul li:last-child {

           padding-right: 0px;
       }
       #horizontal ul li a
       {

             display:block;
             color:white;
             text-align: center;
             text-decoration: none;
             padding: 16px;
          background-color: rgba(123, 255, 250, 0.12);
       }
       #horizontal ul li a:hover
       {
             background-color: rgba(48,152,133,0.41);

       }


       img
       {
          max-width: 100%;
          height: auto;
       }


      #horizontal ul ul
      {
          display: none;
          position: absolute;
          margin:0px;
          padding: 0px;
          list-style-type: none;

      }


       #horizontal ul li:hover > ul
       {
              display: block;
              width:280px; 
              border-bottom: none; 
              height: 600px;




       }

       #horizontal ul ul li
       {
          clear: both;
          width:120px;

       }

        #horizontal ul li ul li a
       {
         clear: both;
         color: white;
         padding: 12px 16px;
         text-decoration: none;
         display: block;
         text-align: left;
         border-top: 1px solid white;
         background-color: rgba(0, 140, 186, 0.85);
         -moz-transition: padding 600ms;
         -webkit-transition: padding 600ms;
         transition: padding 600ms;
       }

      #horizontal ul li ul li a:hover
       {
          background-color: rgba(0, 180, 186, 1);
          padding:20px 16px;
       }

       #horizontal ul ul ul
       {
           margin-left: 120px;
           top: 50px;
           width: 150px;


       }

       #horizontal  ul ul ul.nav
       {
           margin-left: 120px;
           top: 0px;
           width: 150px;


       }

        #horizontal ul ul ul li
       {

           width: 150px;


       }



       .part
       {

              position: absolute;
              left: 0;
              width: 100%;
              height: 590px;
              top: 0;
              z-index: -1;
              background-image: url("bg-textura3.png");


       }

      .logo
       {
             margin-top: 10px;
             background-color: rgba(16, 100, 112,0.41);
             height:100px;
             width:100%;
             text-align: center;



       }
       .wr
       {

          max-width:650px;
          margin:auto;
          height: auto;   

       }
       .adjust
       { 
           padding-top: 20px;
           margin-left: 10px;
           padding-left: 10px;
           font-size:20px; 
           color: white;
           font-family: cursive;
       }


  </style>
</head>


<body>
<div class="part"></div>
  <div class="main">

    <div class="logo">

        <div class="wr"><img style="float:left;" src="ruet.png" width="80px" height="80px" /><div class="adjust">Rajshahi University Of Engineering And Technology</div></div>
    </div>


<div id="horizontal">
  <ul>
   <li><a href="#"><i style="font-size: 20px;" class="fa fa-home"></i></a></li>
   <li><a href="#">Home</a></li>
   <li><a href="#">Notice</a></li>
   <li ><a href="#" class="">Department</a>
   <ul>

      <li><a href="#">CSE</a>

       <ul class="nav">
             <li><a href="#">Achievements</a></li>
             <li><a href="#">Prizes</a></li>

          </ul>


      </li>
      <li><a href="#">EEE</a>

          <ul>
             <li><a href="#">News</a></li>
             <li><a href="#">Achievements</a></li>

          </ul>


      </li>

      <li><a href="#">ETE</a></li>
    </ul>

   </li>

   <li><a href="#">Lab</a></li>
   <li><a href="#">Gallery</a></li>
   <li><a href="#">Admission</a></li>
   <li><a href="#">Result</a></li>
   <li><a href="#">Login</a></li>
   <li><a href="#">Registration</a></li>




  </ul>
  </div>
  </div>
  </body>
  </html>
```

## CSS3 Transition

transition gives slow effect \(smoothly\) to change a property of css based on time \(mili seconds\) .

```html
<!DOCTYPE html>
<html>
<head>
    <title>Transition</title>
    <style>

    .cse
    {
        padding:30px;
        border:1px solid gray;
        border-radius: 0px;
        margin:50px;
        color: white;
        font-weight: bold;
        text-align: center;
        font-size: 40px;
        float: left;
        width: 350px;
        height: auto;
        background-color:rgb(71,49,108);
       -webkit-transition: width 2s;
        -moz-transition: width 2s;
    }
    .cse:hover
    {
        width:500px;
    }



    </style>
</head>
<body>
<div class="cse">CSE</div>
</body>
</html
```

## CSS Transform

```html
<!DOCTYPE html>
<html>
<head>
    <title>Transition</title>
    <meta name="description" content="">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <style>



   .cse
   {

    padding:30px;
    border:1px solid gray;
    border-radius: 0px;
    margin:50px;
    color: white;
    font-weight: bold;
    text-align: center;
    font-size: 40px;
    float: left;
    max-width: 350px;
    height: auto;
    background-color:rgb(71,49,108);
    -webkit-transition: transform 300ms;
   -moz-transition: -moz-transform 300ms;


   }

.cse:hover
{
    -webkit-transform: scale(1.4);
  -moz-transform: scale(1.4);
  -ms-transform: scale(1.4);
  -o-transform: scale(1.4);
  transform: scale(1.4);  
}

.container
{
    margin-left: auto;
    margin-right: auto;
    max-width: 800px;
}


    </style>
</head>
<body>
<div class="container">
    <div class="cse">
      CSE

    </div>
    <div class="cse">
      EEE
    </div>

    <div class="cse">
      ECE
    </div>






</div>
</body>
</html>
```

#### transition-timing-function

`ease`

* specifies a transition effect with a slow start, then fast, then end slowly 

`linear`

* specifies a transition effect with the same speed from start to end

`ease-in`

* specifies a transition effect with a slow start

`ease-out`

* specifies a transition effect with a slow end

`ease-in-out`

* specifies a transition effect with a slow start and end

## CSS3 Box Shadow

```html
<!DOCTYPE html>
<html>
<head>
    <title>Transition</title>
    <style>

    .cse
    {
        padding:30px;
        border:1px solid gray;
        border-radius: 0px;
        margin:50px;
        color: white;
        font-weight: bold;
        text-align: center;
        font-size: 40px;
        float: left;
        width: 350px;
        height: auto;
        box-shadow: 2px 2px 2px 2px gray;
        background-color:rgb(71,49,108);
        -webkit-transition: width 2s;
        -moz-transition: width 2s;
        transition-timing-function: ease-in;
    }
    .cse:hover
    {
        width:500px;
    }



    </style>
</head>
<body>
<div class="cse">CSE</div>
</body>
</html>
```



