<!-- ---------------------------------------------------------------------- -->
<div class="page-back">

[<-- BACK](/FRApps/fr020100_My-HTML-Custom)

</div><div class="page-next">

<!-- ---------------------------------------------------------------------- -->
___

HTML

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <meta http-equiv="X-UA-Compatible" content="ie=edge">
        <title>HTML Custom Apps</title>
        <link rel="shortcut icon" href="assets/images/favicon.png">
        <link rel="stylesheet"    href="https://fonts.googleapis.com/css?family=EB Garamond" >
        <link rel="stylesheet"    href="https://fonts.googleapis.com/css?family=Roboto+Slab" >
        <link rel="stylesheet"    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">
        <link rel="stylesheet"    href="index.css">

    <!-- INSERT Point - DATA FETCHING -->
    <!-- END INSERT Point - DATA FETCHING -->
    </head>

    <body>    

    <!-- REPLACE Point - Header -->
        <div class="Header">

        <!-- INSERT Point - Responsive -->
            <div class="MenuWrap">
                <input title="Menu" type="checkbox" class="Toggler">
                <div class="Hamburger"><div></div></div>
                <div class="Menu">
                    <div>
                        <div>
                            <ul class="MenuList">
                                <li class="MenuListItem" id="H-PHLink" ><a href="#" >Home</a></li>
                                <li class="MenuListItemLine" id="PHLinkLine" ><hr></li>
                                <li class="MenuListItem" id="H-PHLinkCTA" ><a href="#" >H-PH_CTA</a></li>
                                <li class="MenuListItem" id="H-PHLink" ><a href="#" >H-PH_Link1</a></li>
                                <li class="MenuListItem" id="H-PHLink" ><a href="#" >H-PH_Link2</a></li>
                                <li class="MenuListItem" id="H-PHLink" ><a href="#" >H-PH_Link3</a></li>
                                <li class="MenuListItemLine" id="PHLinkLine" ><hr></li>
                                <li class="MenuListItem" id="F-PHLink" ><a href="#" >F-PH_Link1</a></li>
                                <li class="MenuListItem" id="F-PHLink" ><a href="#" >F-PH_Link2</a></li>
                                <li class="MenuListItemLine" id="PHLinkLine" ><hr></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        <!-- END INSERT Point - Responsive -->
        <!-- REPLACE Point Logo -->
            <div class="HeaderLogo"><a href="#">PH Logo</a></div>
        <!-- END REPLACE Point - Logo -->
            <div class="HeaderSpacer"></div> 
            <ul class="HeaderNavList">
                <li class="HeaderNavListItem"><a href=#>PH_Link1</a></li>
                <li class="HeaderNavListItem"><a href=#>PH_Link2</a></li>
                <li class="HeaderNavListItem"><a href=#>PH_Link3</a></li>
                <!-- INSERT Point - Dropdown Menu -->
                <!-- END INSERT  -  Dropdown Menu -->
                <li class="HeaderNavListItemCTA"><a href=#>PH_CTA</a></li>
            </ul>
        </div>
    <!-- END REPLACE Point - Header -->


    <!-- REPLACE Point - Section1 -->
        <div class="Section1">
            <h2 class="Section1ImageText">PH Text Overlay</h2>
        </div>
    <!-- END REPLACE Point - Section1 -->

    <!-- REPLACE Point - Section2 -->        
        <div class="Section2">
            <h2></h2>
            <p class="Section2Paragraph">
                PH<br>
                The quick brown fox jumped over the lazy dog.<br>
                The quick brown fox jumped over the lazy dog.<br>
                The quick brown fox jumped over the lazy dog.<br>
                The quick brown fox jumped over the lazy dog.
            </p>  
        </div>
    <!-- END REPLACE Point - Section2 -->       

    <!-- REPLACE Point - Footer -->
        <div class="Footer">
            <ul class="FooterNavList">
                <li class="FooterNavListItem"><a href=#>PH Link1</a></li>
                <li class="FooterNavListItem"><a href=#>PH Link2</a></li>
            </ul>
        </div>
    <!-- END REPLACE Point - Footer -->
    </body>

</html>

```

___


CSS

```css


/* Basic Blocks Custom App */
@import url('https://fonts.googleapis.com/css?family=EB+Garamond');
@import url('https://fonts.googleapis.com/css2?family=Frank+Ruhl+Libre');
@import url('https://fonts.googleapis.com/css2?family=Roboto+Slab:wght@900&display=swap');

