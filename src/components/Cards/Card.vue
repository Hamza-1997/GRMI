<script setup>
import CustomButton from '../Buttons/Button.vue'

</script>

<template>
    <!-- col-sm-12 col-md-4 col-lg-4 -->
    <div class="connection-card">
        <div class="col-lg-12 col-sm-3 w-100">
            <div class="card text-white card-has-bg click-col" style="background-image:url('https://hdwallpaperim.com/wp-content/uploads/2017/08/25/128936-Turkey-Istanbul-building.jpg');
        background-size: cover; background-repeat: no-repeat;background-position: center;border-radius: 16px;">
                <img class="card-img d-none"
                    src="https://hdwallpaperim.com/wp-content/uploads/2017/08/25/128936-Turkey-Istanbul-building.jpg"
                    alt="Goverment Lorem Ipsum Sit Amet Consectetur dipisi?">
                <div class="card-img-overlay d-flex flex-column">
                    <div class="card-body">
                        <!-- <small class="card-meta mb-2">Thought Leadership</small>
                <h4 class="card-title mt-0 "><a class="text-white"
                        herf="#">Goverment Lorem Ipsum Sit Amet Consectetur
                        dipisi?</a></h4>
                <small><i class="far fa-clock"></i> October 15, 2020</small> -->
                    </div>
                    <div class="card-footer" style="padding: 0;">
                        <div class="media d-flex flex-column" style="padding: 0;">
                            <!-- <img class="mr-3 rounded-circle"
                        src="https://assets.codepen.io/460692/internal/avatars/users/default.png"
                        alt="Generic placeholder image" style="max-width:50px"> -->
                            <div class="media-body d-flex flex-column" style="align-items: flex-start;">
                                <div class="M20 white d-block" style="margin-bottom: 4px;">
                                    Benue
                                </div>
                                <div class="M10 white" style="margin-bottom: 8px;">
                                    Nigeria
                                </div>
                            </div>
                            <CustomButton class="M16 white btn-secondary" btn-text="View Maps" type="success" size="lg"
                                style="width: 100%;min-width: 100px;" />
                        </div>
                        <!-- <Button class="M16 primary-700" button-type="primary" button-text="View Maps"
                            style="width: 100%; height: 67px;margin-right: 20px;border: none;border-radius: 8px;"> -->
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.connection-card {
    width: 354px;
    height: 480px;
    /* // padding-top: 20px; */
    /* margin-bottom: 250px; */
    /* position: relative; */
    /* margin-bottom: 20px; */
    /* display: flex; */
    /* flex-flow: column; */
    /* align-items: center; */
    /* margin-bottom: 20px; */
    /* background: #ffffff; */

    /* box-sizing: border-box; */
    /* border: 1px solid #e9ecef; */
    /* border-radius: 16px; */
}


@media only screen and (max-width:800px) {
    .connection-card {
        width: 100%;
        height: 250px;

        /* gap: 0%; */
        margin-bottom: 150px;

    }


}
</style>