<script>
export default {
  setup() {
    return {};
  },
};
</script>

<template>
  <div id="landing_page" class="landing_page p-0">
    <!-- hero section -->
    <section class="hero_section w-full">
      <div class="hero_content relative pt-10 w-full h-full px-[2.25rem]">
        <div class="hero_image absolute top-10 left-0"></div>
        <div
          class="hero_context w_ct_max_1 h-full mx-auto flex flex-col items-center justify-center"
        >
          <div
            class="hero_value w-full flex flex-col justify-center text-center break-words pt-[0.225rem]"
          >
            <h1 class="core_value font-bold pb-[1.125rem]">
              Decorate your Home, your Events' Space With Natural Flowers Grown
              With Love And Care
            </h1>
            <div
              class="sub_core_value text-[var(--paragraph-color)] pb-[2.25rem] mx-auto"
            >
              <p class="w-max px-[0.225rem]">
                Reconquer your happiness and energize your soul standing over
                beautiful scenery's flowers
              </p>
            </div>
          </div>
          <div
            class="hero_btn pt-[2.925rem] pb-[0.9rem] w-full flex flex-row justify-center gap-[1.8rem]"
          >
            <a href="#" class="btn_order">Place An Order</a>
            <a class="btn_in_shelves">In Shelves</a>
          </div>
        </div>
      </div>
    </section>

    <!-- about me section -->
    <section class="about_section w-full relative mt-[4.5rem]">
      <div
        class="about_content flex flex-row-reverse justify-center h-[20.7rem] mx-auto py-[0.45rem]"
      >
        <figure class="about_image">
          <img
            class="about_pic"
            src="/src/assets/images/woman-8344944_1280.jpg"
          />
          <figcaption
            class="fig_caption flex flex-row justify-end pt-[0.225rem]"
          >
            Image by
            <a
              class="ref_pixabay"
              href="https://pixabay.com/users/long_phung-22896646/?utm_source=link-attribution&utm_medium=referral&utm_campaign=image&utm_content=8894656"
              >Long Phung</a
            >
            from
            <a
              class="ref_pixabay"
              href="https://pixabay.com//?utm_source=link-attribution&utm_medium=referral&utm_campaign=image&utm_content=8894656"
              >Pixabay</a
            >
          </figcaption>
        </figure>
        <div class="about_context w-[56.2%] flex flex-col">
          <h3 class="title_context font-semibold pt-[0.45rem] pb-[1.575rem]">
            About Me
          </h3>
          <div class="about_deal">
            <p
              class="about_dealing_text font-light break-words w-[90%] mb-[1.8rem]"
            >
              My Name is Terry Jehnkins. Over 14years+ i confered my flowers]
              passion a commitment to turn back love, peace, and fulfillment to
              everyone Terry Flowers is my drive to realize so. Tail off grudge
              and pain, and be able to cement a new love where senses pleasurely
              engage to walk you in a life you be happier to set.
            </p>
          </div>
          <div class="about_btn">
            <a class="btn_visit_shop">Visit Our Shop </a>
          </div>
        </div>
      </div>
    </section>

    <!-- recommended flowers section -->

    <section class="recommended_section w-full mt-[1.575rem]">
      <div
        class="recommended_content w_full bg-[var(--background-main)] flex flex-col pt-[1.575rem] pb-[1.35rem] px-[1.35rem]"
      >
        <h3 class="title_context font-semibold pt-[0.45rem] pb-[1.575rem]">
          Recommended
        </h3>
        <div
          class="recommended_deal px-[1.35rem] pb-[1.575rem] grid-cols-3 grid-rows-1 auto-rows-max"
        >
          <div class="recommended_item">
            <figure class="recommended_image">
              <img
                class="recommended_pic object-cover"
                src="/src/assets/images/flowers-8763039_1280.jpg"
              />

              <figcaption>
                <span>Daisies- All fit</span>
              </figcaption>
            </figure>
          </div>
          <div>
            <figure class="recommended_image">
              <img
                class="recommended_pic object-cover"
                src="/src/assets/images/Rosy_bad-Homburg-Germany_Pixabay.jpg"
              />

              <figcaption>
                <span>flower- room/ space</span>
              </figcaption>
            </figure>
          </div>
          <div>
            <figure class="recommended_image">
              <img
                class="recommended_pic object-cover"
                src="/src/assets/images/Manfred-Richter_Pixabay.jpg"
              />

              <figcaption>
                <span>flower- events</span>
              </figcaption>
            </figure>
          </div>
        </div>
        <div class="recommended_btn flex flex-row justify-end">
          <a href="#" class="btn_order">Place An Order</a>
        </div>
      </div>
    </section>

    <!-- shelves section -->
    <div class="shelves_section">
      <div class="shelves_content pt-[2.7rem] pb-[5.4rem] px-[1.35rem]">
        <h3 class="title_context font-semibold pt-[0.45rem] pb-[1.575rem]">
          Available in shelves
        </h3>
        <div class="shelves_deal w_ct_max_1 pb-[2.025rem] mx-auto">
          <div class="shelves_item">
            <figure class="shelves_image">
              <img
                class="shelves_pic object-cover"
                src="/src/assets/images/cactus-7914007_1280.jpg"
              />

              <figcaption class="fig_caption w-full grid place-items-center">
                <span>Cactus</span>
              </figcaption>
            </figure>
          </div>
          <div class="shelves_item">
            <figure class="shelves_image">
              <img
                class="shelves_pic object-cover"
                src="/src/assets/images/flower-3597681_1280.jpg"
              />

              <figcaption class="fig_caption w-full grid place-items-center">
                <span>flower-2</span>
              </figcaption>
            </figure>
          </div>
          <div class="shelves_item">
            <figure class="shelves_image">
              <img
                class="shelves_pic object-cover"
                src="/src/assets/images/flower-4590455_1280.jpg"
              />

              <figcaption class="fig_caption w-full grid place-items-center">
                <span>flower-3</span>
              </figcaption>
            </figure>
          </div>
          <div class="shelves_item">
            <figure class="shelves_image">
              <img
                class="shelves_pic object-cover"
                src="/src/assets/images/flower-8384360_1280.jpg"
              />

              <figcaption class="fig_caption w-full grid place-items-center">
                <span>flower-4</span>
              </figcaption>
            </figure>
          </div>
          <div class="shelves_item">
            <figure class="shelves_image">
              <img
                class="shelves_pic object-cover"
                src="/src/assets/images/flowers-2068692_1280.jpg"
              />

              <figcaption class="fig_caption w-full grid place-items-center">
                <span>flower-5</span>
              </figcaption>
            </figure>
          </div>
          <div class="shelves_item">
            <figure class="shelves_image">
              <img
                class="shelves_pic object-cover"
                src="/src/assets/images/flower-9221176_1280.jpg"
              />

              <figcaption class="fig_caption w-full grid place-items-center">
                <span>flower-6</span>
              </figcaption>
            </figure>
          </div>
        </div>
        <div class="shelves_btn flex flex-row justify-end">
          <a class="btn_in_shelves">In Shelves</a>
        </div>
      </div>
    </div>

    <!-- services section -->
    <section class="services_section">
      <div
        class="bar_deco_1 w-[60%] h-[4px] text-opacity-50 mx-auto bg-[var(--background-main)] rounded-xl"
      ></div>
      <div class="services_content pt-[4.5rem] pb-[1.35rem] px-[1.35rem]">
        <h3
          class="title_context w-full text-center font-semibold pt-[0.45rem] pb-[2.7rem]"
        >
          Services
        </h3>
        <div
          class="services_deal w-[75%] pb-[2.025rem] flex flex-col gap-[2.025rem] mx-auto"
        >
          <article
            class="service_item w-full h-[12.6rem] py-[1.35rem] px-[1.125rem] bg-[var(--background-main)] flex flex-row justify-between border border-solid border-[var(--background-aux)] rounded-sm"
          >
            <figure class="service_image w-[38.6%]">
              <img
                class="service_pic w-full h-full object-cover rounded-sm"
                src="/src/assets/images/flower-3339266_1280.jpg"
              />
              <figcaption></figcaption>
            </figure>
            <div class="service_context w-[59.4%]">
              <div class="service_trade">
                <h3
                  class="title_context font-semibold pt-[0.45rem] pb-[1.575rem]"
                >
                  Cheerful Happiness
                </h3>
                <p>
                  Get New Flowers on our store each season. Make thoughtfull
                  Gifts or align your space with the swing of the time.
                </p>
              </div>
            </div>
          </article>
          <article
            class="service_item w-full h-[12.6rem] py-[1.35rem] px-[1.125rem] bg-[var(--background-main)] flex flex-row-reverse justify-between border border-solid border-[var(--background-aux)] rounded-sm"
          >
            <figure class="service_image w-[38.6%]">
              <img
                class="service_pic w-full h-full object-cover rounded-sm"
                src="/src/assets/images/plum-blossoms-8579641_1280.jpg"
              />
              <figcaption></figcaption>
            </figure>
            <div class="service_context w-[59.4%]">
              <div class="service_trade">
                <h3
                  class="title_context font-semibold pt-[0.45rem] pb-[1.575rem]"
                >
                  Decoration
                </h3>
                <p>
                  Organize desirably flowers for your space or events. Harmonize
                  your thoughts, get new meaningful ideas in mind
                </p>
              </div>
            </div>
          </article>
          <article
            class="service_item w-full h-[12.6rem] py-[1.35rem] px-[1.125rem] bg-[var(--background-main)] flex flex-row justify-between border border-solid border-[var(--background-aux)] rounded-sm"
          >
            <figure class="service_image w-[38.6%]">
              <img
                class="service_pic w-full h-full object-cover rounded-sm"
                src="/src/assets/images/zinnia-3518967_1280.jpg"
              />
              <figcaption></figcaption>
            </figure>
            <div class="service_context w-[59.4%]">
              <div class="service_trade">
                <h3
                  class="title_context font-semibold pt-[0.45rem] pb-[1.575rem]"
                >
                  Gardening
                </h3>
                <p>
                  We can assist and advice you at growing your personal garden
                  at home. A sanctuary where spending times in, brings you joy,
                  peace, and productivity.
                </p>
              </div>
            </div>
          </article>
        </div>
        <div class="services_btn flex flex-row justify-end">
          <a href="#" class="btn_order">Place An Order</a>
        </div>
      </div>
    </section>

    <!-- upcoming section -->
    <section class="upcoming_section w-full mt-[1.575rem]">
      <div
        class="recommended_content w_full bg-[var(--background-main)] flex flex-col pt-[1.575rem] pb-[1.35rem] px-[1.35rem]"
      >
        <h3 class="title_context font-semibold pt-[0.45rem] pb-[1.575rem]">
          Next Quater Upcoming
        </h3>
        <div
          class="recommended_deal px-[1.35rem] pb-[1.575rem] grid-cols-3 grid-rows-1 auto-rows-max"
        >
          <div class="recommended_item">
            <figure class="recommended_image">
              <img
                class="recommended_pic object-cover"
                src="/src/assets/images/flowers-8763039_1280.jpg"
              />

              <figcaption>
                <span>Daisies- All fit</span>
              </figcaption>
            </figure>
          </div>
          <div>
            <figure class="recommended_image">
              <img
                class="recommended_pic object-cover"
                src="/src/assets/images/Rosy_bad-Homburg-Germany_Pixabay.jpg"
              />

              <figcaption>
                <span>flower- room/ space</span>
              </figcaption>
            </figure>
          </div>
          <div>
            <figure class="recommended_image">
              <img
                class="recommended_pic object-cover"
                src="/src/assets/images/Manfred-Richter_Pixabay.jpg"
              />

              <figcaption>
                <span>flower- events</span>
              </figcaption>
            </figure>
          </div>
        </div>
        <div class="upcoming_btn flex flex-row justify-end">
          <a href="#" class="btn_in_shelves">In Shelves</a>
        </div>
      </div>
    </section>

    <!-- special offer section -->
    <section class="offer_section w-full">
      <div class="section_content relative w-full h-[23.4rem]">
        <div class="special_image"></div>
        <div
          class="special_deal absolute top-0 w-full h-full pt-[2.925rem] flex flex-col items-center"
        >
          <h3
            class="title_context w-full text-[var(--background-main)] text-center font-bold pt-[0.45rem] pb-[1.8rem]"
          >
            Special Offers
          </h3>
          <div class="special_context w-8/12 mx-auto">
            <h4
              class="special_text w-full text-[var(--background-main)] text-center font-semibold pb-[2.925rem]"
            >
              Get 20% off on all orders above $150. Use code: FLOWER20 at
              checkout. Limited time offer!
            </h4>
            <div class="special_btn flex flex-row justify-end">
              <a href="#" class="btn_order">Place An Order</a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- trust section -->
    <section class="trust_section w-full">
      <div class="trust_content pt-[4.05rem] pb-[1.35rem] px-[1.35rem]">
        <h3
          class="title_context w-full text-center font-semibold pt-[0.45rem] pb-[3.15rem]"
        >
          Why Us ?
        </h3>
        <div class="trust_deal pb-[3.375rem]">
          <div
            id="benefit_item1"
            class="px-[1.125rem] w-full flex flex-row items-center justify-start gap-[1.35rem] border-r-4 border-solid border-[var(--background-main)] rounded-sm"
          >
            <div class="icon_wrap">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="28"
                height="28"
                viewBox="0 0 24 24"
              >
                <path
                  fill="currentColor"
                  d="M21.45 7.5H9.99A2 2 0 0 0 8.06 6h-1a2 2 0 0 0-1.93 1.5H2.55a.5.5 0 0 0-.5.5a.51.51 0 0 0 .5.5h2.58A2 2 0 0 0 7.06 10h1a2 2 0 0 0 1.93-1.5h11.46a.5.5 0 0 0 0-1M8.06 9h-1a1.006 1.006 0 0 1-1-.98V8a1 1 0 0 1 1-1h1a1 1 0 1 1 0 2m13.39 6.5h-2.58a2 2 0 0 0-1.93-1.5h-1a2 2 0 0 0-1.93 1.5H2.55a.5.5 0 0 0 0 1h11.46a2 2 0 0 0 1.93 1.5h1a2 2 0 0 0 1.93-1.5h2.58a.5.5 0 0 0 .5-.5a.51.51 0 0 0-.5-.5m-3.51.5a1 1 0 0 1-1 1h-1a1 1 0 1 1 0-2h1a1.006 1.006 0 0 1 1 .98Z"
                />
              </svg>
            </div>
            <div class="benefit_context w-[80%] flex flex-col gap-[1.125rem]">
              <h4 class="benefit_title">Priority</h4>
              <p class="benefit_text">
                We are not just delivering, we aims to tease your happiness
                after understanding the essence of your demands.
              </p>
            </div>
          </div>
          <div
            id="benefit_item2"
            class="px-[1.125rem] w-full flex flex-row justify-start gap-[1.35rem]"
          >
            <div class="icon_wrap">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="28"
                height="28"
                viewBox="0 0 24 24"
              >
                <path
                  fill="currentColor"
                  d="M4.415 7.22a.76.76 0 0 0-.35.64v9.67a1.54 1.54 0 0 0 .88 1.38l5.96 2.82a2.62 2.62 0 0 0 2.19 0l5.96-2.82a1.54 1.54 0 0 0 .88-1.38V7.86a.74.74 0 0 0-.36-.64l-2.23-1.15v-1a1 1 0 0 0-.15-.52l-1.33-2.16a.75.75 0 0 0-1.28 0L13.3 4.5l-.66-1.07a.76.76 0 0 0-.64-.35a.79.79 0 0 0-.64.36l-.65 1.06L9.4 2.39a.75.75 0 0 0-1.28 0L6.805 4.55a1 1 0 0 0-.15.52v1Zm12.93-.01l.7.35l-.7.33Zm-2.44-3.43h.64l.5.81h-1.64Zm1.44 1.81v2.77l-.61.29V5.59Zm-2.23 0h.62v3.53l-.62.3Zm-5.67-1.81h.64l.5.81h-1.64Zm1.44 1.81v3.82l-.61-.29V5.59Zm-2.23 0h.62v3.06l-.62-.29Zm-1 1.62v.68l-.7-.33ZM5.365 18a.52.52 0 0 1-.3-.47V8.24l6.43 3.04v9.59Zm6.13-7.83l-.61-.29V6.64h.61Zm-.32-4.53l.51-.82h.62l.51.82Zm1.94 1v3.25l-.62.29V6.64ZM12.5 20.88v-9.59l6.44-3.05v9.29a.51.51 0 0 1-.31.47Z"
                />
              </svg>
            </div>
            <div class="benefit_context w-[80%] flex flex-col gap-[1.125rem]">
              <h4 class="benefit_title">Support</h4>
              <p class="benefit_text">
                Advice you on the process of growing or taking care of natural
                flowers for your garden or home.
              </p>
            </div>
          </div>
          <div
            id="benefit_item3"
            class="px-[1.125rem] w-full flex flex-row justify-start gap-[1.35rem]"
          >
            <div class="icon_wrap">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="28"
                height="28"
                viewBox="0 0 24 24"
              >
                <path
                  fill="currentColor"
                  d="M12.6 20.936h-1.3a.88.88 0 0 1-.852-.654l-.774-2.833l-2.5 1.435a.886.886 0 0 1-1.06-.138l-.925-.919a.884.884 0 0 1-.143-1.066l1.469-2.545l-.006-.016l-2.787-.747a.88.88 0 0 1-.654-.851V11.3a.88.88 0 0 1 .652-.85l2.839-.777L5.12 7.171a.885.885 0 0 1 .141-1.062l.918-.918a.885.885 0 0 1 1.061-.142l2.552 1.465h.012l.745-2.79a.88.88 0 0 1 .851-.655h1.3a.88.88 0 0 1 .852.655l.762 2.838l2.509-1.441a.885.885 0 0 1 1.059.138l.926.919a.88.88 0 0 1 .141 1.067l-1.466 2.532l.008.022l2.786.746a.88.88 0 0 1 .653.851v1.3a.88.88 0 0 1-.654.852l-2.837.774l1.439 2.505a.88.88 0 0 1-.141 1.063l-.917.917a.89.89 0 0 1-1.063.141l-2.539-1.462l-.018.014l-.745 2.785a.885.885 0 0 1-.855.651m-1.21-1h1.119l.738-2.756a.89.89 0 0 1 .528-.592l.134-.052a.87.87 0 0 1 .76.057l2.51 1.445l.789-.789l-1.423-2.478a.88.88 0 0 1-.048-.78l.052-.125a.88.88 0 0 1 .584-.51l2.8-.749v-1.12l-2.755-.737a.89.89 0 0 1-.592-.529l-.052-.132a.88.88 0 0 1 .057-.763l1.449-2.508l-.8-.79l-2.48 1.425a.88.88 0 0 1-.772.052l-.115-.047a.89.89 0 0 1-.518-.588l-.748-2.806h-1.115l-.738 2.762a.88.88 0 0 1-.539.6l-.12.045a.87.87 0 0 1-.751-.058L6.822 5.962l-.789.789l1.422 2.476a.89.89 0 0 1 .046.785l-.051.12a.88.88 0 0 1-.579.5l-2.8.758v1.121l2.757.738a.89.89 0 0 1 .591.525l.048.121a.87.87 0 0 1-.055.77l-1.454 2.516l.8.791l2.47-1.419a.88.88 0 0 1 .787-.045l.106.044a.87.87 0 0 1 .526.591Zm-1.64-2.454h.008Zm-.15-.061h.007Zm4.655-10.885"
                />
                <path
                  fill="currentColor"
                  d="M12 15a3 3 0 1 1 3-3a3 3 0 0 1-3 3m0-5a2 2 0 1 0 2 2a2 2 0 0 0-2-2"
                />
              </svg>
            </div>
            <div class="benefit_context w-[80%] flex flex-col gap-[1.125rem]">
              <h4 class="benefit_title">Flexibility</h4>
              <p class="benefit_text">
                We desirably work with you to organize, arrange, and spark
                beautiful sceneries of flowers.
              </p>
            </div>
          </div>
        </div>
        <div class="trust_btn flex flex-row justify-end">
          <a class="btn_visit_shop">Visit Our Shop </a>
        </div>
      </div>
    </section>

    <!-- testimonials section -->
    <section class="testimonials_section w-full">
      <div class="testimonials_content pt-[4.275rem]">
        <h3
          class="title_context w-full text-center font-semibold pt-[0.45rem] pb-[2.7rem]"
        >
          Testimonials
        </h3>
        <div
          class="testimonials_deal flex flex-col items-center gap-[2.7rem] rounded"
        >
          <article
            class="testimonial_item w-full bg-[var(--background-main)] pt-[1.125rem] pb-[2.025rem] px-[1.125rem] flex flex-row justify-center items-center gap-[1.8rem]"
          >
            <div class="testimonial_image self-end">
              <p class="font-bold text-[var(--title-color)]">1</p>
            </div>
            <div class="testimonial_context w-[72%]">
              <h4
                class="testimonial_title w-full text-left font-semibold pb-[0.45rem]"
              >
                Monique
              </h4>
              <span class="testimonial_text w-full text-justify font-light">
                I was confuse about the choice of the shops to have me made new
                decoration for my son's birthday. I gave Terry Flowers a try ,
                the result was glowing. They didn't just deliver , they help me
                spark my home with beautifuls flowers coupling with the frame's
                furniture as they were living with me for years.
              </span>
            </div>
          </article>

          <article
            class="testimonial_item w-full bg-[var(--background-main)] pt-[1.125rem] pb-[2.025rem] px-[1.125rem] flex flex-row justify-center items-center gap-[1.8rem]"
          >
            <div class="testimonial_image self-end">
              <p class="font-bold text-[var(--title-color)]">2</p>
            </div>
            <div class="testimonial_context w-[72%]">
              <h4
                class="testimonial_title w-full text-left font-semibold pb-[0.45rem]"
              >
                Arlan
              </h4>
              <span class="testimonial_text w-full text-justify font-light">
                After my retirement. I find difficult staying at home by myself
                . I discovered my love for flowers one day at a meeting of
                ex-students in my university. I try a service online of Terry
                flowers, they even help me grow a mini-garden in my home's
                backyard. All these flowers give me a regain of confidence and
                courage to help people online with my skills via consulting.
              </span>
            </div>
          </article>

          <article
            class="testimonial_item w-full bg-[var(--background-main)] pt-[1.125rem] pb-[2.025rem] px-[1.125rem] flex flex-row justify-center items-center gap-[1.8rem]"
          >
            <div class="testimonial_image self-end">
              <p class="font-bold text-[var(--title-color)]">3</p>
            </div>
            <div class="testimonial_context w-[72%]">
              <h4
                class="testimonial_title w-full text-left font-semibold pb-[0.45rem]"
              >
                Isabella
              </h4>
              <span class="testimonial_text w-full text-justify font-light">
                I always have to plan many wedding. with a tight schedule or
                reorganisal at the last minute. With Terry Flowers, i find the
                services at delivery amazing. They understand quickly the need
                of the moment and supply diverse flowers that fit perfectly the
                event's theme.
              </span>
            </div>
          </article>
        </div>
      </div>
    </section>

    <!-- reinforcement section -->
    <section
      class="reinforcement_section w-full bg-[var(--background-aux)] text-opacity-80 relative mt-[7.425rem]"
    >
      <div
        class="about_content flex flex-row justify-between gap-[1.8rem] mx-auto pt-[4.05rem] pb-[2.925rem]"
      >
        <figure class="about_image">
          <img
            class="about_pic"
            src="/src/assets/images/woman-8894656_1280.jpg"
          />
          <figcaption
            class="fig_caption flex flex-row justify-start pt-[0.225rem]"
          >
            Image by
            <a
              class="ref_pixabay"
              href="https://pixabay.com/users/long_phung-22896646/?utm_source=link-attribution&utm_medium=referral&utm_campaign=image&utm_content=8894656"
              >Long Phung</a
            >
            from
            <a
              class="ref_pixabay"
              href="https://pixabay.com//?utm_source=link-attribution&utm_medium=referral&utm_campaign=image&utm_content=8894656"
              >Pixabay</a
            >
          </figcaption>
        </figure>
        <div class="about_context w-[56.2%] flex flex-col">
          <h3 class="title_context font-semibold pt-[0.45rem] pb-[1.575rem]">
            Close Happiness
          </h3>
          <div class="about_deal">
            <p
              class="about_dealing_text font-light break-words w-[90%] mb-[1.8rem]"
            >
              Capture Moments That Crystallize Your Entire Events. Share the
              beauty Quietly and peacefully.
            </p>
          </div>
          <div class="about_btn">
            <a class="btn_visit_shop">Visit Our Shop </a>
          </div>
        </div>
      </div>
    </section>

    <!-- farewell section -->
    <section class="farewell_section w-full">
      <div class="farewell_content relative w-full h-[31.5rem]">
        <div class="farewell_drop_shadow"></div>
        <div class="farewell_deal w-full h-full">
          <div class="farewell_image"></div>
          <div
            class="farewell_context absolute top-0 left-0 w-full h-full grid place-items-center"
          >
            <h1
              class="farewell_text variant_h10 w-[86%] mx-auto font-semibold text-center break-words"
            >
              A Fairy World Created By Yourself. A Sustainable Holder For Your
              Happiness And Reconnection With Your Divine's Senses
            </h1>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<style scoped>
