<template>
  <div>
    <!-- Start Footer Section -->
    <footer class="ftco-footer py-5">
      <div class="container text-center">
        <div class="row">
          <div class="col-md-12 text-center">
            <p>
              <!-- Link back to Colorlib can't be removed. Template is licensed under CC BY 3.0. -->
              Copyright &copy;
              {{ getThisYear }} All rights reserved | This template is made with
              <i
                class="icon-heart"
                aria-hidden="true"
              ></i> by
              <a href="https://colorlib.com" target="_blank">Colorlib</a>
              <!-- Link back to Colorlib can't be removed. Template is licensed under CC BY 3.0. -->
            </p>

            <ul class="ftco-footer-social p-0">
              <li class="ftco-animate">
                <a href="#">
                  <span class="icon-twitter"></span>
                </a>
              </li>
              <li class="ftco-animate">
                <a href="#">
                  <span class="icon-facebook"></span>
                </a>
              </li>
              <li class="ftco-animate">
                <a href="#">
                  <span class="icon-instagram"></span>
                </a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </footer>
    <!-- End Footer Section -->
  </div>
</template>

<script>
export default {
  computed: {
    getThisYear() {
      return new Date().getFullYear();
    }
  }
};
</script>

<style>
</style>