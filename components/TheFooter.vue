<template>
  <footer class="bg-electric-pink">
    <div
      class="container mx-auto pt-[50px] pb-[10px] px-[17.5px] md:pt-[70px] md:pb-[20px] md:px-[30px] 2xl:pt-[109px] 2xl:px-[55px]"
    >
      <div
        class="flex flex-col items-center 2xl:flex-row 2xl:items-start 2xl:justify-between"
      >
        <div>
          <img
            class="w-[164px] md:w-[180px] 2xl:w-[223px]"
            src="~assets/images/logo.svg"
            width="223px"
            height="190px"
            alt="Logo Lola van Praag"
          />
        </div>
        <div
          class="mt-[50px] md:mt-[70px] md:grid md:grid-cols-2 md:w-full 2xl:mt-0 2xl:grid-cols-3"
        >
          <div class="md:grid md:grid-cols-2">
            <div
              class="font-serif font-light text-[24px] leading-[35px] text-center md:text-left md:w-[115px]"
            >
              Want to get in touch?
            </div>
            <div>
              <a
                class="block font-light leading-[32px] text-center md:text-left"
                href="mailto:info@lolavanpraag.com"
                >info@lolavanpraag.com</a
              >
            </div>
          </div>

          <div class="mt-[40px] md:mt-0 md:grid md:grid-cols-2">
            <div
              class="font-serif font-light text-[24px] leading-[35px] text-center md:text-left md:w-[115px]"
            >
              Find my work at the following gallery
            </div>
            <div>
              <a
                class="block font-light leading-[32px] text-center md:text-left"
                href="https://www.rademakersgallery.com/"
                target="_blank"
                rel="nofollow noreferrer noopener"
              >
                Rademarkers Gallery
              </a>
            </div>
          </div>

          <div class="mt-[40px] md:mt-0 md:grid md:grid-cols-2">
            <div
              class="font-serif font-light text-[24px] leading-[35px] text-center md:text-left md:w-[115px]"
            >
              Follow Lola on
            </div>
            <div>
              <a
                class="block font-light leading-[32px] text-center md:text-left"
                href="https://www.instagram.com/lolavanpraag/"
                target="_blank"
                rel="nofollow noreferrer noopener"
              >
                Instagram
              </a>
              <a
                class="block font-light leading-[32px] text-center md:text-left"
                href="https://www.linkedin.com/in/lola-van-praag/"
                target="_blank"
                rel="nofollow noreferrer noopener"
                >LinkedIn</a
              >
            </div>
          </div>
        </div>
      </div>

      <div
        class="mt-[50px] pt-[50px] border-t border-[#F941CB] flex flex-col items-center md:mt-[40px] md:pt-[40px] md:flex-row md:justify-between md:items-end 2xl:mt-[100px] 2xl:pt-[10.5px]"
      >
        <div
          class="flex flex-col w-full md:flex-row md:items-end md:w-auto 2xl:ml-[330.5px]"
        >
          <div
            class="font-serif font-light text-[24px] leading-[35px] text-center md:inline-block md:text-left md:w-[115px]"
          >
            Join my mailinglist
          </div>
          <div class="md:inline-block md:ml-[30px] md:w-[345px]">
            <subscribe />
          </div>
        </div>
        <div class="mt-[50px] font-light text-[12px] leading-[17px] md:mt-0">
          &copy; {{ currentYear }} Lola van Praag
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  computed: {
    currentYear() {
      return new Date().getFullYear();
    },
  },
};
</script>
