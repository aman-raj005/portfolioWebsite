<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>amanraj005</title>
    <link rel="icon" type="image/x-icon" href="a-solid-icon.svg">
    <link rel="stylesheet"href="portfolio.css">
    <style>
        *{
    padding:0;
    margin:0;
    box-sizing:border-box;
    scroll-behavior: smooth;
    font-family:"Be Vietnam pro",sans-serif;
}

.wrapper{
           height:auto;
           width: 100%;
           overflow-y: hidden;
            overflow-x:hidden; /*auto*/

}
.container{
             width:100%;
             height:auto;
             margin:0 auto;
             overflow-x:hidden; 
             overflow-y:hidden ;
}
.logoconatiner{display: flex;
                justify-content: baseline;   
                align-items: center;            

}
.navbar{
          display: flex;
          justify-content: space-between;
          align-items: center;
          padding-top: 0.7rem;     /*1rem*/
        }
.nav-items{
             display: flex;
             gap:1.5rem;
             padding:0 3.8em;

          }
.nav-items div{ 
                font-size: 1.25rem;  /*1rem*/
                font-weight: 500;
                cursor: pointer;
              }

.logo{width:6.19rem;     /*99px*/
      padding-left: 2.5rem;  /*40px*/
      }
      @media (max-width: 768px) {
        .logo {
            width: 4rem; 
            padding-left: 1.5rem; 
        }
    }
    
    
    @media (max-width: 576px) {
        .logo {
            width: 3rem; 
            padding-left: 1rem; 
        }
    }
.logo-text{
                 margin:-0.68125rem;   /*10.9px*/
                 font-size: 1.75rem;   /*     28px    */
                
          }
          @media (max-width: 768px) {
            .logo-text {
                margin: -0.5rem; 
                font-size: 1.5rem;
            }
        }
        
        
        @media (max-width: 576px) {
            .logo-text {
                margin: -0.25rem; 
                font-size: 1.25rem; 
            }
        }
a{ 
    text-decoration: none;
   
}
.nav-items div a {
    color:black;
}
.nav-items div :hover {
                        font-weight: bold;
                        transition:4s ease-in;
}




.hero-section{
               display: flex;
               height:25rem;        
               justify-content: center;
               align-items: center;
              
               margin-left: auto;
               margin-right: auto;
               margin-top: 4rem;
               margin-bottom: 0;
             }       

.p-button{
            width:fit-content;
            display: flex;
            flex-shrink: 2;
            padding: 0.8rem 2.3rem;
            box-shadow: 0 0  0.625rem black; 
            font-size: 1.125rem;    
            cursor: pointer;
            transform: all 0.3s;
            color: antiquewhite;
             font-weight: 500;
            border: solid 0.1875 transparent; 
            background-color: brown;
            position: relative;
            z-index: 0;
          }
.p-button::before{
                    content: "";
                    padding-left: 0;
                    padding-top: 0;
                    padding-bottom: 0;
                    padding-right:0 ;
                    background-color:#fff;
                    position: absolute;
                    transform: scaleX(0);
                    transform-origin: left;
                    transition:all 0.4s;
                    z-index: 1; 
     
                  }
.p-button:hover::before {
                           transform:scaleX(1);
                        }


.hero-section-left{
                     display: flex;
                     flex-direction: column;
                     justify-content: center;
                     gap:2rem;
                    }
.herosection-heading{ 
                        display: flex;
                        flex-shrink:2;
                       font-size:2.1875rem; /*  35px*/
                       color:#343d68;
                       font-weight:500;
                     }

@media (max-width: 768px) {
                        .herosection-heading {
                            font-size: 1.5rem;
                            opacity: 0; /* Adjust font size for smaller screens */
             }
        }
.role{
    font-size: 3rem;
       font-weight: 800;
       color:#4e45d5; 
     }

     @media (max-width: 768px) {
        .role {
          font-size: 2rem; /* Adjust font size for smaller screens */
        }
      }
      
      /* Media query for even smaller viewports */
      @media (max-width: 576px) {
        .role {
          font-size: 1.5rem; /* Further adjust font size for very small screens */
        }
    }
.hero-section-sub-heading{
                          font-size: 2.8125rem;  /*   45px      */
                          line-height: 2.8125rem;  /*    45px     */
                          }
