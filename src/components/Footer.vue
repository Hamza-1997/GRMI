<script setup>
// import Button from './Buttons/Button.vue'

</script>

<template>
    <!-- Remove the container if you want to extend the Footer to full width. -->
    <!-- <div class=""> -->

    <footer class="text-white text-center text-lg-start footer-container">
        <!-- Grid container -->
        <div class="container">
            <!--Grid row-->
            <div class="row mt-4">
                <!--Grid column-->
                <div class="col-lg-3 col-md-6 mb-4 mb-md-0">
                    <div>
                        <img src='../assets/icons/GRMI_logo.png' alt="Responsive image" width="183">
                    </div>
                    <div style="margin-top: 16px;display: inline-flex;">
                        <div style="margin-right: 16px;">
                            <img src='../assets/icons/Linkedin.png' alt="Responsive image">
                        </div>
                        <div>
                            <img src='../assets/icons/Twitter.png' alt="Responsive image">
                        </div>
                    </div>
                </div>
                <!--Grid column-->

                <!--Grid column-->
                <div class="col-lg-2 col-md-3 mb-4 mb-md-0">
                    <div class="d-flex flex-column" style="margin-right: 12px;">
                        <div class="M20 white" style="font-weight: 700;margin-bottom: 24px;">QUICKLINKS</div>
                        <span class="M16 white">
                            About GRMI
                        </span>
                        <span class="M16 white">
                            Team
                        </span>
                        <span class="M16 white">
                            News and Media
                        </span>
                        <span class="M16 white">
                            Projects
                        </span>
                        <span class="M16 white">
                            Portal
                        </span>
                        <span class="M16 white">
                            Events
                        </span>

                    </div>

                </div>

                <div class="col-lg-2 col-md-3 mb-4 mb-md-0">
                    <div class="d-flex flex-column" style="margin-right: 12px;">
                        <div class="M20 white" style="font-weight: 700;margin-bottom: 24px">CONTACT</div>
                        <span class="M16 white">hey@georiskmap.org</span>
                    </div>
                </div>
                <!--Grid column-->

                <!--Grid column-->
                <div class="col-lg-5 col-md-12 mb-4 mb-md-0 mt-md-4">
                    <section class="newsletter">
                        <div class="container">
                            <div class="row">
                                <div class="col-sm-12">
                                    <div class="content" style="text-align: left;">
                                        <div class="C49 white" style="margin-bottom: 24px;">Subscribe to our
                                            Newsletter
                                        </div>
                                        <div class="input-group">
                                            <input type="email" class="form-control" placeholder="Enter your email">
                                        </div>
                                        <span class="input-group-btn">
                                            <button class="btn" type="submit"><span class="M20"
                                                    style="color: #FCFCFC;">Subscribe</span></button>
                                        </span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </section>

                </div>
                <!--Grid column-->
            </div>
            <!--Grid row-->
            <div style="margin-top: 114px;">
                <div class="M13 white d-flex justify-content-center">
                    2023 georiskmap.org© ALL RIGHTS RESERVED
                    <!-- <a class="text-white" href="https://mdbootstrap.com/">MDBootstrap.com</a> -->
                </div>
                <div class="M10 white d-flex justify-content-center">
                    Website designed by Timi Salaam
                </div>
            </div>
        </div>
        <!-- Grid container -->

        <!-- Copyright -->

        <!-- Copyright -->
    </footer>

    <!-- </div> -->
    <!-- End of .container -->
</template>

<style scoped>
.footer-container {
    /* height: 506px; */
    background-color: #134A39;
    padding: 78px 0;
    /* padding: 78px 120px; */
    /* justify-content: space-between; */
    /* background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    position: relative; */
    /* margin-top: 65px; */
}

.newsletter {
    /* padding: 80px 0; */
    /* background: #19beda; */
}

.newsletter .content {
    max-width: 650px;
    margin: 0 auto;
    text-align: center;
    position: relative;
    z-index: 2;
}

.newsletter .content .form-control {
    height: 50px;
    border-color: #ffffff;
    border-radius: 6px;
}

.newsletter .content.form-control:focus {
    box-shadow: none;
    border: 2px solid #ffffff;
}

.newsletter .content .btn {
    min-height: 52px;
    border-radius: 6px;
    background: #1A1A1A;
    margin-top: 16px;
    /* color: #FCFCFC; */
    /* font-weight: 600; */
}

/* .hero-text {
    padding: 0 40px 0 40px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    text-align: center;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: white;
}

.hero-text button {
    border: none;
    outline: 0;
    display: inline-block;
    padding: 10px 25px;
    color: black;
    background-color: #ddd;
    text-align: center;
    cursor: pointer;
}

.hero-text button:hover {
    background-color: #555;
    color: white;
} */
</style>