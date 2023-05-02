<script>
// export default {
//   data() {
//     return {
//       showDropdown: false
//     };
//   },
//   methods: {
//     toggleDropdown() {
//       this.showDropdown = !this.showDropdown;
//     }
//   },
//   mounted() {
//     const dropdownToggle = document.querySelector('.rotate-arrow');
//     const defaultArrow = document.querySelector('.rotate-arrow .arrow-default');
//     const openArrow = document.querySelector('.rotate-arrow .arrow-open');

//     dropdownToggle.addEventListener('show.bs.dropdown', () => {
//       defaultArrow.style.display = 'none';
//       openArrow.style.display = 'inline';
//       this.showDropdown = true;
//     });

//     dropdownToggle.addEventListener('hide.bs.dropdown', () => {
//       defaultArrow.style.display = 'inline';
//       openArrow.style.display = 'none';
//       this.showDropdown = false;
//     });
//   }
// };
import MyDropdown from './Dropdowns/Dropdowns.vue';
import CustomButton from './Buttons/Button.vue';

export default {
  components: {
    MyDropdown,
    CustomButton
  }
};
</script>

<template>
  <!-- <nav class="navbar bg-dark" data-bs-theme="dark"> -->
  <nav class="navbar navbar-expand-lg bg-dark" data-bs-theme="dark">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">
        <!-- <div> -->
        <router-link to="/">
          <img src='../assets/icons/GRMI_logo.png' alt="Responsive image" width="183" style="color: green;">
        </router-link>
        <!-- </div> -->
      </a>
      <!-- <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button> -->
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown"
        aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavDropdown">
        <ul class="navbar-nav ms-auto me-auto mb-2 mb-lg-0">

          <!-- <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle white" href="#" id="navbarDropdownMenuLink" role="button"
              data-bs-toggle="dropdown" aria-expanded="false">
              Dropdown link
            </a>
            <ul class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
              <li><a class="dropdown-item" href="#">Action</a></li>
              <li><a class="dropdown-item" href="#">Another action</a></li>
              <li><a class="dropdown-item" href="#">Something else here</a></li>
            </ul>
          </li> -->
          <MyDropdown buttonText="About Us">
            <div class="M20 primary-500">About Us</div>
            <router-link to="/about">About GRMI</router-link>

            <router-link to="/team">Team</router-link>
            <router-link to="/news-and-media">News and Media</router-link>

            <!-- <a class="custom-dropdown-item" href="#">Team</a> -->
            <!-- <a class="custom-dropdown-item" href="#">News and Media</a> -->
            <a class="custom-dropdown-item" href="#">Careers</a>
          </MyDropdown>

          <MyDropdown buttonText="Services">

            <a class="custom-dropdown-item" href="#">Item 4</a>
            <a class="custom-dropdown-item" href="#">Item 5</a>
            <a class="custom-dropdown-item" href="#">Item 6</a>
          </MyDropdown>

          <MyDropdown buttonText="Projects">
            <div class="M20 primary-500">Projects</div>
            <router-link to="/completed-projects">Completed</router-link>
            <router-link to="/">Proposed</router-link>
            <router-link to="/">Ongoing</router-link>

            <!-- <a class="custom-dropdown-item" href="#">Item 4</a>
            <a class="custom-dropdown-item" href="#">Item 5</a>
            <a class="custom-dropdown-item" href="#">Item 6</a> -->
          </MyDropdown>

          <MyDropdown buttonText="Data">
            <a class="custom-dropdown-item" href="#">Item 4</a>
            <a class="custom-dropdown-item" href="#">Item 5</a>
            <a class="custom-dropdown-item" href="#">Item 6</a>
          </MyDropdown>

          <MyDropdown buttonText="Partners">
            <a class="custom-dropdown-item" href="#">Item 4</a>
            <a class="custom-dropdown-item" href="#">Item 5</a>
            <a class="custom-dropdown-item" href="#">Item 6</a>
          </MyDropdown>

          <MyDropdown buttonText="Knowledge">
            <router-link to="/insights">Insights</router-link>
            <router-link to="/">Events</router-link>
            <router-link to="/">Research Papers</router-link>
          </MyDropdown>


          <!-- <li class="nav-item">
            <a class="nav-link disabled">Disabled</a>
          </li> -->
        </ul>

        <CustomButton class="M16 white btn-success" btn-text="View Water Level" type="success" size="lg" />
        <!-- style="border-radius: 0;background-color: #134A39;border: none;width: 216px;height: 67px;" -->

      </div>
    </div>
  </nav>
  <!-- <router-view /> -->
</template>

<style scoped>
.navbar {
  padding: 28px 120px 28px 120px;
}

.navbar-nav a {
  color: black;
  display: block;
}

.navbar-nav a:hover {
  color: green;
}

a {
  color: inherit;
  text-decoration: none;
}

/* .custom-dropdown-item */

/* .rotate-arrow .bi-arrow-down {
  transition: transform 0.3s ease;
}

.rotate-arrow.show .bi-arrow-down {
  transform: rotate(180deg);
} */

/* .dropdown .dropdown-toggle:hover {
  background-color: transparent;
} */

/* .dropdown-toggle::after {
  display: none !important;
} */

@media (max-width: 767px) {
  .navbar {
    padding: 40px 0px 40px 0px;
  }
}
</style>