.hero-section-discription{
                           margin-top: 1rem;
                           width:70%;
                           font-weight: 500 ;
                           
                         }
 @media (max-width: 768px) {
                            .hero-section-discription {
                                font-size: 1rem; /* Adjust font size for smaller screens */
                            }
                        }
                        
                        /* Media query for even smaller viewports */
@media (max-width: 576px) {
                            .hero-section-discription {
                                font-size: 0.875rem; /* Further adjust font size for very small screens */
                            }
                        }
/*---------faded text------------------------*/  
.faded-text {
    display: flex;
    flex-shrink: 4;
    user-select: none;
    color: rgb(231, 231, 231);  
    transition: all 3s;
    font-weight: 580;
   padding-bottom: 0;
   padding-top: 1.1rem;
   font-size:6.2rem ;
}
/*---------faded text------------------------*/  

.hero-section-right{  
                     display: flex;
                     flex-shrink: 3;
                    width:17.5rem;      /*   280px      */
                    height:23.75rem;         /*    380px     */
                     background-image: url("Aman RAj (2).jpg");
                     background-position: center;
                     background-repeat: no-repeat;
                     background-size: cover;
                     display: grid;
                     color: aqua;
                     grid-template-rows: repeat(3,1fr);
                     grid-template-columns:repeat(3,1fr) ;
                     grid-template-areas:
                                         "header1 . header2"
                                            ". . ."
                                        "footer1 . footer2";
                    border-radius: 0.3125rem;  /*     5px     */
                    padding: -2.5rem;
                    filter: grayscale(1);
                    transition: all 1s;
                    animation:scaleImage 9s linear infinite;
                    
                    
                                         }
 @keyframes scaleImage{
    0%{
        transform:scale(1);
        filter:grayscale(1);
        
    }

    50%{
        transform:scale(1.1);
        filter:grayscale(0);
        box-shadow: 0px 0px 2.5rem #1f1f1f; /*   40px      */
    }
    100%{
        transform:scale(1);
        filter:grayscale(1); 
        box-shadow:0.25rem 0.25rem 0.625rem  black;  /*     4px 4px 10px    */
    }

 }
.icon{
         width:3.375rem;  /*  54px  */
         height:3.75rem;   /*  60px  */
       
}
.icon11{ grid-area:header1;}
.icon12{ grid-area:header2;}
.icon13{ grid-area:footer1;}
.icon14{ grid-area:footer2;font-weight: 900;}

.icon11 { 
    grid-area: header1;
    justify-self: start; 
    align-self: start; 
}

.icon12 { 
    grid-area: header2;
    justify-self: end; 
    align-self: start; 
}

.icon13 { 
    grid-area: footer1;
    justify-self: start; 
    align-self: end; 
}

.icon14 { 
    grid-area: footer2;
    justify-self: end; 
    align-self: end; 
}
@keyframes moveIconUp {
    0% {
        transform: translateY(0);
    }
    50% {
        transform: translateY(1.875rem);  /*   30px */
    }
    100% {
        transform: translateY(0);
    }
}

@keyframes moveIconDown {
    0% {
        transform: translateY(0);
    }
    50% {
        transform: translateY(1.875rem);   /* 30px   */
    }
    100% {
        transform: translateY(0);
    }
}

.icon14, .icon11 {
    animation: moveIconUp 4s infinite;
}

.icon13, .icon12 {
    animation: moveIconDown 3s infinite; 
}


.icon13 {
    animation-delay: 1.5s; 
}

