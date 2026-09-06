  /* ****************   Hero Section    **************** */

  
.hero {
    min-height: 100vh;
    position: relative;
    overflow: hidden;
    background: white;
}


.hero-image {
    position: absolute;
    top: 0;
    right: 0;
    width: 65%;
    height: 100%;
    background-image: url("/studyDashboard/images/white.png");
    background-size: cover;
    background-position: center;
}


.hero-content {
    position: relative;
    z-index: 2;
    width: 90%;
    max-width: 1200px;
    margin:0 auto;
    padding-top: 200px;

}



.hero-content h1 {
    max-width: 600px;
    font-size: 3rem;
}

.hero-content p {
    max-width: 500px;
    line-height: 1.6;
}


.hero-image::before {
    content: "";
    position: absolute;
    inset: 0;

    background: linear-gradient(
        to right,
        white 0%,
        white 15%,
        rgba(255, 255, 255, 0.8) 35%,
        rgba(255, 255, 255, 0.3) 55%,
        transparent 75%
    );
}



 
  
.hero-content span {
    font-family: monospace;
   display: inline-block;
    margin: 0;
    overflow: hidden;
    white-space: nowrap;
    border-right: 1px solid;
    width: 0;
    animation: typing 3s steps(30) forwards,
               blink 1s step-end infinite;

} 




@keyframes typing {
    from {
        width: 0%;

    }
    to {
        width: 32ch;
    }
}

@keyframes blink  {
    50% {
        border-color: transparent;
    }
}




  /* ****************   Hero Section  end  **************** */