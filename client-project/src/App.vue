<script>
import { ref, onMounted } from "vue";
import LandingPageOne from "./components/LandingPageOne.vue";
export default {
  components: { LandingPageOne },
  setup() {
    const navlinks = ref([
      { id: "navlink-1", label: "HOME", ref: null },
      { id: "navlink-2", label: "ABOUT", ref: null },
      { id: "navlink-3", label: "STORE", ref: null },
      { id: "navlink-4", label: "NEW SEASON", ref: null },
      { id: "navlink-5", label: "CONTACT", ref: null },
    ]);

    const currentActiveLink = ref(null);

    const setElementsLinkRef = (el, i) => {
      if (el) {
        navlinks.value[i].ref = el;
      }
    };

    const handleNavLinks = async (el, i) => {
      if (currentActiveLink.value) {
        currentActiveLink.value.classList.remove("active_navlink");
      }
      currentActiveLink.value = await navlinks.value[i].ref;
      currentActiveLink.value?.classList.add("active_navlink");
    };

    onMounted(() => {
      currentActiveLink.value = navlinks.value[0].ref;
      currentActiveLink.value.classList.add("active_navlink");
    });

    return {
      navlinks,
      setElementsLinkRef,
      handleNavLinks,
    };
  },
};
</script>

<template>
  <header>
    <nav
      class="w-full flex flex-row justify-between md:justify-between py-5 pl-5 pr-10 md:px-10"
    >
      <div class="logo_brand">TERRY_FLOWERS</div>
      <ul class="flex flex-row space-x-4 md:space-x-6">
        <li
          class="navlink"
          :key="item.id"
          :id="item.id"
          v-for="(item, i) in navlinks"
          :ref="(el) => setElementsLinkRef(el, i)"
          @click="async (el) => handleNavLinks(el, i)"
        >
          {{ item.label }}
        </li>
      </ul>
    </nav>
  </header>
  <main class="w-full">
    <LandingPageOne />
  </main>

  <footer>
    <div class="footer_container w-full">
      <div
        class="footer_resume w-full h-[21.375rem] md:h-[28.575rem] pt-10 md:pt-40 px-10 flex flex-col md:flex-row items-center justify-center md:justify-between gap-[2.025rem] md:gap-0"
      >
        <div class="footer_logo_brand self-center md:self-start">
          TERRY FLOWERS
        </div>
        <div
          class="footer_links w-11/12 md:w-8/12 self-center md:self-start flex flex-row justify-start"
        >
          <div class="footer_space w-1/4 flex flex-col items-start gap-8">
            <h4 class="sub_links_title">Home</h4>
            <div
              class="footer_expand_links w-full flex flex-col items-start gap-4"
            >
              <a>about me</a>
              <a>garden</a>
              <a>learn more</a>
            </div>
          </div>
          <div class="footer_space w-1/4 flex flex-col items-start gap-8">
            <h4 class="sub_links_title">store</h4>
            <div
              class="footer_expand_links w-full flex flex-col items-start gap-4"
            >
              <a>recommended</a>
              <a>bunch flowers</a>
              <a>ready to garden</a>
            </div>
          </div>
          <div class="footer_space w-1/4 flex flex-col items-start gap-8">
            <h4 class="sub_links_title">New Season</h4>
            <div
              class="footer_expand_links w-full flex flex-col items-start gap-4"
            >
              <a>feelings</a>
              <a>coming</a>
              <a>discover</a>
            </div>
          </div>
          <div class="footer_space w-1/4 flex flex-col items-start gap-8">
            <h4 class="sub_links_title">Contact</h4>
            <div
              class="footer_expand_links w-full flex flex-col items-start gap-4"
            >
              <a>abdterry@gmail.com</a>
              <a>learn more</a>
              <div
                class="social_media px-[0.5em] py-2 w-full flex flex-row items-center gap-5"
              >
                <i id="facebook" class="media">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    width="18"
                    height="18"
                    viewBox="0 0 486.037 1000"
                  >
                    <path
                      fill="currentColor"
                      d="M124.074 1000V530.771H0V361.826h124.074V217.525C124.074 104.132 197.365 0 366.243 0C434.619 0 485.18 6.555 485.18 6.555l-3.984 157.766s-51.564-.502-107.833-.502c-60.9 0-70.657 28.065-70.657 74.646v123.361h183.331l-7.977 168.945H302.706V1000z"
                    />
                  </svg>
                </i>
                <i id="linkedin" class="media">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    width="18"
                    height="18"
                    viewBox="0 0 1046.16 1000"
                  >
                    <path
                      fill="currentColor"
                      d="M237.485 1000V325.301H13.229V1000zM125.386 233.127c78.202 0 126.879-51.809 126.879-116.553C250.808 50.37 203.591-.001 126.87-.001C50.161-.001-.002 50.371-.002 116.574c0 64.747 48.665 116.553 123.924 116.553h1.457zM361.61 1000h224.256V623.215c0-20.165 1.457-40.309 7.379-54.724c16.212-40.289 53.111-82.017 115.06-82.017c81.149 0 113.613 61.872 113.613 152.572v360.949h224.242V613.129c0-207.241-110.636-303.668-258.183-303.668c-120.977 0-174.094 67.622-203.603 113.679h1.497v-97.853H361.615c2.943 63.31 0 674.699 0 674.699z"
                    />
                  </svg>
                </i>
                <i id="tweeter" class="media">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    width="18"
                    height="18"
                    viewBox="0 0 1231.051 1000"
                  >
                    <path
                      fill="currentColor"
                      d="M1231.051 118.453q-51.422 76.487-126.173 130.403q.738 14.46.738 32.687q0 101.273-29.53 202.791q-29.53 101.519-90.215 194.343T841.297 843.145T639.62 957.395t-252.474 42.606q-210.2 0-387.147-113.493q31.406 3.495 60.242 3.495q175.605 0 313.687-108.177q-81.877-1.501-146.654-50.409q-64.777-48.907-89.156-124.988q24.097 4.59 47.566 4.59q33.782 0 66.482-8.812q-87.378-17.5-144.975-87.04q-57.595-69.539-57.595-160.523v-3.126q53.633 29.696 114.416 31.592q-51.762-34.508-82.079-89.999q-30.319-55.491-30.319-120.102q0-68.143 34.151-126.908q95.022 116.607 230.278 186.392q135.258 69.786 290.212 77.514q-6.609-27.543-6.621-57.485q0-104.546 73.994-178.534Q747.623 0 852.169 0q109.456 0 184.392 79.711q85.618-16.959 160.333-61.349q-28.785 90.59-110.933 139.768q75.502-8.972 145.088-39.677z"
                    />
                  </svg>
                </i>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="footer_terms_use w-full p-5 flex flex-row justify-between">
        <div class="w-max flex gap-2">
          <p>&copy;</p>
          <p>Terry Flowers</p>
        </div>
        <div class="terms_use flex gap-4">
          <a class="underline">Privacy Policy</a>
          <a class="underline">Terms of services</a>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>