/*=============================================*/
/* root REPLACE Point - :root */
/*----------------------------------------------
:root selector for variables
-----------------------------------------------*/
:root {
    --Body_background-color: #E5E4E2; /*platinum*/
   
    --Header_background-color: red;
    --Header_hover-color: white;
    --HeaderLogo-image: "";
    --HeaderLogo_margin: 35px 0 0 0px;
    --HeaderLogo-FontFamily: "Roboto Slab";
    --HeaderList-font-size: 1.2rem;
  
    --Section1_background-color: blue;
    --Section1_background-image: url( 'assets/images/monaco-blue-soft.jpg' );
  
    --Section2_background-color: lightgray;
    --Section2Paragraph-font-color: #ff7034;  /* dark orange */
  
    --Footer_background-color:green;
    --Footer_hover-color: white;
    --FooterList-font-size: .9rem;  
    
    --GlobalFontFamily: "Frank Ruhl Libre", "EB Garamond";

    --Button_Logo_font-color: whitesmoke;
} 
/* END REPLACE :root ==========================*/


/*=============================================*/
/* HTML REPLACE Point */
/*----------------------------------------------
The <html> tag properites (unchanged)
-----------------------------------------------*/
html {
    background: var(--Body_background-color);
    height: 100%;
    text-align: center;
    max-width: 1000px;
    margin: auto;
}
/* END HTML ===================================*/


/*----------------------------------------------
The body properites
-----------------------------------------------*/
body {
    background: var(--Body_background-color);
    height: 100%;
    width: 100%;
    margin: 0;
    font-family: var(--GlobalFontFamily);
}

/*----------------------------------------------
The <h2> tag properties
-----------------------------------------------*/
h2 {
    margin: 0;
    font-size: 1.5rem;
    color: white;
    padding: 1.5rem;
    text-align: center;
}

