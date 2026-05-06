<script>
import { ref, onMounted } from "vue";
import LandingPageOne from "./components/LandingPageOne.vue";
export default {
  components: { LandingPageOne },
  setup() {
    const navlinks = ref([
      { id: "navlink-1", label: "Home", ref: null },
      { id: "navlink-2", label: "About", ref: null },
      { id: "navlink-3", label: "Store", ref: null },
      { id: "navlink-4", label: "New Season", ref: null },
      { id: "navlink-5", label: "Contact", ref: null },
    ]);

    const currentActiveLink = ref(null);

    const checkMenuRef = ref(null);

    const middleBarRef = ref(null);

    const modalMenuRef = ref(null);

    const setElementsLinkRef = (el, i) => {
      if (el) {
        navlinks.value[i].ref = el;
      }
    };

    const handleMenu = (e) => {
      console.log("checkMenuRef:", checkMenuRef);
      if (!checkMenuRef.value.checked) {
        middleBarRef.value.classList.add("active_menu");
        modalMenuRef.value.classList.add("active_menu");
      } else {
        middleBarRef.value.classList.remove("active_menu");
        modalMenuRef.value.classList.remove("active_menu");
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
      checkMenuRef,
      middleBarRef,
      modalMenuRef,
      setElementsLinkRef,
      handleNavLinks,
      handleMenu,
    };
  },
};
</script>

<template>
  <header>
    <nav
      class="w-full flex flex-row justify-between py-3 pl-5 pr-7 md:py-5 md:px-10"
    >
      <div class="logo_brand">TERRY_FLOWERS</div>
      <ul
        class="navlink_desktop flex flex-row space-x-4 md:space-x-6 hidden min-[520px]:flex"
      >
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
      <!-- Menu Mobile -->
      <div class="menu_wrap block min-[520px]:hidden">
        <div
          class="menu_content relative w-8 h-8 flex justify-center items-center rounded border border-solid border-[var(--color-text)]"
        >
          <div
            class="middle_bar relative h-[1px] w-[60%] bg-[var(--paragraph-color)] z-0"
            ref="middleBarRef"
          ></div>
          <div
            class="input_check_wrap absolute w-4/5 h-4/5 opacity-0 mx-auto z-10"
            @click="handleMenu"
          >
            <input
              type="checkbox"
              name="checkbox"
              class="check_menu w-full h-full rounded cursor-pointer"
              ref="checkMenuRef"
            />
          </div>
        </div>
        <div class="modal_menu" ref="modalMenuRef">
          <div class="modal_close w-full z-0">
            <div
              class="icon_menu_close w-full h-6 cursor-pointer flex flex-row justify-end z-10"
              @click="handleMenu"
            >
              x
            </div>
          </div>
          <ul class="modal_menu_links flex flex-col space-y-6">
            <li
              class="modal_menu_link"
              :key="item.id"
              :id="item.id"
              v-for="(item, i) in navlinks"
              :ref="(el) => setElementsLinkRef(el, i)"
              @click="async (el) => handleNavLinks(el, i)"
            >
              <div
                class="holder_navlink inline-flex items-center justify-end tansition-all duration-300 ease-in-out hover:text-[var(--accent-color-three)]"
              >
                <div>
                  <p class="nav_p_link">{{ item.label }}</p>
                </div>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </header>
  <main class="w-full">
    <LandingPageOne />
  </main>

  <footer>
    <div class="footer_container w-full">
      <div
        class="footer_resume w-full max-[520px]:h-auto h-[21.375rem] md:h-[28.575rem] pt-10 md:pt-40 px-10 flex flex-col md:flex-row items-center justify-center md:justify-between gap-[2.025rem] md:gap-0"
      >
        <div class="footer_logo_brand self-center md:self-start">
          TERRY FLOWERS
        </div>
        <div
          class="footer_links w-11/12 md:w-8/12 self-center md:self-start flex max-[520px]:flex-col max-[520px]:justify-center flex-row justify-start max-[520px]:gap-[2.025rem] gap-0"
        >
          <div
            class="footer_space max-[520px]:w-full w-1/4 flex flex-col max-[520px]:items-center items-start gap-8"
          >
            <h4 class="sub_links_title">Home</h4>
            <div
              class="footer_expand_links w-full flex flex-col max-[520px]:items-center items-start gap-4"
            >
              <a>about me</a>
              <a>garden</a>
              <a>learn more</a>
            </div>
          </div>
          <div
            class="footer_space max-[520px]:w-full w-1/4 flex flex-col max-[520px]:items-center items-start gap-8"
          >
            <h4 class="sub_links_title">store</h4>
            <div
              class="footer_expand_links w-full flex flex-col max-[520px]:items-center items-start gap-4"
            >
              <a>recommended</a>
              <a>bunch flowers</a>
              <a>ready to garden</a>
            </div>
          </div>
          <div
            class="footer_space max-[520px]:w-full w-1/4 flex flex-col max-[520px]:items-center items-start gap-8"
          >
            <h4 class="sub_links_title">New Season</h4>
            <div
              class="footer_expand_links w-full flex flex-col max-[520px]:items-center items-start gap-4"
            >
              <a>feelings</a>
              <a>coming</a>
              <a>discover</a>
            </div>
          </div>
          <div
            class="footer_space max-[520px]:w-full w-1/4 flex flex-col max-[520px]:items-center items-start gap-8"
          >
            <h4 class="sub_links_title">Contact</h4>
            <div
              class="footer_expand_links w-full flex flex-col max-[520px]:items-center items-start gap-4"
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

@media screen and (min-width: 140px) {
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

  /* Menu Mobile */
  .middle_bar {
    transition: all 1s ease;
  }

  .middle_bar::before {
    content: "";
    position: absolute;
    top: -6px;
    left: 0;
    right: 0;
    width: 100%;
    height: 1px;
    background-color: var(--paragraph-color);
    transition: all 1s ease;
  }

  .middle_bar::after {
    content: "";
    position: absolute;
    top: 6px;
    left: 0;
    right: 0;
    width: 100%;
    height: 1px;
    background-color: var(--paragraph-color);
    transition: all 1s ease;
  }

  .input_check_wrap {
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  /* activate menu */

  .middle_bar.active_menu {
    transform: rotate(135deg);
  }

  .middle_bar.active_menu::before {
    top: 0;
    /* transform: rotate(45deg); */
    transform: rotate(90deg);
  }

  .middle_bar.active_menu::after {
    top: 0;
    /* transform: rotate(135deg); */
    transform: rotate(90deg);
  }

  .modal_menu {
    position: absolute;
    top: 4.275rem;
    left: 0;
    /*  transform: scale(0.45) translateX(-50%); */
    transform: translateX(-100%);
    width: max(275px, 92%);
    height: max-content;
    padding: 1.125rem 0.9rem;
    color: var(--paragraph-color);
    background-color: var(--background-main);
    visibility: invisible;
    opacity: 0;
    border-radius: 50%;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    transition: all 310ms linear;
  }

  .modal_menu.active_menu {
    position: absolute;
    top: 4.53rem;
    left: 50%;
    /* transform: scale(1) translateX(-50%); */
    transform: translateX(-50%);
    width: max(260px, 90%);
    height: max-content;
    padding: 1.125rem 0.9rem;
    visibility: visible;
    opacity: 0.99;
    border-radius: 2px;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    transition: all 300ms linear;
  }
}

@media screen and (min-width: 520px) {
  /* navbar */
  .logo_brand {
    font-family: "Noto Serif", serif;
    font-size: var(--size-cater);
    font-weight: 600;
    color: var(--leading-color);
  }

  .navlink {
    color: var(--paragraph-color);
    opacity: 0.86;
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
