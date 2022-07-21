<template>
    <section id="resume">
      
      <div class="timeline">
        <div class="mmm">
        <p class="lead text-center fw-bold"><span>R</span>ESUME</p>
      </div>
        <div class="box left">
          <div class="content">
            <h3>2022 - Current</h3>
            <small>
              Life Choices Academy of Coding.
            </small>
            <p>Where i started learning coding and Web Development.</p>
          </div>
        </div>
        <div class="box right">
          <div class="content">
            <h3>2017 - 2021</h3>
            <small>
              Oude Molen Academy of Science and technology.
            </small>
            <p>Studied at High School in Pinelands and passed with a Bachalor's pass</p>
          </div>
        </div>
        <div class="box left">
          <div class="content">
            <h3>2019-2021</h3>
            <small>
              Oude Molen Academy of Science and Technology.
            </small>
            <p>I studied Engineering Graphics and Design( EGD ) in High school.</p>
          </div>
        </div>
        <div class="box right">
          <div class="content">
            <h3>2019 - 2020</h3>
            <small>
              Oude Molen Academy of Science and Technology.
            </small>
            <p>I studied Mechanical Engineering for a year in High School.</p>
          </div>
        </div>
        <div class="box left">
          <div class="content">
            <h3>2020 - 2021</h3>
            <small>
              Oude Molen Academy of Science and Technology.
            </small>
            <p>I studied Automotive Engineering for two years in High School.</p>
          </div>
        </div>
        <div class="box right">
          <div class="content">
            <h3>2009 - 2016</h3>
            <small>
              Arcadia Primary School.
            </small>
            <p>I attended primary school in Bonteheuwel.</p>
          </div>
        </div>
      </div>
    </section>
</template>

<style scoped>

:root {
    --color-primary: #ef1e48;
    --color-white: #e8e6e3;
    --color-black: #000000;
    --color-dark: #642330;
    --color-gray: #c3c0c1;


    --font-Poppins: 'Poppins', sans-serif;
    --font-Raleway: 'Raleway', sans-serif;
    --font-OpenSans: 'Open Sans', sans-serif;

    --font-lg: 64px;
    --font-xm: 45px;
    --font-md: 26px;
    --font-sm: 15px;
    --font-xs: 9px;

    --size-lg: 1280px;
    --size-md: 976px;
    --size-sm: 768px;
    --size-xs: 500px;
}

#resume {
  scroll-margin: 100px;
  background-color: var(--color-white);
  padding:20px;
  display:flex;
  justify-content: right;
}
* {
  box-sizing: border-box;
  
}

.mmm p{
  font-size: var(--font-xm);
}
.mmm span{
  color: var(--color-primary);
  font-size: var(--font-lg);
}

div .timeline{
  width: 900px;
}


.timeline {
  position: relative;
  max-width: 1000px;
  margin: 0 auto;
}
/* The actual timeline (the vertical ruler) */
.timeline::after {
  content: '';
  position: absolute;
  width: 2px;
  background-color: var(--color-black);
  top: 0;
  bottom: 0;
  left: 50%;
  margin-left: 0px;
  margin-top: 100px
}
/* Container around content */
.box {
  padding: 10px 40px;
  position: relative;
  width: 50%;
}
/* The circles on the timeline */
.box::after {
  content: '';
   position: absolute; 
  width: 15px;
  height: 15px;
  right: -17px;
  background-color: var(--color-primary);
  border: 2px solid var(--color-dark);
  top: 15px;
  border-radius: 50%;
  z-index: 1;
}

p, small{
    color:var(--color-dark);
}

h2{
    color: var(--color-dark);
    font-size:var(--font-md);
}

/* h4{
    color:var(--color-primary);
    font-size: var(--font-lg);
} */

/* Place the container to the left */
.left {
  left: 0;
}
/* Place the container to the right */
.right {
  left: 50%;
}
/* Add arrows to the left container (pointing right) */
.left::before {
  content: " ";
  height: 0;
  position: absolute;
  top: 22px;
  width: 0;
  z-index: 1;
  right: 30px;
  border: medium solid var(--color-gray);
  border-width: 10px 0 10px 10px;
  border-color: transparent transparent transparent var(--color-gray);
}
/* Add arrows to the right container (pointing left) */
.right::before {
  content: " ";
  height: 0;
  position: absolute;
  top: 22px;
  width: 0;
  z-index: 1;
  left: 30px;
  border: medium solid var(--color-gray);
  border-width: 10px 10px 10px 0;
  border-color: transparent var(--color-gray) transparent transparent;
}
/* Fix the circle for containers on the right side */
.right::after {
  left: -16px;
}
/* The actual content */
.content {
  padding: 20px 30px;
  background-color: var(--color-gray);
  position: relative;
}
.content > h3 {
  color:var(--color-primary);
}
/* Mediaqueries - Responsive timeline on screens less than 600px wide */
@media screen and (max-width: 600px) {
  /* Place the timelime to the left */
  .timeline::after {
  left: 31px;
  }
  /* Full-width containers */
  .box {
  width: 100%;
  padding-left: 70px;
  padding-right: 25px;
  }
  /* Make sure that all arrows are pointing leftwards */
  .box::before {
  left: 60px;
  border: medium solid rgb(255, 255, 255);
  border-width: 10px 10px 10px 0;
  border-radius: 1px;
  border-color: transparent rgb(255, 255, 255) transparent transparent;
  }
  /* Make sure all circles are at the same spot */
  .left::after, .right::after {
  left: 15px;
  }
  /* Make all right containers behave like the left ones */
  .right {
  left: 0%;
  }
}
</style>