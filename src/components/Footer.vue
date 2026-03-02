<script setup></script>

<template>
    <footer class=" bg-black text-white flex flex-col items-center py-16 space-y-12 text-center md:flex-row md:justify-between md:items-start md:px-4 lg:px-32">
        <!-- logo -->
        <div class="">
            <img src="../assets/logo.svg" alt="">
        </div>

        <!-- footer-links -->
        <div class=" space-y-12 md:flex md:flex-1 md:justify-between md:text-left md:px-8 lg:flex-0 lg:space-x-24">
            <div>
                <h3>Features</h3>
                <ul class=" space-y-2">
                    <li><a href="#">Link Shortening</a></li>
                    <li><a href="#">Branded Links</a></li>
                    <li><a href="#">Analytics</a></li>
                </ul>
            </div>

            <div>
                <h3>Resources</h3>
                <ul class=" space-y-2">
                    <li><a href="#">Blog</a></li>
                    <li><a href="#">Developers</a></li>
                    <li><a href="#">Support</a></li>
                </ul>
            </div>

            <div>
                <h3>Company</h3>
                <ul class=" space-y-2">
                    <li><a href="#">About</a></li>
                    <li><a href="#">Our Team</a></li>
                    <li><a href="#">Careers</a></li>
                    <li><a href="#">Contact</a></li>
                </ul>
            </div>
        </div>

        <!-- social -->
        <div class=" flex space-x-4">
            <a href="#"><img src="../assets/icon-facebook.svg" alt="Facebook"></a>
            <a href="#"><img src="../assets/icon-twitter.svg" alt="Twitter"></a>
            <a href="#"><img src="../assets/icon-pinterest.svg" alt="Pinterest"></a>
            <a href="#"><img src="../assets/icon-instagram.svg" alt="Instagram"></a>
        </div>
    </footer>
</template>

<style scoped>
h3{
    font-weight: bold   ;
    margin-bottom: 16px;
}
</style>