.icon12 {
    animation-delay: 1.5s; 
}
/*--------------------------------------project section-------------------------------------------------------------------------------*/  
.project-section{
                  background-color: rgb(231, 231, 231);
                  height:auto;
                  width: 100vw;
                   overflow-x: hidden;
                   overflow-y: hidden;
                  margin:auto 0; 
}
.page-header{
           color:var(--bg0range);
           font-size: 5.625rem;     /*   90px */
           text-align: center;
           padding-top:1.875rem;     /* 30px   */
           color:brown;
}
.project-conatiner{
               max-width:1000px;
               margin:0 auto;
               padding:3rem 0;
               display: flex;
               flex-direction: column;
               gap:5.625rem;      /* 90px   */
}
.project-card {
                width:80%; 
                height:25rem;    /*   400px */
                /* background-image: url("html/carfinal.jpeg"); */
                background-size: cover;
                background-position: center;
                background-repeat: no-repeat;
                position: relative;
                box-shadow: 0px 0px 2.5rem #1f1f1f;  /* 40px   */
                color:white;  
               
                       
}
.project-card::after{
                      content:" ";
                      position: absolute;
                      top:0;
                      left:0;
                      right:0;
                      bottom:0;
                      background-color: #1f1f1f9a;
                      z-index: 0;
                     
}
.project-card::before{
    content:" ";
    position: absolute;
    top:0;
    left:0;
    right:0;
    bottom:0;
    background: linear-gradient(45deg,#343d68,#343d68be,#343d687c);
    transform: scaleX(0);
    transform-origin: left;
    transition:all 0.4s;
    z-index: 1;

}
.project-card:hover::before{
           transform:scaleX(1);
}
.project-number{
    position:absolute;
    font-size:12.5rem;    /* 200px   */
    font-weight: 600;
    color:white;
    z-index:10;
    display: none;

}
.project-card:hover .project-number{
                   display:block;
                   transition:block 4s;
                   
}
.project-number-right{
                      right:-2.5rem;  /*  40px  */
                      top:-2.8125rem;   /*    */
                     }
.project-number-left{
                        left:-1.875rem;  /*   30px */
                        top:-2.8125rem;  /* 45px   */
                       }
.project-content{
         position: absolute; 
         display: flex;  
         flex-direction: column;    
         color: white;
        padding:2rem;
        bottom:-20%;
        z-index:5;
        gap:1rem;
        transition:all 0.4s;
}
.project-content-left{ 
                        top:20%;
                       left:24%;

}
.project-content-right{
    top:20%;
    right:1%;
    
}
.project-skills-container{
    width:49%;
    display: flex;
    gap:0.5rem;            
    flex-wrap: wrap;
}
.project-skills{
    width:2.1875rem;   
}
.btn-group{
              display: flex;
              flex-direction: row;
              justify-content: flex-start;
              align-items:center;
              gap:0.9rem;             
}
.github-icon{
    width:1.5625rem;   
    color: azure;
}
.github-icon:hover{
    background-color: brown;
    color:brown;
}
.link-icon{
    width:0.625rem;   
    color: azure;
}
.project-headings{
    font-size:3.125rem;   
    font-weight: bold;
    line-height:3rem ;
}
.project-sub-heading{
           width:100%;
           font-size: 1rem;   
           font-style: italic;
}
.icon-lower{
           cursor: pointer;
           color:white;
           font-size:2.0625rem; 
}
.icon-lower:hover{
    color:brown;
}
.project-card:hover .project-content{
    transform: scale(1.1); 
}
#project-1{
    margin-left:7.5rem;    
    background-image: url(Scrolling-display-system.jpg);
}
#project-2{
   
    background-image: url(Amazonclone.png);
}
#project-3{
    margin-left:7.5rem;   
    background-image: url(smartcooler.jpg);
}
#project-4{
  
    background-image: url(allinonesystem.jpg);
}
@media(max-width:62.5rem) 
{
    .page-header{
        padding-top: 1.875rem;    
        color:var(--bg0range);
        text-align: center;
        font-size: 2.5rem;    
    }
.project-conatiner{
    padding:0.3125rem;  
    margin:0.625rem;   
    gap:3.75rem;     
}
.project-card{
    width:100%;
    height:18.75rem;   /* 300px    */
}
.project-card{
    background-size: cover;
    background-position: center;
}
.project-content{
    scale:0.5;
    bottom:0;
    left:0;
    right:0;
    top:0;
}
.project-content-left{
    left:0;
}
.project-headings{
    font-size:2.5rem;  /*   40px  */
    width:100%;
}
.project-sub-heading{
    width:100%;
}
#project-2{
    margin-left: 0;
}
#project-4{
    margin-left:0;
}
.project-skills-container{
    width:100%;
}
.project-skills{
    width:2.1875rem;    /*   35px  */
}
.project-card:hover .project-number{
    display: none;
}
.project-card:hover .project-content{
    scale:0.55;
}

}

.skillsection-2{
         width:100%;
         height: 120vh;
         background-color: white;
         display: flex;
      
         flex-direction:column;
     
        
}
.innersection {
    width: 79%;
    height: 85%;
    
    margin: auto; 
    display: flex; 
    flex-direction:row;
    align-items: center; 
}

