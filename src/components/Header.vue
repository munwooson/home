<template>
    
    <nav class="navbar">
    <div class="navbar__logo">
        <font-awesome-icon icon="house" />
        <a href="">Home</a>
    </div>

    <ul class="navbar__menu">
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Gallery</a></li>
        <li><a href="#">FAQ</a></li>
    </ul>

    <ul class="navbar__icons">
        <li><i class="fab fa-twitter"></i></li>
        <li><i class="fab fa-facebook-f"></i></li>
    </ul>
    </nav>
</template>
<script>
export default {
    name: 'HeaderComponent', 
    data() {
        return {

        }
    }
}
</script>
<style>
    body{
        margin: 0;
    }
    a{
        text-decoration: none;
        color: white;
    }
    .navbar{
        display: flex;
        justify-content: space-between;
        align-items: center;
        background-color: #263343;
        padding: 8px 12px;
    }
    .navbar__logo {
        font-size:24px;
        color: white;
        display: flex;
    }
    /* .navbar__logo i {
        color: #d49466
    } */
    .navbar__menu {
        display: flex;
        list-style: none;
        padding-left:0;
    }
    .navbar__menu li {
        padding: 8px 12px;
    }
    .navbar__icons {
        list-style: none;
        color: white;
        display: flexbox
    }
    .navbar__icons li {
        padding: 8px 12px;
    }
    .home_icon {
        background-image: url('../assets/home_app_logo.svg') ;
        background-repeat: no-repeat;
        background-position: center;
        background-size: contain;
        width: 1em;
        height: 1em;
        /* filter: blur(5px); */
          filter: invert(16%) sepia(89%) saturate(6054%) hue-rotate(358deg) brightness(97%) contrast(113%); 
        
         /* filter: invert(16%) sepia(89%) saturate(6054%) hue-rotate(358deg) brightness(97%) contrast(113%);  */
    }
     .menu_icon {
        background-image: url('../assets/menu_icon.svg') ;
        background-repeat: no-repeat;
        background-position: center;
        background-size: contain;
        width: 1em;
        height: 1em;
        /* filter: blur(5px); */
          filter: invert(16%) sepia(89%) saturate(6054%) hue-rotate(358deg) brightness(97%) contrast(113%); 
        
         /* filter: invert(16%) sepia(89%) saturate(6054%) hue-rotate(358deg) brightness(97%) contrast(113%);  */
    }
    
    @media screen and (max-width: 768px) {
        .navbar{
            flex-direction: column;
            align-items:flex-start;
        }
        .navbar__menu{
            flex-direction: column;
            align-items: center;
            width:100%
        }

        .navbar__menu li {
            width: 100%;
            text-align: center;
        }
        .navbar__icons{
            justify-content: center;
            width: 100%;
        }
    }
</style>