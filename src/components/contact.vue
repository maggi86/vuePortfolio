<template>
    <!-- <div id="form">
        <h2>Feel free to Contact me</h2>

        <form action="https://formspree.io/f/xayvrnkd" method="POST">
            <label>
                Name:
                <input type="name" name="name" placeholder="Enter your Name">
            </label>
            <label>
                Email Address:
                <input type="email" name="email" placeholder="name@number.com">
            </label>
            <label>
              Your Message:
              <textarea name="message" rows="3"></textarea>
            </label> -->
  <!-- your other form fields go here -->
            <!-- <button type="submit">Send</button>
        </form>
    </div> -->
    <section class="contact" id="contact">
        <div class="container">
            <div class="heading text-center">
                <h2>Contact
                    <span> Us </span></h2>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                    <br>incididunt ut labore et dolore magna aliqua.</p>
            </div>
            <div class="row">
                <div class="col-md-6">
                    <div class="title">
                        <h3>Contact detail</h3>
                        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor </p>
                    </div>
                    <div class="content">
                        <!-- Info-1 -->
                        <div class="info">
                            <i class="bi bi-telephone"></i>
                            <h4 class="d-inline-block">PHONE :
                                <br>
                                <span>+27 67 155 0947, +27 81 496 3622</span></h4>
                        </div>
                        <!-- Info-3 -->
                        <div class="info">
                            <i class="bi bi-geo-alt"></i>
                            <h4 class="d-inline-block">ADDRESS :<br>
                                <span></span></h4>
                        </div>
                        <!-- Info-2 -->
                        <div class="info">
                            <i class="bi bi-envelope"></i>
                            <h4 class="d-inline-block">EMAIL :
                                <br>
                                <span>meaganwilliams407@gmail.com</span></h4>
                        </div>

                    </div>
                </div>

                <div class="col-md-6">

                    <form action="https://formspree.io/f/xayvrnkd" method="POST">
                        <div class="row">
                            <div class="col-sm-5 mx-6">
                                <input type="text" class="form-control" placeholder="Name" name="fname" required>
                            </div>
                            <div class="col-sm-7">
                                <input type="email" class="form-control" placeholder="Email" name="email" required>
                                
                            </div>
                            <div class="col-sm-12">
                                <input type="text" class="form-control" placeholder="Subject" name="subject" required>
                            </div>
                            <div class="form-group">
                            <textarea class="form-control" rows="5" id="comment" placeholder="Message"></textarea>
                        </div>
                        </div>
                        <!-- <div class="form-group">
                            <textarea class="form-control" rows="5" id="comment" placeholder="Message"></textarea>
                        </div> -->
                        <button class="btn btn-block" type="submit">Send Now!</button>
                    </form>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
// import Foot from "@/components/footer.vue";

export default {
    data() {
        return {
            name: "",
            email: "",
        }     
    },

};
</script>

<style scoped>

.title{
    padding-top: 40px;
}
section{
    margin-right: 20px;
}
* {
    font-family: 'Raleway', sans-serif;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

:root {
    --color-primary: #ef1e48;
    --color-white: #e8e6e3;
    --color-black: #030910;
    --color-dark: #642330;
    --color-gray: #9d8790;


    --font-Poppins: 'Poppins', sans-serif;
    --font-Raleway: 'Raleway', sans-serif;
    --font-OpenSans: 'Open Sans', sans-serif;

    --font-lg: 64px;
    --font-md: 26px;
    --font-sm: 15px;
    --font-xs: 9px;

    --size-lg: 1280px;
    --size-md: 976px;
    --size-sm: 768px;
    --size-xs: 500px;
    --size-mi: 300px;
}
.contact {
    padding: 50px 0;
}

.contact .heading h2 {
    font-size: var(--font-md);
    font-weight: var(--size-sm);
    margin: 0;
    padding: 0;

}

.contact .heading h2 span {
    color: var(--color-primary)
}

.contact .heading p {
    font-size: var(--font-sm);
    font-weight: var(--size-xs);
    line-height: 1.7;
    color: var(--color-dark);
    margin: 20px 0 60px;
    padding: 0;
}

.contact .form-control {
    padding: 25px;
    font-size: var(--font-sm);
    margin-bottom: 10px;
    margin:10px;
    background: var(--color-white);
    border: 0;
    border-radius: 10px;
}

.contact button.btn {
    padding: 10px;
    border-radius: 10px;
    font-size: var(--font-sm);
    background: var(--color-gray);
    color: var(--color-white);
}

.contact .title h3 {
    font-size: var(--font-sm);
    font-weight: var(--size-md);
}

.contact .title p {
    font-size: var(--font-sm);
    font-weight: var(--size-xs);
    color: var(--color-gray);
    line-height: 1.6;
    margin: 0 0 40px;
}

.contact .content .info {
    margin-top: 30px;
}
.contact .content .info i {
    font-size: var(--font-md);
    padding: 0;
    margin: 0;
    color: var(--color-black);
    margin-right: 20px;
    text-align: center;
    width: 20px;
}
.contact .content .info h4 {
    font-size: var(--font-sm);
    line-height: 1.4;
}

.contact .content .info h4 span {
    font-size: var(--font-sm);
    font-weight: var(--size-mi);
    color: var(--color-gray);
}
.btn{
    margin-left:10px ;
}
</style>