.inner-section-left {
    width: 60%;
    height: 100%;
    padding-top: 1.4rem;
    
    box-sizing: border-box; 
}
.inner-section-right {
   
   
    width: calc(50% - 4px); 
    height: 98%;
    box-sizing: border-box; 
}
.inner--right-section{
    display: flex;
    padding-left: 13%;
    align-items: center;
    width:100%;
    height:100%;
   
    
}
.icons-container{
    width:100%;
    margin-top: 4.9rem;
    height:80%;
    display:grid;
    grid-template-columns: repeat(5,1fr);
    grid-template-rows: repeat(4,1.6fr);
    align-items: center;
    justify-content:center;
    text-align: center;
    z-index: 1;
    grid-template-areas: 
    "1st 2nd 3rd 4th 5th"
    "  6th 7th 8th 9th  10th"
    "  11th 12th 13th 14th 15th"
    " 16th 17th 18th 19th 20th"
    ;  
    
    
}
#icons--1{ grid-area: 1st;
   
}
#icons--2{ grid-area: 2nd;
}
#icons--3{ grid-area: 3rd;
}
#icons--4{ grid-area: 4th;
}
#icons--5{ grid-area: 5th;
}
#icons--6{ grid-area: 6th;
}
#icons--7{ grid-area: 7th;
}
#icons--8{ grid-area: 8th;
}
#icons--9{ grid-area: 9th;
}
#icons--10{ grid-area: 10th;
}
#icons--11{ grid-area: 11th;
}
#icons--12{ grid-area: 12th;
}
#icons--13{ grid-area: 13th;
}
#icons--14{ grid-area: 14th;
}
#icons--15{ grid-area: 15th;
}
#icons--16{ grid-area: 16th;
}
#icons--17{ grid-area: 17th;
}
#icons--18{ grid-area: 18th;
}
#icons--19{ grid-area: 19th;
}
#icons--20{ grid-area: 20th;
}
.faded-text-2nd{
                 
                 user-select: none;
                 color:rgba(231,231,231);
                 align-self: flex-end;
                 justify-self: flex-end;
                 flex-shrink: 4;
                 text-align: end;
                 font-size:5.2rem;
                 margin-right: 3rem;
                 display: flex;
              
                 max-height:75px ;
                 font-weight: 600;
                 
}

.inner-section-subheading{
       font-size: 5.2rem;
       font-weight: 800;
}
.inner-section-left-heading{
    padding-top:3.9rem;
    color:brown;
    font-size: 3.5rem;
    font-weight: 400;
    line-height: 3.125rem; 
}
.inner-section-left-discription{
    font-size: 1rem;
    color:var(--bg0range);
    margin-top: 2rem;
    text-align: justify;
    overflow-y: hidden;
    
}


.footer {
    position: relative;
    margin-top: -1px;
    background-color: #343d68;
    padding: 5rem;
}

.footer-wrapper {
    display: flex;
    gap: 1rem;
    padding: 1.2rem;
    justify-content: space-between;
    align-items: center;
    background-color: #535c87;
}

.footer-fadded-text {
    position: absolute;
    left: 0;
    bottom: 0;
    user-select: none;
    font-size: 5em;
}

.link-wrapper {
    display: flex;
    gap: 1.2rem;
    flex-direction: row;
}

.link-wrapper div a {
    color: white;
}

.icon-wrapper {
    display: flex;
    flex-direction: row;
    align-items: center; 
}

.social-media-icons {
    width: 4rem;
}


@media only screen and (max-width: 768px) {
    .footer {
        padding: 3rem;  
    }

    .footer-fadded-text {
        font-size: 3em; 
    }

    .link-wrapper div a {
        font-size: 0.8em; 
    }

    .social-media-icons {
        width: 3rem; 
    }
}


@media only screen and (max-width: 480px) {
    .footer {
        padding: 2rem; 
    }

    .footer-fadded-text {
        font-size: 2em; 
    }

    .link-wrapper div a {
        font-size: 0.7em; 
    }

    .social-media-icons {
        width: 2.5rem; 
    }
}

.inner--right{
    width:6rem;
}
.bobble-animation{
    position: absolute;
    z-index: -3;
    width:20rem;
    padding-left: 4rem;
    padding-bottom: 2rem;
    filter: grayscale(100%);
    animation: moveDiagonally 9s alternate infinite;
}
@keyframes moveDiagonally {
    0% {
      transform: translate(0, 0);
    }
    100% {
      transform: translate(100px, 100px); 
    }
  }
  .inner--right:hover{
    transform: scale(1.1);
    transition: transform 0.1s;
  }
  
  .contactus-from-container{
    width:100%;
    background-color: rgb(231,231,231);
  }
