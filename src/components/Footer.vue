<template>
  <div class="call-to-action d-flex justify-content-between">
    <div class="cta-right pt-5 pb-5 align-items-center">
      <div class="">
        <span class="fw-medium fs-3 text-light"> Trusted Partners </span>
        <div class="separator mt-3"></div>
        <span class="text-light mt-3"
          >Vivamus sed consectetur tellus dolor sit amet, consectetur adipiscing
          lorem elit sadip ipsum ets ficilis uns.
        </span>
      </div>
    </div>
    <div class="cta-right pt-5 pb-5 d-flex flex-column text-light">
      <button>Get a Free Quote</button>
      <span class="text-center pt-3">Only takes a few seconds!</span>
    </div>
  </div>

  <div class="footer-container d-flex justify-content-between">
    <div class="my-footer d-flex flex-column">
      <img
        src="\src\assets\img\footer-logo.png"
        alt="logo"
        style="width: 30px height=30px"
      />
      <span class="text-center fs-6 text-light"
        >We are specialists in the construction of unique and exclusive
        properties. Our work inspires. We pride ourselves on delivering
        outstanding quality and design for leading clients across the
        world.</span
      >
      <button class="btn btn-light mt-2">Learn More</button>
    </div>
    <div class="my-footer d-flex flex-column">
      <h5>LATEST TWEET</h5>
      <div class="mt-3 ms-1">
        <i class="fa-brands fa-x-twitter fa-2xl" style="color: #1d9bf0"></i>
      </div>
      <h2 class="fw-semibold mt-1 text-light">Nothing to see here - yet</h2>
      <small class="text-light mt-1"
        >When they Tweet, their Tweets will show up here.</small
      >
      <button class="btn btn-light mt-3">VIEW ON TWITTER</button>
    </div>
    <div class="my-footer d-flex flex-column">
      <h5>CONTACT US TODAY</h5>
      <ul>
        <li>
          <span>
            <i class="fa-solid fa-globe"></i>
          </span>
          Corporate Location<br />1600 Amphitheatre Parkway<br />London WC1 1BA
        </li>
        <li>
          <span>
            <i class="fa-solid fa-house"></i>
          </span>

          Residential Location<br />
          9521 Broadsberry Avenue<br />
          Paddington RC7 9ZA
        </li>
        <li>
          <i class="fa-solid fa-phone-flip"></i> 1.800.458.556 / 1.800.532.2112
        </li>
        <li><i class="fa-solid fa-phone-flip"></i> info@your-domain.com</li>
        <li>
          <i class="fa-regular fa-clock"></i> Monday – Friday: 9:00 AM – 6:00 PM
        </li>
        <li>
          <i class="fa-regular fa-clock"></i> Saturday – Sunday: 9:00 AM – 12:00
          PM
        </li>
      </ul>
    </div>
    <div class="my-footer d-flex flex-column">
      <h5>Our Location</h5>
      <img
        src="src\assets\img\construction_map_pin.png-Notti"
        alt="maps"
        class="maps"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style lang="scss" scoped>
@import "../assets/style/main.scss";
</style>
