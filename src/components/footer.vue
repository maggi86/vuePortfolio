<template>
<div id="space">
  <footer id="footer">
        <p>Copyright &copy; 2022 MEAGAN </p>
    </footer>
</div>
    
</template>

<style scoped>
:root {
    --color-primary: #ee2f5576;
    --color-white: #e8e6e3;
    --color-black: #030910;
    --color-dark: #551523;
    --color-gray: #9d879064;


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
#footer {
 background-color:var(--color-gray);
  width: 100%;
  height: 40px;
  padding: 10px ;
  display: flex;
  flex-direction: column;
  align-items: center;
  color: var(--color-dark);
  text-align: center;
  bottom: 0;
  position: fixed;
  z-index: 10;
}
</style>