#submit-btn{
    gap:0.8rem; 
}
 .contactus-heading{
    font-size:4rem ;   
    color:brown;
    padding-top: 3rem;   
    padding-left: 11rem;   

 }
 .contact-us-subheading{
         font-size: 2rem;   
         color:#343d68;
         text-transform: capitalize;
         padding-left: 11rem;
 }
.contactus-form-container{
      display: flex;
      align-items: center;
      justify-content: center;
}
.contact-form{
      display: flex;
      flex-direction: column;
      
      width:60%;           
      margin:1.3rem 5rem;  


}
.formfield-container{
     width:100%;           
}
.formfield{
            width:100%;
            height: 32px;        
            padding:0 2rem;
            font-size: 18px;    
            border-radius: 5px;
            box-shadow:2px 2px 10px #1f1f1f ;
            font-weight: 500;
            border: none;
            margin-top:13px;     
}
.form-field-textarea{
    height:auto;
    padding-top: 0.7rem;   
}
#submit-btn{
    border:none;
    font-size: 1.2rem;    
    margin:1rem 0;
    margin-top: 1.7rem;   
}
#submit-btn:hover{
    scale:0.9 ;

}
.fa-solid{
         padding:0.1rem;
         font-size: 1.3rem;   
}


.containeeer{
    position:relative;
    width:100%;
    display: flex;
    justify-content: center;
    align-items: center;
    height:7rem;
   
    background-color:#343d68 ;
}
.footer-wrapper11{
    width: 65%;
    height: 30%;
  
     display:flex;
    justify-content:space-between;
    align-items: center;
    margin-top: 0.2rem;  
    
}

.link-wrapper{
   
    display: flex;
    gap: 1rem;
     flex-direction:row; 
}
.link-wrapper div a{
     color:white;
     text-decoration: none;
     transition: all 0.5s;
     
}
.link-wrapper div a:hover {
      color:brown;
}
.icon-wrapper{
    
    display: flex;
    flex-direction: row;
     gap:0.5rem;
    justify-content: center;
}
.social-media-icons{
    font-size: 2rem;
    color: white;
}
.social-media-icons :hover{
    color: brown;
    transition:all 0.5s ;
}
    </style>
    