.landing_page {
  scroll-margin-top: 12px;
}

@media screen and (min-width: 768px) {
  /* utilities */
  .w_ct_max_1 {
    width: 61.2rem;
  }

  /* hero section */
  .hero_section {
    position: relative;
    width: 100%;
    height: 80vh;
    /*  background: linear-gradient(
      97.39deg,
      hsl(35, 18%, 90%) 25.12%,
      hsl(35, 18%, 75%) 82.16%
    ); */
  }

  .hero_content {
    backdrop-filter: blur(48px);
  }

  .hero_image {
    width: max(100%, 16.2rem);
    height: 90%;
    border-top: 2px solid var(--background-aux);
    border: 2px solid transparent;
    background: url("../assets/images/Couleur_Pixabay.jpg") left center
      no-repeat;
    background-size: 100%;
    backdrop-filter: grayscale(18%);
    backdrop-filter: hue-rotate(240deg);
    border: none;
    outline: none;
    z-index: -1;
  }

  .sub_core_value p {
    filter: drop-shadow(#ee969d 0.25rem 0.25rem 1rem);
    background-color: var(--background-aux);
    backdrop-filter: invert(30%);
  }

  .hero_image::before {
    content: "";
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    opacity: 0.45;
  }

  /* about section */
  .about_content {
    width: min(92%, 61.2rem);
  }

  .about_image {
    width: 42.6%;
    padding: 0.45rem;
  }

  .about_pic {
    width: 100%;
    aspect-ratio: 16/10;
    object-fit: cover;
  }

  /* recommended flowers section */
  .recommended_deal {
    width: max(60%, 40.05rem);
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: max-content;
    gap: 1.35rem;
  }

  /* shelves section */
  .shelves_deal {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(15.75rem, 1fr));
    grid-template-rows: max-content;
    place-items: center;
    gap: 1.35rem;
  }

  .shelves_item {
    width: 100%;
    height: 100%;
    padding: 1.125rem;
    border-radius: 0.225rem;
    text-align: center;
    display: grid;
    grid-template-rows: subgrid;
    grid-row: span 1;
  }

  .shelves_image {
    width: 100%;
    height: 100%;
    display: grid;
    grid-template-columns: 100%;
    grid-template-rows: 94% auto;
    gap: 1.125rem;
  }

  .shelves_pic {
    width: 100%;
    height: 100%;
  }

  /* special offer section */
  .special_image {
    width: 100%;
    height: 100%;
    /*  border-top: 2px solid var(--background-aux); */
    border: 2px solid transparent;
    background: url("../assets/images/chaos-answer_pixabay.jpg") left center
      no-repeat;
    background-size: 100%;
    backdrop-filter: invert(70%);
    border: none;
    outline: none;
    z-index: -1;
  }

  /* trust section */

  .trust_deal {
    width: max(70%, 40.05rem);
    margin: 0 auto;
    display: grid;
    grid-template-areas:
      "benefit-1 benefit-1 benefit-2 benefit-2"
      "benefit-1 benefit-1 benefit-3 benefit-3";
    gap: 1.35rem;
    grid-template-columns: 25% 25% 25% 25%;
    grid-template-rows: auto auto;
  }

  #benefit_item1 {
    width: 100%;
    grid-area: benefit-1;
    grid-column: 1 / span 2;
    grid-row: 1 / span 2;
  }

  #benefit_item2 {
    width: 100%;
    grid-area: benefit-2;
    grid-column: 3 / span 2;
    grid-row: 1 / span 1;
  }

  #benefit_item3 {
    width: 100%;
    grid-area: benefit-3;
    grid-column: 3 / span 2;
    grid-row: 2 / span 1;
  }

  /* testimonials section */
  .testimonials_deal {
    width: max(70%, 40.05rem);
    margin: 0 auto;
  }

  .testimonial_image {
    flex-shrink: 0;
    width: 5.85rem;
    height: 5.85rem;
    display: grid;
    place-items: center;
    background-color: var(--background-aux);
    clip-path: polygon(
      20% 0%,
      80% 0%,
      100% 20%,
      100% 80%,
      80% 100%,
      20% 100%,
      0% 80%,
      0% 20%
    );
  }

  /* reinforcement section */

  /* farewell section */
  .farewell_drop_shadow {
    position: absolute;
    top: 0;
    width: 100%;
    height: 100%;
    background-color: hsla(0, 0%, 12%, 0.349);
  }

  .farewell_image {
    width: 100%;
    height: 100%;
    background: url("../assets/images/kasjan-farbisz_pixabay.jpg") left center
      no-repeat;
    background-size: 100%;
    border: none;
    outline: none;
    /* z-index: -1; */
  }
}
</style>