/*===============================================*/
/* HR-1 REPLACE Point - .Header */
/*------------------------------------------------
The .Header properites
-------------------------------------------------*/
.Header {
    background: var(--Header_background-color);
    width: 100%;
    height: 80px;
    position: fixed;  /*was relative*/
    z-index: 100;
    max-width: 1000px;
    margin: auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
/* END HR-1 .Header =============================*/


/*===============================================*/
/* H-2 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/*===============================================*/
/* H2 INSERT Point - .HeaderLogo */
/*------------------------------------------------
The .HeaderLogo properites
-------------------------------------------------*/
.HeaderLogo {
    margin-left: 5px;
    padding-left: 25px;
}

/*===============================================*/
/* INSERT Point - .HeaderLogo a */
/*------------------------------------------------
The .HeaderLogo a properites
-------------------------------------------------*/
.HeaderLogo a {
    text-decoration: none;
    font-size: 1.5rem;
    font-family: var(--HeaderLogo-FontFamily);
    font-weight: 600;    
    color: var(--Button_Logo_font-color);
    background: blue ;
    padding: 0.5rem .5rem;
    border-radius: 8px;
    box-shadow: 4px 4px black;
}

/*===============================================*/
/* INSERT Point - .HeaderSpacer */
/*-------------------------------------------------
The .HeaderSpacer properites
-------------------------------------------------*/
.HeaderSpacer {
    flex: 1;
}
/* H-2 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/*===============================================*/
/* H-3 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/*===============================================*/
/* H-3 INSERT Point - .HeaderNavList */
/*------------------------------------------------
The .HeaderNavList (horizontal menu) properites
-------------------------------------------------*/
.HeaderNavList {
    list-style: none;
    margin-right: 30px;
    padding: 0;
    display: flex;
    flex-direction: row;
    align-items: center;
    font-size: var(--HeaderList_font-size);
}

/* INSERT Point .HeaderNavListItem a */
/*------------------------------------------------
The .HeaderNavListItem a properites
-------------------------------------------------*/
.HeaderNavListItem a {
    color: black;
    font-weight: bold;
    text-decoration: none;
    margin: 8px 0;
    padding: 25px;
}

/* INSERT Point .HeaderNavListItem a:hover
                .HeaderNavListItem a:active */
/*------------------------------------------------
The .HeaderNavListItem a properites
-------------------------------------------------*/
.HeaderNavListItem a:hover,
.HeaderNavListItem a:active {
    color: var(--Header_hover-color);
}
/* H-3 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/*===============================================*/
/* H-4 INSERT Point - .HeaderNavListItemCTA a */
/*------------------------------------------------
The .HeaderNavListItemCTA a properties
-------------------------------------------------*/
.HeaderNavListItemCTA a {
    color: var(--Button_Logo_font-color);
    background: blue ;
    padding: 0.5rem 1rem;
    border-radius: 8px;
    text-decoration: none;
    font-family: var(--GlobalFontFamily);
    font-weight: 600;
}
/* END H-4 .HeaderNavListItemCTA a ==============*/


/*===============================================*/
/* H-5 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* H-5 INSERT Point - .HeaderNavListItemCTA */
/*------------------------------------------------
The .HeaderNavListItemCTA properties
-------------------------------------------------*/
.HeaderNavListItemCTA {
    animation     : wiggle 400ms 2s 8 ease-out none;
    }
  
  /*===============================================*/
  /* INSERT Point - @keyframes wiggle */
  /*------------------------------------------------
  The @keyframes wiggle properties
  -------------------------------------------------*/
  @keyframes wiggle {
      0% { transform: rotateZ(  0deg ); }
     50% { transform: rotateZ(-10deg ); }
    100% { transform: rotateZ( 10deg ); }
  }
/* H-5 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
  

/*===============================================*/
/* D-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* INSERT DROPDOWN ==============================*/

/* END DROPDOWN */
/* D-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/*===============================================*/


/*===============================================*/
/* S1R-1 REPLACE Point - Section1 */
/*------------------------------------------------
The .Section1 properites
-------------------------------------------------*/
.Section1 {
    background: var(--Section1_background-color);
    width: 100%; /*was 300px*/
    height: 46%; /*was 100px*/
    position: relative;
    top: 80px; /*<---ADD to adjust the top position*/
}
/* END S1R-1 .Section1 ===========================*/


/*===============================================*/
/* S1-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/*===============================================*/
/* S1-1 INSERT Point - .Section1ImageText */
/*------------------------------------------------
The .Section1ImageText properties
-------------------------------------------------*/
.Section1ImageText {
    font-family: var(--GlobalFontFamily);
    font-size: 3rem;
    font-weight: 800;
    color: lightgray;
    text-shadow: 1px 1px 3px #000000;
    padding: 80px 250px 20px 0px;
}

/*===============================================*/
/* INSERT Point - .Section1ImageText::first-letter */
/*------------------------------------------------
The .Section1ImageText::first-letter properties
-------------------------------------------------*/
.Section1ImageText::first-letter {
    font-size: 150%;
    color: cornflowerblue;
}
/* S1-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/

/*=============================================*/
/* S2 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/

/*===============================================*/
/* S2R-1 REPLACE Point - Section2 */
/*------------------------------------------------
The .Section2 properites
-------------------------------------------------*/
.Section2 {
    background: var(--Section2_background-color);
    width: 100%;
    height: 46%;
    position: relative;
    color: black;
    font-family: var(--GlobalFontFamily);
    font-size: 1.2rem;
    font-weight: 600;
    top: 80px; /*<---ADD to adjust the top position*/
}
/* END S2R-1 .Section2 ===========================*/


/*===============================================*/
/* S2-1 INSERT Point - Section2 h2 */
/*      DELETE Point - Section2 h2 */
/*-----------------------------------------------
The .Section2 h2 properites
-------------------------------------------------*/
.Section2 h2 {
    padding: 1.5;
    color: black;
}
/* END S2-1 .Section2 h2=========================*/


/*===============================================*/
/* S2-2 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* S2-2 INSERT Point - Section2Paragraph */

/* INSERT Point - Section2Paragraph::first-letter/line */
/* S2-2 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/

/* S2 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/


/*===============================================*/
/* FR-1 REPLACE Point - Footer */
/*------------------------------------------------
The .Footer properites
-------------------------------------------------*/
.Footer {
    background: var(--Footer_background-color);
    width: 100%; 
    /*top: 80px;  Removed in place of the bottom property*/
    bottom: 0;
    position: fixed;
    z-index: 99;
    max-width: 1000px;
    margin: auto;
  } 
/* END FR-1 .Footer =============================*/


/*===============================================*/
/* F-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/*===============================================*/
/* F1 INSERT Point - .FooterNavList */
/*------------------------------------------------
The .FooterNavList properties
-------------------------------------------------*/
.FooterNavList {
    list-style: none;
    margin: 20px;
    padding: 0;
    display: flex;
    flex-direction: row;
    justify-content: center;
    font-size: var(--FooterList-font-size);
}

/*===============================================*/
/* INSERT Point - .FooterNavListItem a */
/*------------------------------------------------
The .FooterNavListItem a properties
-------------------------------------------------*/
.FooterNavListItem a {
    color: black;
    font-weight: bold;
    text-decoration: none;
    margin: 8px 0;
    padding: 12px;
}

/*===============================================*/
/* INSERT Point - .FooterNavListItem a:hover
                  .FooterNavListItem a:active */
/*------------------------------------------------
The .FooterNavListItem a:hover,
    .FooterNavListItem a:active properties
------------------------------------------------*/
.FooterNavListItem a:hover,
.FooterNavListItem a:active {
  color: var(--Footer_hover-color);
}
/* F-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/



/*~~~~~~~~~~~ VERY LARGE BLOCK OF CODE ~~~~~~~~~~*/
/*===============================================*/
/* HAM HAMBURGER START BLOCK ^^^^^^^^^^^^^^^^^^^^*/
/* Hamburger Code */

/* MENU (3 bars) STYLES */
.MenuWrap {
    position: fixed;
    top: 0;
    left: 0;
    z-index: 1;
    display: none;
  }
  .MenuWrap .Toggler {
    position: absolute;
    top: 0;
    left: 0;
    z-index: 2;
    cursor: pointer;
    width: 50px;
    height: 50px;
    opacity: 0;
  }
  /*===============================================*/
  /*BEGIN Make a three line Hamburger*/
  .MenuWrap .Hamburger {
    position: absolute;
    top: 0;
    left: 0;
    z-index: 1;
    width: 30px;
    height: 30px;
    padding: 18px 16px 10px 16px;
    background: var(--Header_background-color);
      /*Red for Layout; Orange for Customization*/
    display: flex;
    align-items: center;
    justify-content: center;
  }
  
  /* Hamburger Line */
  .MenuWrap .Hamburger > div {
    position: relative;
    flex: none;
    width: 100%;
    height: 3px;
    background: blue; /*bar colors*/
    display: flex;
    align-items: center;
    justify-content: center;
    transition: all 0.4s ease;
  }
  
  /* Hamburger Lines - Top & Bottom */
  .MenuWrap .Hamburger > div::before,
  .MenuWrap .Hamburger > div::after {
    content: '';
    position: absolute;
    z-index: 1;
    top: -10px;
    width: 100%;
    height: 3px;
    background: inherit;
  }
  
  /* Moves Line Down */
  .MenuWrap .Hamburger > div::after {
    top: 10px;
  }
  /*END Make a three line Hamburger*/
  /*===============================================*/
  
  /*===============================================*/
  /* BEGIN Toggler Animation -- Allows the... */
  /*change the BGColor of the hamburger from red*/
  .MenuWrap .Toggler:checked + .Hamburger {
    background-color: whitesmoke;
    opacity: 0.3;
  }
  .MenuWrap .Toggler:checked + .Hamburger > div {
    background: var(--Header_background-color); 
      /* X color  Red in Layout; Orange for customization*/
  }
  
  /* ...three lines to turn into an animated X */
  .MenuWrap .Toggler:checked + .Hamburger > div {
    transform: rotate(135deg);
  }
  /* Turns Lines Into X */
  .MenuWrap .Toggler:checked + .Hamburger > div:before,
  .MenuWrap .Toggler:checked + .Hamburger > div:after {
    top: 0;
    transform: rotate(90deg);
  }
  /* Rotate On Hover When Checked */
  .MenuWrap .Toggler:checked:hover + .Hamburger > div {
    transform: rotate(1305deg); 
    transition-duration: .5s; 
  }
  /*END Toggler animation*/
  /*===============================================*/
  
  /*===============================================*/
  /* BEGIN Show Menu */
  .MenuWrap .Toggler:checked ~ .Menu {
    visibility: visible;
  }
  .MenuWrap .Toggler:checked ~ .Menu > div {
    transform: scale(1.1);
    transition-duration: 0.5s; 
  }
  .MenuWrap .Toggler:checked ~ .Menu > div > div {
    opacity: 1.0;
    transition:  opacity 0.1s ease;
  }
  .MenuWrap .Menu {
    position: fixed;
    top: 0;
    left: 0;
    width: 90%;
    height: 90%;
    visibility: hidden;
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 30px 0px 150px 95px;
  }
  .MenuWrap .Menu > div {
    background: whitesmoke;
    opacity: 0.95;
    border-radius: 10%;
    width: 150vw; 
    height: 350vw;     
    display: flex;
    flex: none;
    align-items: center;
  /*move menu around*/
    justify-content: left; 
    padding-left: 155px; 
    margin-top: -175px; 
  /*end of move around*/
    transform: scale(0);
    transition: all 0.5s ease;
  }
  .MenuWrap .Menu > div > div {
    text-align: center;
    max-width: 90vw;
    max-height: 100vh;
    opacity: 0.0;
    transition: opacity 0.5s ease;
  }
  .MenuWrap .Menu > div > div > ul > li {
    list-style: none;
    color: blue;
    font-weight: 800;
    padding: 5px;
    background-color: whitesmoke; 
    opacity: 1;
  }
  .MenuWrap .Menu > div > div > ul > li > a {
    font-size: .9rem;
    font-weight: 800;
    color: inherit;
    text-decoration: none;
    transition: color 0.1s ease;
  }
  /*===============================================*/
  
  /*===============================================*/
  #PHLinkLine hr {
    height: 1px;
    background-color: blue;
  }
  #H-PHLinkCTA {
    color: white;
    background: blue;
    opacity: .9;
    border-radius: 8px;
  }
  /* END Show Menu */
  /*===============================================*/
  
  /* HAMBURGER END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^*/
  /*~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~*/
  

