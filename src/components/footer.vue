<template>
    <div>
        <footer>
            <div id="footer">
                <marquee behavior="scroll" direction="left" style="margin-top: 5px;">
                    <h1>Tshimologo King Mabena</h1>
                </marquee>
                <div class="footer_bottom">
                    <router-link to="/">
                        <h2>Copyright 2022: Kingdom Network Official</h2>
                    </router-link>
                </div>
            </div>
        </footer>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
    .footer-menu{
        background-color: black;
    }

    a{
        padding: 10px;
        text-decoration: none;
    }
    #footer{
        background-color: black;
    }
    h1{
        font-size: 23px;
    }
    h2{
        font-size: 14px;
    }
</style>