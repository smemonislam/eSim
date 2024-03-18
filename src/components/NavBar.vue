<script>
export default {
  data() {
    return {
      showCopyright: true,
    };
  },
  methods: {
    toggleCopyright() {
      this.showCopyright = !this.showCopyright;
    },
  },
};
</script>
<template>
  <!-- Navbar -->
  <nav
    class="main-header navbar navbar-expand navbar-white navbar-light align-items-center"
  >
    <!-- Left navbar links -->
    <ul class="navbar-nav">
      <li class="nav-item">
        <a
          class="nav-link"
          @click="toggleCopyright"
          data-widget="pushmenu"
          href="#"
          role="button"
          ><i class="fas fa-bars"></i
        ></a>
      </li>
      <li class="nav-item d-none d-sm-inline-block">
        <a href="#" class="btn primary-btn">Book a Shipment</a>
      </li>
    </ul>

    <!-- Right navbar links -->
    <ul class="navbar-nav ml-auto">
      <!-- Notifications Dropdown Menu -->
      <li class="nav-item">
        <a class="nav-link badge-bell" href="#">
          <i class="far fa-bell"></i>
          <span class="badge warning-badge navbar-badge">4</span>
        </a>
      </li>
      <li class="nav-item">
        <a class="nav-link pt-0" href="#">
          <div class="d-flex align-items-center">
            <img src="/img/avatar.png" class="profile_info" alt="Author" />
            <div class="profile_info_iner ml-2">
              <h5>Easwaran</h5>
            </div>
          </div>
        </a>
      </li>
    </ul>
  </nav>
  <aside class="main-sidebar navbar-white elevation-4">
    <!-- Sidebar -->
    <div class="sidebar">
      <!-- Sidebar user (optional) -->
      <div class="user-panel mt-3 pb-3 mb-3 d-flex align-items-center">
        <div class="image">
          <img src="/img/logo.png" alt="Logo" />
        </div>
        <div class="info">
          <a href="#" class="d-block">ShipIndia</a>
        </div>
      </div>

      <!-- Sidebar Menu -->
      <nav class="mt-2 d-flex flex-column justify-content-between v-height">
        <ul
          class="nav nav-pills nav-sidebar flex-column"
          data-widget="treeview"
          role="menu"
          data-accordion="false"
        >
          <li class="nav-item">
            <a href="#" class="nav-link">
              <i class="fa-solid fa-house"></i>
              <p class="ml-3">Dashboard</p>
            </a>
          </li>
          <li class="nav-item">
            <a href="#" class="nav-link">
              <i class="fa-solid fa-box-archive"></i>
              <p class="ml-3">Packages</p>
            </a>
          </li>
          <li class="nav-item">
            <a href="#" class="nav-link">
              <i class="fa-solid fa-ship"></i>
              <p class="ml-3">Shipments</p>
            </a>
          </li>
          <li class="nav-item">
            <a href="#" class="nav-link">
              <i class="fa-solid fa-warehouse"></i>
              <p class="ml-3">Warehouses</p>
            </a>
          </li>
          <li class="nav-item">
            <a href="#" class="nav-link">
              <i class="fa-regular fa-circle-question"></i>
              <p class="ml-3">FAQs</p>
            </a>
          </li>
          <li class="nav-item">
            <a href="#" class="nav-link">
              <i class="fa-regular fa-comment-dots"></i>
              <p class="ml-3">Contact Us</p>
            </a>
          </li>
        </ul>
        <ul
          class="nav nav-pills nav-sidebar flex-column"
          data-widget="treeview"
          role="menu"
          data-accordion="false"
        >
          <li class="nav-item">
            <a href="#" class="nav-link"
              ><svg
                xmlns="http://www.w3.org/2000/svg"
                width="24"
                height="24"
                viewBox="0 0 24 24"
                fill="none"
              >
                <path
                  d="M14 8V6C14 4.89543 13.1046 4 12 4H5C3.89543 4 3 4.89543 3 6V18C3 19.1046 3.89543 20 5 20H12C13.1046 20 14 19.1046 14 18V16"
                  stroke="#6F6B7D"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M7 11.25C6.58579 11.25 6.25 11.5858 6.25 12C6.25 12.4142 6.58579 12.75 7 12.75V11.25ZM21 12V12.75C21.3033 12.75 21.5768 12.5673 21.6929 12.287C21.809 12.0068 21.7448 11.6842 21.5303 11.4697L21 12ZM18.5303 8.46967C18.2374 8.17678 17.7626 8.17678 17.4697 8.46967C17.1768 8.76256 17.1768 9.23744 17.4697 9.53033L18.5303 8.46967ZM17.4697 14.4697C17.1768 14.7626 17.1768 15.2374 17.4697 15.5303C17.7626 15.8232 18.2374 15.8232 18.5303 15.5303L17.4697 14.4697ZM21.5303 12.5303C21.8232 12.2374 21.8232 11.7626 21.5303 11.4697C21.2374 11.1768 20.7626 11.1768 20.4697 11.4697L21.5303 12.5303ZM7 12.75H21V11.25H7V12.75ZM21.5303 11.4697L18.5303 8.46967L17.4697 9.53033L20.4697 12.5303L21.5303 11.4697ZM18.5303 15.5303L21.5303 12.5303L20.4697 11.4697L17.4697 14.4697L18.5303 15.5303Z"
                  fill="#6F6B7D"
                />
              </svg>
              <p class="ml-3">Logout</p></a
            >
          </li>
          <li>
            <p class="copyright ml-3" v-show="showCopyright">
              COPYRIGHT © 2023 <a href="#" class="primary-clr">ShipIndia</a>,
              <br />All rights Reserved
            </p>
          </li>
        </ul>
      </nav>
      <!-- /.sidebar-menu -->
    </div>
    <!-- /.sidebar -->
  </aside>
</template>