/*===========================================*/
/* R-1 START BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/
/* Responsive Code */  
/* R-1 INSERT Point - @media (responsive max-width)*/
/*-----------------------------------------
The @media MAX-width query properties
Tablet Portrait
=========================================*/
@media only screen
and (min-width: 621px)
and (max-width: 1000px) 
{
  .Section1ImageText {
    font-size: 3rem;
    padding: 20px 200px 0px 0px;
  }
  .Section2Paragraph {
    font-size: 1rem;
    padding: 0px 0px 0px 0px;
    margin: -30px 0px 0px 0px;
  }
}  
/*-----------------------------------------
The @media MAX-width query properties
iPhone Landscape
=========================================*/
@media only screen
and (min-width: 441px)
and (max-width: 620px) 
{
  .HeaderLogo {
      font-size: 1.2rem;
      margin-left: 50px;
      background-size: 180px 51px;
  }
  .MenuWrap {
    display: flex;
  }
  .MenuWrap .Menu > div {
    /*move menu around*/
      justify-content: left;
      padding-left: 280px;
      margin-top: -280px; 
    /*end of move around*/
    }
  .HeaderNavList {
      display: none;
  }
  .Section1ImageText {
    font-size: 2.5rem;
    text-align: center;
    vertical-align: center;
    padding: 20px 150px 20px 0px;
  }
  .Section2 h2 {
    font-size: 1.7rem;
  }
  .Section2Paragraph {
    font-size: 75%;
    margin-top: -40px;
  }
  .Footer {
    display: none;
  }
}
/*-----------------------------------------
The @media MAX-width (440px) query properties
iPhone Portrait
=========================================*/
@media only screen
and (max-width: 440px)  
{
  .MenuWrap {
    display: flex;
  }
  .MenuWrap .Menu > div {
  /*move menu around*/
    justify-content: left;
    padding-left: 200px;
    margin-top: -80px; 
  /*end of move around*/
  }
  .Footer {
    display: none;
  }
  .HeaderLogo {
      font-size: .8rem;
      margin-left: 0px;
      margin-top: 0px;
      background-size: 144px 41px;
      padding: 10px 0px 20px 70px;
  }
  .HeaderNavList {
    display: none;
  }
  .Section1ImageText {
      font-size: 2rem;
      padding: 40px 80px 20px 0px;
      text-align: center;
      vertical-align: center;
    } 
  .Section2Paragraph {
      font-size: 70%;
      margin-top: -10px;
    }
  h2 {
      padding: 10;
  } 
}
/* R-1 END BLOCK ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^*/ 


/* END CSS */

```