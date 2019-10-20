
<!doctype html>
<html lang="en">
<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
    <!-- Page Title -->
    <title>Wexim</title>
    <!-- Favicon -->
    <style>
        section{height: 1000px; background: silver; border: solid 5px red;}
        section, .section-padding { position: relative; padding: 7.5rem 0; overflow: hidden;}
header {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    display: flex;
    justify-content: space-between;
    z-index: 99999;
    background: #000;
    padding: 30px;
    color: #fff;
}
    </style>
      
</head>
<body data-spy="scroll" data-target=".navbar" data-offset="90"> 
<body> 
<!--Header Start-->
<header class="header"> 
    <div class="logo">Logo</div>
 <!--Nav Links-->  
 <button onclick="mobileToggle()">Try it</button>
        <div id="nav-main">
                <a class="scroll" href="#home">Home</a>
                <a class="scroll" href="#about">About</a>
                <a class="scroll" href="#team">Team</a>
                <a class="scroll" href="#portfolio">Work</a>
                <a class="scroll" href="#price">Pricing</a>
                <a class="scroll" href="#blog">Blog</a>
                <a class="scroll" href="#contact">Contact</a>  
    </div>  
</header>
<!--Header end-->
<section id="home"><h1>home</h1></section>
<section id="about"><h1>about</h1></section>
<section id="team"><h1>team</h1></section>
<section id="portfolio"><h1>portfolio</h1></section>
<section id="Pricing"><h1>Pricing</h1></section>
<section id="Blog"><h1>Blog</h1></section>
<section id="home"><h1>home</h1></section>
<section id="contact"><h1>contact</h1></section>
 


<!-- Optional JavaScript -->
<script src="js/jquery-3.3.1.min.js"></script>
<script>
    jQuery(function ($) {
    "use strict"; 
    /* ===================================
            Scroll
    ====================================== */  
    $(window).on('scroll', function () {
        if ($(this).scrollTop() > 220) { // Set position from top to add class
            $('header').addClass('header-appear');
        }
        else {
            $('header').removeClass('header-appear');
        }
    });


    //scroll sections 
        $(".scroll").on("click", function (event) {
            event.preventDefault();
            $("html,body").animate({
                scrollTop: $(this.hash).offset().top - 60}, 1200);
        });   

        // mobileToggle
        $(document).ready(function(){
            $(".header button").click(function(){
              $("#nav-main").addClass("intro"); 
              $("#nav-main").removeClass("intro");
            });
          }); 
        
});

// mobileToggle
/*
function mobileToggle() {
    var element = document.getElementById("nav-main");
    element.classList.toggle("navstyle");
 }
 */

123456
</script>

</body>
</html>
