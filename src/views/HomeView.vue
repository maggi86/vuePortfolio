<template>
    <div class="container vw-50">
        <aside class="container-aside">
            <div class="containerAside-header">
                <div class="asideHeader-userInformations">
                <img src="https://i.postimg.cc/sDjnJCtj/Meagan-2.jpg" class="asideHeader-imgUserImage">
                  <h3 class="asideHeader-lblUserName"><span>M</span>eagan <span>W</span>illiams</h3>
                    <div class="asideHeader-socialsBox">
                        <a href="#" class="asideHeader-btnSocial"><i class="bi-github"></i></a>
                        <a href="#" class="asideHeader-btnSocial"><i class="bi-linkedin"></i></a>
                    </div>
                </div>
            </div>
            <div class="containerAside-main">
                <div class="asideMain-menuItemsBox">
                    <!-- <div class="asideMain-menuItem">
                        <a href="home" class="mainMenu-btnMenuItem"><i class="bi-house"></i> <span
                        class="mainMenu-lblMenuItem">Home</span></a>
                    </div> -->
                    <div class="asideMain-menuItem">
                        <a href="about" class="mainMenu-btnMenuItem"><i class="bi-person"></i> <span
                        class="mainMenu-lblMenuItem">About</span></a>
                    </div>
                    <div class="asideMain-menuItem">
                        <a href="resume" class="mainMenu-btnMenuItem"><i class="bi bi-file"></i> <span
                        class="mainMenu-lblMenuItem">Resume</span></a>
                    </div>
                    <div class="asideMain-menuItem">
                        <a href="projects" class="mainMenu-btnMenuItem"><i class="bi bi-book"></i> <span
                        class="mainMenu-lblMenuItem">Projects</span></a>
                    </div>
                    <div class="asideMain-menuItem">
                        <a href="contact" class="mainMenu-btnMenuItem"><i class="bi bi-envelope"></i> <span
                        class="mainMenu-lblMenuItem">Contacts</span></a>
                    </div>
                    <div class="asideMain-menuItem">
                        <a href="testimonial" class="mainMenu-btnMenuItem"><i class="bi bi-chat-left-quote"></i> <span
                        class="mainMenu-lblMenuItem">Testimonial</span></a>
                    </div>
                </div>
            </div>
        </aside>
        <main class=" container-fluid" style="height: 100vh">
        <div id="landing">
            <div class="container-small">
                <p class="title">An Aspiring Web developer</p>
                <p class="words">Welcome to my portfolio. I enjoy creating and designing colourful, fun, simplistic websites with a touch of minimalism. 
                <br>I'm passionate about web development and I believe it's one of the most powerful resources to put yourself out there</p>
            </div>
        </div>
        </main>
    </div>
</template>

<style>
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
}

.container-fluid {
    width: 100%;
    height: 100%;
    background: url("https://i.postimg.cc/sDjnJCtj/Meagan-2.jpg") no-repeat;
    background-size: cover;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-end;
    right: 0;
    background-color: rgba(37, 37, 37, 0.253);
    position: absolute;
    z-index: 2;
}

.container-small{
    display: flex;
    flex-direction: column;
    width:400px;
    justify-content: center;
    right:20px;
    background-color: var(--color-dark);
    color: var(--color-black);
}

.container-small span{
    color: var(--color-primary);
}


.title{
    font-size: var(--font-md); 
    font-weight: var(--size-lg);
}

.words{
    font-size: var(--font-sm);
    font-weight: var(--size-lg);
}

.containerMain-lblName, .containerMain-lblAbility {
    font-size: var(--font-lg);
    color: var(--color-white);
    position: relative;
    z-index: 3;
    margin-left: 30vw;
}

.containerMain-lblAbility {
    font-family: var(--font-Poppins);
    font-size: var(--font-md);
    font-weight: 400;
}

.containerMain-lblAbility span {
    border-bottom: 3px solid var(--color-primary);
}

.containerMain-ShowMenu {
    display: none;
    position: fixed;
    top: 10px;
    right: 10px;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    z-index: 5;
    border: none;
    font-family: var(--font-OpenSans);
    font-size: var(--font-md);
    background-color: var(--color-primary);
    color: var(--color-white);
    cursor: pointer;
}

.container-aside, .asideHeader-userInformations {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 20px 0;    
}

.asideHeader-userInformations {
    padding: 0;
}


.containerAside-main, .asideMain-menuItemsBox {
    width: 100%;
    margin: 20px 0;
}

.asideMain-menuItem {
    margin: 15px 0;
}

.asideMain-menuItemsBox {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding-left: 30px;
}

.mainMenu-btnMenuItem {
    color: var(--color-gray);
    font-family: var(--font-OpenSans);
    font-size: var(--font-sm);
    font-weight: 400;
    transition: color .5s;
}

.mainMenu-btnMenuItem i {
    font-size: 24px;
}

.mainMenu-btnMenuItem:hover {
    color: var(--color-white);
}

.mainMenu-btnMenuItem:hover i {
    color: var(--color-primary);
}

.mainMenu-btnMenuItem:focus {
    color: var(--color-white);
}

.mainMenu-btnMenuItem:focus i {
    color: var(--color-primary);
}

.mainMenu-lblMenuItem {
    display: inline;
    margin-left: 5px;
}

.containerAside-footer {
    width: 100%;
    height: 100px;
    position: absolute;
    bottom: 0;
    left: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.asideFooter-lblInfo {
    font-size: 13px;
    color: var(--color-white);
    margin-top: 10px;
}

@media screen and (max-width: 1200px) {
    .container-aside {
        left: -500px;
    }
    
    .containerMain-ShowMenu {
        display: block;
    }

    .containerMain-lblName, .containerMain-lblAbility {
        margin-left: 10vw;
    }
}

@media screen and (max-width: 768px) {
    .containerMain-lblName{
        font-size: 28px;
    }
}
</style>