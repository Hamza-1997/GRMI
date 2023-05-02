<template>
    <!-- <li class="nav-item dropdown">

        <a class="white rotate-arrow" href="#" role="button" :id="'dropdownMenuLink-' + uniqueId" data-bs-toggle="dropdown"
            aria-haspopup="true" aria-expanded="false" @click="toggleDropdown" :class="{ 'show': showDropdown }">
            {{ buttonText }}
            <img src="../../assets/icons/arrow-down.png" class="img-fluid bi-arrow-down arrow-default" alt="Responsive image">
            <img src="../../assets/icons/arrow-up.png" class="img-fluid bi-arrow-up arrow-open" alt="Responsive image">
        </a>
        <ul class="dropdown-menu">
            <slot></slot>
        </ul>
    </li> -->
    <li class="nav-item dropdown">
        <a class="nav-link white rotate-arrow" href="#" id="navbarDropdownMenuLink" role="button" data-bs-toggle="dropdown"
            aria-expanded="false">
            {{ buttonText }}
            <img src="../../assets/icons/arrow-down.png" class="img-fluid bi-arrow-down arrow-default"
                alt="Responsive image">
            <img src="../../assets/icons/arrow-up.png" class="img-fluid bi-arrow-up arrow-open" alt="Responsive image">
        </a>
        <ul class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink"
            style="padding: 48px;margin:0;background-color: white;white-space: nowrap;">
            <slot></slot>
        </ul>
    </li>
</template>
  
<script>
export default {
    props: {
        // dropdownId: {
        //     type: String,
        //     required: true
        // },
        buttonText: {
            type: String,
            required: true
        },
        //     defaultArrow: {
        //         type: String,
        //         default: '../../assets/icons/arrow-down.png'
        //     },
        //     openArrow: {
        //         type: String,
        //         default: '../../assets/icons/arrow-up.png'
        //     },
        //     uniqueId: {
        //         type: String,
        //         required: true,
        //     },
        // },
        // data() {
        // return {
        //     showDropdown: false
        // };
    },
    // methods: {
    //     toggleDropdown() {
    //         this.showDropdown = !this.showDropdown;
    //     },
    //     closeDropdowns() {
    //         this.showDropdown = false;
    //     },
    //     closeOtherDropdowns() {
    //         const dropdowns = document.querySelectorAll('.dropdown');
    //         dropdowns.forEach((dropdown) => {
    //             if (dropdown !== this.$el) {
    //                 dropdown.__vue__.showDropdown = false;
    //             }
    //         });
    //     }
    // },
    // mounted() {
    //     const dropdownToggle = document.getElementById(this.dropdownId);
    //     const defaultArrow = dropdownToggle.querySelector('.arrow-default');
    //     const openArrow = dropdownToggle.querySelector('.arrow-open');

    //     dropdownToggle.addEventListener('show.bs.dropdown', () => {
    //         defaultArrow.style.display = 'none';
    //         openArrow.style.display = 'inline';
    //         this.showDropdown = true;
    //         this.closeOtherDropdowns()
    //     });

    //     dropdownToggle.addEventListener('hide.bs.dropdown', () => {
    //         defaultArrow.style.display = 'inline';
    //         openArrow.style.display = 'none';
    //         this.showDropdown = false;
    //     });
    // }
}
</script>
  
<style scoped>
.arrow-open {
    display: none;
}

.rotate-arrow.show .arrow-open {
    display: inline;
}

.rotate-arrow.show .arrow-default {
    display: none;
}
</style>