</head>
<body>
        <div class="wrapper">

            <div class="container">

                   <div class="navbar">

                        <div class="logoconatiner">
                            <img src="icons8-aAAA-80.png"alt="Image not Found"class="logo">
                             <div class="logo-text">man Raj</div>
                            
                        </div>

                        <div class="nav-items">
                             <div > <a href="#projects">Projects</a> </div>
                             <div > <a href="#Skills">Skills</a> </div>
                             <div > <a href="#Contactme">Contact Me</a> </div>

                        </div>
                   </div>

                <div class="hero-section">
                    
                    <div class="hero-section-left">

                        <div class="herosection-heading">Hii! Aman Raj</div> 
                        <div class="hero-section-sub-heading"> I am a <span class="role"></span></div>
                        <div class="hero-section-discription"> I am a Frontend Developer and Here is my Portfollio Website
                            . Here you will learn about my joureny as a Frontend Developer.
                        </div>

                         <div class="p-button">
                             Hire Me
                         </div>
                         <div class="faded-text">AMAN RAJ</div>
                    </div>
          
                 <div class="hero-section-right">
                     

                    <div class="icon11">
                        <img src="6 dots image.svg"alt="image not found"class="icon">
                     </div>
                     <div class="icon12">
                        <img src="cubeimage-removebg-preview.png"alt="image not found"class="icon">
                    </div>
                    <div class="icon13" >
                        <img src="cubeimage-removebg-preview.png"alt="image not found"class="icon">
                     </div>
                     <div class="icon14">
                        <img src="6 dots image.svg"alt="image not found"class="icon">
                     </div>
                    
                   
               </div>

          </div>


    <div class="project-section"id="projects">
           
            <h2 class="page-header">
               Projects
           </h2>
            
           <div class="project-conatiner">
                  
                 <div class="project-card"id="project-1">
                      <div class="project-number project-number-left">
                          01
                      </div>
                      <div class="project-content project-content-left">
                          <div class="project-skills-container">
                          
                            <img class="project-skills" src="icons8-css-64.png"alt="image missing";>
                            <img class="project-skills" src="icons8-automation-50.png"alt="image missing";>
                            <img class="project-skills" src="icons8-ms-word-48.png"alt="image missing";>
                            <img class="project-skills" src="icons8-excel-48.png"alt="image missing";>
                            <img class="project-skills" src="html-icon.png"alt="image missing";>  
                            <img class="project-skills" src="icons8-powerpoint-48.png"alt="image missing";>
                            <img class="project-skills" src="icons8-electronics-64.png"alt="image missing";>
                            <img class="project-skills" src="icons8-java-script-188.png"alt="image missing";>
                            <img class="project-skills" src="icons8-arduino-48.png"alt="image missing";>
                            <img class="project-skills" src="icons8-nodejs-48.png"alt="image missing";>
                                                        
                          </div>
                            <h2 class="project-headings">
                                 
                                  Pixel Advertise
                            </h2>
                                   <div class="project-sub-heading">
                                    This system comprises a six-by-four-foot board equipped
                                     with 3456 pixel LEDs, managed by T8000 and T1000 controllers.      
                                  </div>
                                     <div class="btn-group">
                                              <div class="p-button">
                                                    Know More
                                               </div>
                                                 <div class="github-icon icon-lower">
                                                       <img src="icons8-github-64.png"alt="image-not-loaded">
                                                 </div>
                                                 <div class="link-icon icon-lower">
                                                    <img src="icons8-link-50.png"alt="image-not-loaded">
                                                 </div>

                                     </div>
                                  
                                        </div>
                            </div>
                  
              <div class="project-card"id="project-2">
                <div class="project-number project-number-right">
                    02
                </div>
                <div class="project-content project-content-right">
                    <div class="project-skills-container">
                      <img class="project-skills" src="icons8-css-64.png"alt="image missing";>
                      <img class="project-skills" src="icons8-automation-50.png"alt="image missing";>
                      <img class="project-skills" src="icons8-ms-word-48.png"alt="image missing";>
                      <img class="project-skills" src="icons8-excel-48.png"alt="image missing";>
                      <img class="project-skills" src="html-icon.png"alt="image missing";>  
                      <img class="project-skills" src="icons8-powerpoint-48.png"alt="image missing";>
                      <img class="project-skills" src="icons8-electronics-64.png"alt="image missing";>
                      <img class="project-skills" src="icons8-java-script-188.png"alt="image missing";>
                      <img class="project-skills" src="icons8-arduino-48.png"alt="image missing";>
                      <img class="project-skills" src="icons8-nodejs-48.png"alt="image missing";>
                                                  
                    </div>
                      <h2 class="project-headings">
                            Amazon-clone-Frontend
                      </h2>
                             <div class="project-sub-heading">
                             An incredible journey diving deep into the intricacies of frontend technologies like HTML and CSS     
                            </div>
                               <div class="btn-group">
                                        <div class="p-button">
                                              Know More
                                         </div>
                                           <div class="github-icon icon-lower">
                                                 <img src="icons8-github-64.png"alt="image-not-loaded">
                                           </div>
                                           <div class="link-icon icon-lower">
                                              <img src="icons8-link-50.png"alt="image-not-loaded">
                                           </div>

                               </div>
                            
                                  </div>
                      </div>
                       
                
                <div class="project-card"id="project-3">
                    <div class="project-number project-number-left">
                        03
                    </div>
                    <div class="project-content  project-content-left">
                        <div class="project-skills-container">
                          <img class="project-skills" src="icons8-css-64.png"alt="image missing";>
                          <img class="project-skills" src="icons8-automation-50.png"alt="image missing";>
                          <img class="project-skills" src="icons8-ms-word-48.png"alt="image missing";>
                          <img class="project-skills" src="icons8-excel-48.png"alt="image missing";>
                          <img class="project-skills" src="html-icon.png"alt="image missing";>  
                          <img class="project-skills" src="icons8-powerpoint-48.png"alt="image missing";>
                          <img class="project-skills" src="icons8-electronics-64.png"alt="image missing";>
                          <img class="project-skills" src="icons8-java-script-188.png"alt="image missing";>
                          <img class="project-skills" src="icons8-arduino-48.png"alt="image missing";>
                          <img class="project-skills" src="icons8-nodejs-48.png"alt="image missing";>
                                                      
                        </div>
                          <h2 class="project-headings">
                            Touchless Cooling 
                          </h2>
                                 <div class="project-sub-heading">
                                  Enhancing safety by preventing electric shock
                                   incidents and providing a cooler accessible to 
                                   individuals with disabilities who lack hands.
                                </div>
                                   <div class="btn-group">
                                            <div class="p-button">
                                                  Know More
                                             </div>
                                               <div class="github-icon icon-lower">
                                                     <img src="icons8-github-64.png"alt="image-not-loaded">
                                               </div>
                                               <div class="link-icon icon-lower">
                                                  <img src="icons8-link-50.png"alt="image-not-loaded">
                                               </div>

                                   </div>
                                
                                      </div>
                          </div>
            
              

                    <div class="project-card"id="project-4">
                            <div class="project-number project-number-right">
                                04
                            </div>
                            <div class="project-content project-content-right">
                                <div class="project-skills-container">
                                  <img class="project-skills" src="icons8-css-64.png"alt="image missing";>
                                  <img class="project-skills" src="icons8-automation-50.png"alt="image missing";>
                                  <img class="project-skills" src="icons8-ms-word-48.png"alt="image missing";>
                                  <img class="project-skills" src="icons8-excel-48.png"alt="image missing";>
                                  <img class="project-skills" src="html-icon.png"alt="image missing";>  
                                  <img class="project-skills" src="icons8-powerpoint-48.png"alt="image missing";>
                                  <img class="project-skills" src="icons8-electronics-64.png"alt="image missing";>
                                  <img class="project-skills" src="icons8-java-script-188.png"alt="image missing";>
                                  <img class="project-skills" src="icons8-arduino-48.png"alt="image missing";>
                                  <img class="project-skills" src="icons8-nodejs-48.png"alt="image missing";>
                                                              
                                </div>
                                  <h2 class="project-headings">
                                       
                                         Omni-Power Solution
                                  </h2>
                                         <div class="project-sub-heading">
                                          Streamlining power management by consolidating various bulky, basic power 
                                          supply devices into single unit.

                                          </div>
                                           <div class="btn-group">
                                                    <div class="p-button">
                                                          Know More
                                                     </div>
        
                                                                 <div class="github-icon icon-lower">
                                                                        <img src="icons8-github-64.png"alt="image-not-loaded">
                                                                 </div>
                                                                <div class="link-icon  icon-lower">
                                                                        <img src="icons8-link-50.png"alt="image-not-loaded"class="lastone">
                                                                </div>
                                       
                                              </div>

                                   </div>
               
           </div>

    </div>
            </div>



        <div class="skillsection-2" id="Skills">
                 
               <div class="innersection">
                         <div class="inner-section-left"> 
                                 <div class="inner-section-left-heading">
                                      <span class="inner-section-subheading">
                                        Me
                                      </span>           
                                   and <br>My Tech stack
                                
                                 </div>
                                 <div class="inner-section-left-discription">
                                 <p>
                                  Hi Everyone , My name is Aman Raj  I am a  Frontend Developer 
                                   || Innovating & Leveraging electronics 
                                   and automation expertise Applications
                                  </p>
                                  <br>
                                   <p>
                                   || MINOR CS'26 || AIR-5 SET SLIET
                                    || Goldmedlist E.C DIPLOMA G.P.M || Carpediem! ||BE ECE'26 ||
                                    Believe - Plan - Execute It is always now or never Start doing things before 
                                    anyone thinks of doing it.
                                    </p>
                                    <br>
                                    <p>
                                    My commitment to staying abreast of industry trends positions me as a forward-thinking
                                     professional ready to contribute to innovative projects. Excited to merge 
                                     computational expertise with AI advancements,
                                    </p> 
                                    <br>
                                    <p>
                                    I am poised to make meaningful contributions in the ever-evolving intersection 
                                    of computer science and artificial intelligence. As a graduate in Electronics and Communication Engineering, I possess a strong foundation in designing, analyzing .
                                  </p>
                                  <br>

                                 
                                 </div>
                         </div>
                                    
                         <div class="inner--right-section">
                              <div class="icons-container">

                             <img src="bobbleanimation.png"alt="image not found" class="bobble-animation"  >
                                <img class="inner--right"id="icons--1" src="icons8-video-trimming-48.png"alt="image missing";>
                                <img class="inner--right"id="icons--2"  src="icons8-automation-50.png"alt="image missing";>
                                <img class="inner--right" id="icons--3" src="icons8-ms-word-48.png"alt="image missing";>
                                <img class="inner--right" id="icons--4" src="icons8-excel-48.png"alt="image missing";>
                                <img class="inner--right"id="icons--5" src="icons8-butterfly-48.png"alt="image missing";>  
                                <img class="inner--right" id="icons--6"src="icons8-designer-48.png"alt="image missing";>  
                                <img class="inner--right" id="icons--7"src="icons8-canva-48.png"alt="image missing";>  
                                <img class="inner--right" id="icons--8" src="icons8-filmora-48.png"alt="image missing";>  
                                <img class="inner--right"id="icons--9"  src="icons8-idea-48.png"alt="image missing";>  

                                <img class="inner--right"id="icons--10" src="icons8-css-64.png"alt="image missing";>
                                <img class="inner--right"id="icons--11"  src="icons8-automation-50.png"alt="image missing";>
                                <img class="inner--right" id="icons--12" src="icons8-ms-word-48.png"alt="image missing";>
                                <img class="inner--right" id="icons--13" src="icons8-excel-48.png"alt="image missing";>
                                <img class="inner--right"id="icons--14" src="icons8-toolbox-48.png"alt="image missing";>  
                                <img class="inner--right" id="icons--15"src="icons8-idea-48.png"alt="image missing";>  
                                <img class="inner--right" id="icons--16"src="icons8-game-controller-48.png"alt="image missing";>  
                                <img class="inner--right" id="icons--17" src="icons8-youtuber-48.png"alt="image missing";>  
                                <img class="inner--right"id="icons--18"  src="icons8-drone-48.png"alt="image missing";> 
                                <img class="inner--right" id="icons--19" src="icons8-open-document-48.png"alt="image missing";>  
                                <img class="inner--right"id="icons--20"  src="icons8-arduino-uno-board-50.png"alt="image missing";> 
                              </div>
                         </div>
               </div>
               <div class="faded-text-2nd">
                   Skills
               </div>
                
        </div>




      <div class="contactus-from-container" id="Contactme">
            <div class="contaiiner">
                 <h1 class="contactus-heading">
                   Contact me
                 </h1>
                  <h3 class="contact-us-subheading">
                     Questions,thoughts,or just want to say
                     hello?
                  </h3>
              
              <div class="contactus-form-container">
                <form class="contact-form">
                  <div class="formfield-container">
                      <input class="formfield" type="text" name="name" id="" placeholder="Enter Your Name">
                  </div>
              
                  <div class="formfield-container">
                      <input class="formfield" type="email" name="email" id="" placeholder="Enter Your Email address">
                  </div>
              
                  <div class="formfield-container">
                      <input class="formfield" type="text" name="subject" id="" placeholder="Enter Your Subject">
                  </div>
              
                  <div class="formfield-container">
                      <textarea class="formfield form-field-textarea" name="message" id="" rows="10" cols="30" placeholder="Enter Your Message"></textarea>
                  </div>
              
                  <div>
                      <button type="submit" class="p-button" id="submit-btn">
                         <div> Send Message </div> <div>  <i class="fa-solid fa-paper-plane"></i></div>
                      </button>
                  </div>
              </form>
              
              </div>
            </div>
      </div>



    <footer>
        <div class="containeeer">
                   <div class="footer-wrapper11">
                     
               <div class="link-wrapper">
                      <div>
                          <a href="#projects">Projects</a>
                      </div>
                       <div>
                           <a href="#skills">Skills</a>
                        </div>
                        <div>
                            <a href="#contactme">Contact Me</a>
                        </div>
                </div>

              <div class="icon-wrapper">
                
                        <div class="social-media-icons">
                            <i class="fa-brands fa-linkedin"></i>
                       </div>
                   <div class="social-media-icons">
                        <i class="fa-brands fa-github"></i>
                   </div>
                        <div class="social-media-icons">
                             <i class="fa-brands fa-twitter"></i>
                         </div>
                   <div class="social-media-icons">
                      <i class="fa-brands fa-square-instagram"></i>
                   </div>
                         <div class="social-media-icons">
                          <i class="fa-brands fa-facebook-messenger"></i>
                         </div>

             </div>

        </div>


    </footer>


        </div>

        <script src="https://cdn.jsdelivr.net/npm/typed.js@2.0.12"></script>
        <script src="https://kit.fontawesome.com/58a810656e.js" crossorigin="anonymous"></script>
        <script>
          var typeData = new Typed(".role", {
            strings: [
              "Frontend Developer",
              "Web Developer",
              "Electronics Engineer",
              "Fast Learner",
              "Coder"
            ],
            loop: true,
            typeSpeed: 100,
            backSpeed: 80,
            backDelay: 1000
          });
        </script>
        
              </script>


</body>
</html>
