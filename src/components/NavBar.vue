<template>
<nav> <!--navabr-->
    <ul>
        <li><a href="#"> Home </a></li>
        <li><a href="#"> About </a></li>
        <li><a href="#"> Services </a></li>
        <li><a href="#"> Products  </a></li>
        <li><a href="#"> Contact </a></li>
    </ul>


    <!--TABLET & MOBILE DISPLAY!! -->
    
    <div @click="toggleCancel" ref='ham' id="hamburger">
        <span></span>
        <span></span>  
    </div>
    
    <a href="#">
        <i class="fa fa-shopping-cart" aria-hidden="true"></i>
    </a>
</nav>
</template>

<script>

export default {
    methods: {
        toggleCancel() {
            this.$refs.ham.classList.toggle('cancel')
        }
    }
}

</script>
