<template>
    <div class="container">
        <aside class="container-aside">
            <div class="containerAside-header">
              <div class="asideHeader-userInformations">
                <img src="https://i.postimg.cc/sDjnJCtj/Meagan-2.jpg" class="asideHeader-imgUserImage">
                  <h3 class="asideHeader-lblUserName">Meagan Williams</h3>
                    <div class="asideHeader-socialsBox">
                        <a href="#" class="asideHeader-btnSocial"><i class="bi-github"></i></a>
                        <a href="#" class="asideHeader-btnSocial"><i class="bi-linkedin"></i></a>
                    </div>
                </div>
            </div>
            <div class="containerAside-main">
                <div class="asideMain-menuItemsBox">
                    <div class="asideMain-menuItem">
                        <a href="home" class="mainMenu-btnMenuItem"><i class="bi-house"></i> <span
                        class="mainMenu-lblMenuItem">Home</span></a>
                    </div>
                    <div class="asideMain-menuItem">
                        <a href="about" class="mainMenu-btnMenuItem"><i class="bi-person"></i> <span
                        class="mainMenu-lblMenuItem">About</span></a>
                    </div>
                    <div class="asideMain-menuItem">
                        <a href="resume" class="mainMenu-btnMenuItem"><i class="bi-file"></i> <span
                        class="mainMenu-lblMenuItem">Resume</span></a>
                    </div>
                    <div class="asideMain-menuItem">
                        <a href="projects" class="mainMenu-btnMenuItem"><i class="bi-book"></i> <span
                        class="mainMenu-lblMenuItem">Projects</span></a>
                    </div>
                    <div class="asideMain-menuItem">
                        <a href="contact" class="mainMenu-btnMenuItem"><i class="bi-envelope"></i> <span
                        class="mainMenu-lblMenuItem">Contacts</span></a>
                    </div>
                </div>
            </div>
        </aside>
        <main class="container-main">
            <div class="containerMain-backgroundFilter"></div>
            <h1 class="containerMain-lblName">Meagan Williams</h1>
            <p class="containerMain-lblAbility">I'm <span>Developer</span></p>
            <button onclick="ShowMenu()" class="containerMain-ShowMenu"><i class="bi-list"></i></button>
        </main>
    </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans&family=Poppins:wght@400;600&family=Raleway:wght@700&display=swap');
* {
    font-family: 'Raleway', sans-serif;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

:root {
    --color-primary: #1fb2ed;
    --color-white: #e8e6e3;
    --color-black: #030910;
    --color-dark: #1a1d27;
    --color-gray: #9d9487;


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

html, body {
    height: 100%;
}

a {
    text-decoration: none;
}

div.container {
    width: 100%;
    height: 100%;
}

.container-aside {
    width: 20%;
    max-width: 300px;
    min-width: 300px;
    height: 100%;
    position: fixed;
    left: 0;
    top: 0;
    z-index: 4;
    background-color: var(--color-black);
    transition: left 1s;
}

.showMenu {
    left: 0 !important;
}

.container-main {
    width: 100%;
    height: 100%;
    background: url("https://i.postimg.cc/N09qG5TF/images.jpg") no-repeat center;
    background-size: cover;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
}

.containerMain-backgroundFilter {
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.253);
    position: absolute;
    z-index: 2;
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

.asideHeader-imgUserImage {
    width: 120px;
    height: 120px;
    border-radius: 50%;
    border: 4px solid #000000;
    margin-bottom: 20px;
}

.asideHeader-lblUserName {
    font-family: var(--font-Poppins);
    font-size: var(--font-md);
    font-weight: 600;
    color: var(--color-white);
    margin-bottom: 20px;
}

.asideHeader-btnSocial {
    padding: 10px 12px;
    margin: 0 2px;
    border-radius: 50%;
    background-color: var(--color-dark);
    color: var(--color-white);
    font-size: var(--font-sm);
    transition: background-color .5s;
}

.asideHeader-btnSocial:hover {
    background-color: var(--color-primary);
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

.asideFooter-lblCopyRight, .asideFooter-lblInfo {
    font-family: var(--font-OpenSans);
    font-size: var(--font-sm);
    font-weight: 400;
    color: #accbef;
}

.asideFooter-lblInfo {
    font-size: 13px;
    color: var(--color-white);
    margin-top: 10px;
}

.asideFooter-lblInfo strong {
    color: #36b2ed;
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