ul {
  list-style: none;
}

nav {
  position: fixed;
  top: 0;
  /*  background-color: var(--accent-color-1); */

  background-color: var(--background-aux);

  /* box-shadow: 0px 0px 3px var(--link-color); */

  box-shadow: 0px 0px 3px var(--paragraph-color);
  z-index: 25;
}

@media screen and (min-width: 520px) {
  /* navbar */
  .logo_brand {
    font-family: "Noto Serif", serif;
    font-size: var(--size-cater);
    font-weight: 600;
    color: var(--paragraph-color);
  }

  .navlink {
    color: var(--paragraph-color);
    font-weight: inherit;
    text-decoration: none;
    transition: all 450ms ease-in-out;
  }

  .navlink:hover {
    cursor: pointer;
  }

  .navlink.active_navlink {
    color: var(--paragraph-color);
    font-weight: 600;
    text-decoration: underline;
  }

  /* footer */
  .footer_logo_brand {
    font-size: var(--size-h4);
  }

  footer a {
    line-height: 1.6;
    font-size: var(--size-sm);
    font-family: "Noto Serif", serif;
    font-weight: 300;
    text-decoration: underline;
  }

  .footer_container {
    color: var(--paragraph-color);
    background-color: var(--background-aux);
    font-weight: 500;
  }
}

@media screen and (min-width: 860px) {
  /* navbar */
  .logo_brand {
    font-size: var(--size-regular);
  }

  /* footer */
  .footer_logo_brand {
    font-size: var(--size-h4);
  }
}
</style>
