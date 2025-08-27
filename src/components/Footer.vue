<template>
    <div class="footer container mx-auto py-10 mt-30">
        <div class="grid grid-cols-1 lg:grid-cols-4 gap-4 text-center px-10">
            <div class="logo flex justify-center">
                <img src="@/assets/icons/footer-logo.png" alt="Logo" class="size-fit" />
            </div>
            <div class="menu">
                <h3 class="text-md text-orange-500 mb-10 uppercase">Menu</h3>
                <ul class="flex flex-col space-y-2 text-orange-950">
                    <li><a href="#">About</a></li>
                    <li><a href="#">Services</a></li>
                    <li><a href="#">Blog</a></li>
                    <li><a href="#">Contact</a></li>
                </ul>
            </div>
            <div class="services">
                <h3 class="text-md text-orange-500 mb-10 uppercase">services</h3>
                <ul class="flex flex-col space-y-2 text-orange-950">
                    <li><a href="#">Design</a></li>
                    <li><a href="#">Development</a></li>
                    <li><a href="#">Marketing</a></li>
                    <li><a href="#">See More</a></li>
                </ul>
            </div>
            <div class="social flex flex-row justify-center lg:justify-end lg:space-x-4">
                <img src="@/assets/icons/facebook.png" alt="facebook" class="size-10">
                <img src="@/assets/icons/twitter.png" alt="twitter" class="size-10 mx-2">
                <img src="@/assets/icons/instagram.png" alt="instagram" class="size-10">
            </div>
        </div>
    </div>
</template>