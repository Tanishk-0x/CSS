
-------------------------------------------------------------------------
-> {sabse jyada priority INLINE CSS ki hoti he }

// --------------------------------------------------------
# -------------------- SELECTORS----------------------------------
// --------------------------------------------------------


-> id selector = using #name (unique id)
-> class selector = using .name (can be use multiple classes)
-> element selector = using name jaise [body,h1]
-> universal selector = * { to access all the elements } 
-> grouping selector = #firstname , #secondname {}
-> nested selector = #name > h1 {color: blue ;} to name id me h1 ka color blur kr do .. 

!important = to use it any how 
color: blue !important ; 


// --------------------------------------------------------
 # -----------------SPECIFIC ORDER--------------------------------------
 ID > CLASS > ELEMENTS .. sabse jyada priority id ki hoti he 
// --------------------------------------------------------


// --------------------------------------------------------
# ------------------- COLORS ------------------------------- 
// --------------------------------------------------------

-> Color = color change krne ke liye 
-> BackGround Color = background color change krne ke liye 
-> #ffffff = hax code kehte he isko 

--------------------------------------------------------------------------------------------------------------------------------------------------
 # ------------- UNITS IN CSS -------------------------------------------
-------------------------------------------------------------------------

-> % (percent) = parent ka ___ % isko de dega 
-> vw (view-width) = screen ka width ka __ 
-> vh (view-height) =  screeb ka height lenga __ 
-> em () = relative unit he parent ka aur relative to parent hota he 
-> px (pixels) = absolute value he .. 
-> rem (root em) = relative to the root kaam krta he 


--------------------------------------------------------------------------------------------------------------------------------------------------
-----------------BOX MODEL-------------------------------------------
------------------------------------------------------------------------






// --------------------------------------------------------
# ------- media query --------------------------------
// --------------------------------------------------------

/*
    syntax --- 
    @media ( condition ) { ---- } 
    @media screen and ( condition ) { --- } 
    @media ( condition-1 ) and ( condition-2 ) { --- } 
    @media ( 400px <= width <= 600px ) { --- } 

   orientation : potrait ; 
   width : 200px ; 
   width <= 400px ; 
   max-width: 300px ; // upto 
   min-width: 200px ; // starting from 

    --------- screen - size ----------- : 
    small = 640px ; 
    medium = 768px ; 
    large = 1024px ; 
    x large = 1280px ; 
    2x large = 1536px ; 

*/

// --------------------------------------------------------
 #  CSS VARIABLES -------------------------------
// --------------------------------------------------------

    --myvariable : rgb(38, 255, 0) ; 

     // --- global declaration of variable --------------  
    
    :root{
    --myvariable : rgb(38, 255, 0) ; 
    }


// --------------------------------------------------------
  # PSEUDO CLASSES -------------------------------
// --------------------------------------------------------

-> pseudo class = it is used to define a special state of an element

// pseudo class : 

-> :hover = jab mouse hovered hoga 
-> :link = jab click nhi kra he 
-> visited = jab link per click kr diya he jab visit kr lenge 
-> active = jaise hi click kra 

-> FIRST CHILD = pehla child lake dedeta he (to select first child) 

-> Nth child = ( an+b ) , 
-> 2n = even positions 

-> pseudo element = the specific part ko slect krte he 
pseudo element :: 

-> ::first-letter = to access the first letter of the elements 
-> :: selection = jo select krte he usko bhi change kr sakte he 
-> ::first-line = to select the first line of the elements 
-> ::before = usse pehle ko select krne ke liye .. 
-> ::after = uske baad ko select krne ke liye .. 

*/



// --------------------------------------------------------
# ------- TRANSFORM IN CSS  --------------------------------
// --------------------------------------------------------

= kisi element pe 2D ya 3D transfromnmation apply krta he 

/* 

    Scale = kisi bhi particular div ko scale kr sakte he X ya Y direction me 
    scaleX() , scaleY() , scaleZ() 
    skew = used to tilt an element is X and Y axis 
    translate = previuos location ki reference me move krta he 
    rotate = rotate krne ke liye rotate(degree) ... 

*/


// --------------------------------------------------------
# ------- TRANSITION IN CSS  --------------------------------
// --------------------------------------------------------

= transition allows to change property values smoothly over a given duration

/*  

    transition = smoothly change ke liye use krte he 
    {transition : duration ; }  

    -> transition-duration = kitna time lagega transition me 
    -> transition-property = specify krte he ki konsi property ke andar transition krna he 
    -> transition-delay = kitna der baad transition start hogi 
    -> transition-timing-function = kis tarah se A point se B point pe jaa rhe ho . speed ky ahe aur konsa rasta chuna he 

    : ease-in = start slow 
    -> ease = slow start then fast then end slowly 
    -> linear = same speed from start to end 
    -> ease-out = slow end 
    -> ease-in-out = slow start and end 
    -> cubic-bezier(n,n,n,n) = let define your own values 

*/

// --------------------------------------------------------
# ------- Keyframe / Animation IN CSS  --------------------------------
// --------------------------------------------------------

/* // --------- applying animation to the elements ------------ */
    
  animation-name: circles;
    animation-duration: 3s;
    animation-delay: 2s;
    animation-iteration-count: 4;
    animation-direction: alternate;

  /* // --------- applying animation to the elements ------------ */



/*  
 -> animation-name : name to add animation into element 
 -> animation-duration : kitni der chalni chahiye 
 -> animation-delay : kitne dalay ke baad animation chalna chahiye
 -> animation-iteration-count : kitne baar animation chalegi 
 -> animation-direction : spacifies direction of the animation 
 -> animation-fill-Mode : ye batata he ki jab start ho rhi he to element kha par honi chahhiye aur end ho rhi he to element kha per hona chahiye 
*/ 


/* //----------- KEYFRAMES --------------------- */

@keyframes circles {
    
    0% {
        transform: translate(0 , 0);
    }

    25% {
        transform: translate(200px , 0);
    }

    50% {
        transform: translate(200px , 200px);
    }

    75% {
        transform: translate(0 , 200px);
    }

}

