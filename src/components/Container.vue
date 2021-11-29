<template>
<div class="container-1">
    <div id="hero-product"> <!--left side of the main body consisting of the hero image and text-->
        <img src="./../assets/images/skate.png" id="skate-1" alt="" ref='heroImage'>
        <div id="hero-text">
            <p>Speedy</p>
            <p>Quads</p>
        </div>
    </div>

    <div id="product-details">
        <div id="title-header">
            <p class='title'>Lorem speedy quads
            </p>
            <div id="stars">
                <img class="star" src="./../assets/images/star-images-9441.png" alt="">
                <img class="star" src="./../assets/images/star-images-9441.png" alt="">
                <img class="star" src="./../assets/images/star-images-9441.png" alt="">
                <img class="star" src="./../assets/images/star-images-9441.png" alt="">
                <img class="star" src="./../assets/images/star-images-9441.png" alt="">
            </div>
        </div>

        <small>Stuff 800-595-00</small>
        
        <p id='stuff'>3 500 py6.</p>

        <p class="random-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam libero consequatur aliquid nesciunt ipsum, doloremque tempore nihil? Blanditiis, incidunt earum, autem porro laudantium quos enim harum excepturi aliquid laboriosam sint odio est, dicta dolores eligendi numquam ducimus molestiae? sit amet consectetur adipisicing elit. Dicta aut nam quidem!
            <a href="#" id='details'>Details</a>
        </p>

        <div class="colours-tab">
            <p>Colour:</p>
            <div class="colours">
                <div @click="changeColor1" ref="blue" id="light-blue"></div>
                <div @click="changeColor2" ref="pink" id="pink"></div>
                <div @click="changeColor3" ref="yellow" id="yellow"></div>
                <div @click="changeColor4" ref="grey" id="grey"></div>
            </div>
        </div>
        <div class="size">
            <label for="size">Size: </label>
            <select @change="scale" ref='select' name='size' id="">
                <option value="lg">Large</option>
                <option value="md" selected>Medium</option>
                <option value="sm">Small</option>
                <option value="mn">Mini</option>
            </select>
        </div>

        <button type="submit">Complete Order</button>
    </div>

</div>
</template>



<script>
let body = document.querySelector('body')

export default {
    methods: {
        changeColor1() {
            body.classList = '';

            document.querySelector('select').style.borderColor = 'rgba(255, 255, 255, 0.5)'   
            document.querySelector('button, select').style.color = 'rgba(255, 255, 255, 0.5)'
            document.querySelector('small').style.color = 'rgba(255, 255, 255, 0.5)'
            document.querySelector('button, #details').style.color = '#fff'

            for (const child of this.$refs.blue.parentElement.children) {
                child.style.transform = ''   
            }
            this.$refs.blue.style.transform = 'scale(1.3)'
                    
            console.log(this)
        },
        changeColor2() {
            body.classList = 'pink'

            document.querySelector('select').style.borderColor = 'rgba(255, 255, 255, 0.5)'   
            document.querySelector('button, select').style.color = 'rgba(255, 255, 255, 0.5)'
            document.querySelector('small').style.color = 'rgba(255, 255, 255, 0.5)'
            document.querySelector('button, #details').style.color = '#fff'

            for (const child of this.$refs.pink.parentElement.children) {
                child.style.transform = ''   
            }
            this.$refs.pink.style.transform = 'scale(1.3)'
                    
        },
        changeColor3() {
            body.classList = 'yellow';

            document.querySelector('select').style.borderColor = 'rgba(255, 255, 255, 0.5)'   
            document.querySelector('button, select').style.color = 'rgba(255, 255, 255, 0.5)'
            document.querySelector('small').style.color = 'rgba(255, 255, 255, 0.5)'
            
            document.querySelector('button, #details').style.color = '#fff'
        
            for (const child of this.$refs.yellow.parentElement.children) {
                child.style.transform = ''   
            }
            this.$refs.yellow.style.transform = 'scale(1.3)'
        },
        changeColor4() {
            body.classList= 'white'

            document.querySelector('select').style.borderColor = '#2c3e50'   
            document.querySelector('button, select').style.color = '#2c3e50'
            document.querySelector('small').style.color = '#2c3e50'
            document.querySelector('#details').style.color = '#2c3e50'
        
            for (const child of this.$refs.grey.parentElement.children) {
                child.style.transform = ''   
            }
            this.$refs.grey.style.transform = 'scale(1.3)'
        },

        scale() {
            if (this.$refs.select.value == 'lg') {
                this.$refs.heroImage.style.transform = 'scale(1.3)'
            }
            else if (this.$refs.select.value == 'md') {
                this.$refs.heroImage.style.transform = 'scale(1.0)'
            }
            else if (this.$refs.select.value == 'sm') {
                this.$refs.heroImage.style.transform = 'scale(0.8)' 
            }
            else if (this.$refs.select.value == 'mn') {
                this.$refs.heroImage.style.transform = 'scale(0.6)' 
            }
        }
    }
}
</script>