<template>
  <div
    class="container mx-auto px-[17.5px] md:px-[30px] xl:grid xl:grid-cols-5 xl:px-[55px]"
  >
    <div class="xl:col-span-3 xl:pl-[120px]">
      <div class="grid grid-cols-20">
        <div class="mt-[23px] col-span-12">
          <img
            class="w-full"
            src="/images/instagram/instagram-1.jpg"
            alt=""
            width="400"
            height="400"
            loading="lazy"
          />
        </div>
        <div class="col-span-7 ml-auto col-start-14">
          <img
            class="w-full"
            src="/images/instagram/instagram-2.jpg"
            alt=""
            width="250"
            height="250"
            loading="lazy"
          />
          <div class="mt-[14px]">
            <img
              class="w-full"
              src="/images/instagram/instagram-3.jpg"
              alt=""
              width="250"
              height="250"
              loading="lazy"
            />
          </div>
        </div>
      </div>
      <div class="mt-[20px] md:mt-[37px] md:ml-[109px]">
        <h2
          class="font-extralight text-[20px] leading-[28px] md:ml-[28px] md:font-thin md:text-[40px] md:leading-[80px]"
        >
          Follow me
        </h2>
        <div
          class="mt-[10px] font-serif font-light text-electric-pink text-[40px] leading-[35px] md:text-[70px] md:leading-[80px]"
        >
          @lolavanpraag
        </div>
        <a
          href="https://www.instagram.com/lolavanpraag/"
          target="_blank"
          rel="nofollow noreferrer noopener"
          class="block mt-[20px] ml-[20px] md:mt-[40px] md:ml-[30px]"
        >
          <img
            class="inline-block"
            src="~assets/images/arrow.svg"
            width="18px"
            height="14px"
            alt=""
          />
          <div
            class="inline-block ml-[29px] leading-[22px] lowercase md:text-[18px] md:leading-[24px]"
          >
            Follow me
          </div>
        </a>
      </div>
    </div>

    <div
      class="hidden xl:grid xl:grid-cols-2 xl:col-span-2 xl:grid-rows-2 xl:ml-[30px]"
    >
      <div class="mt-auto">
        <img
          class="w-full"
          src="/images/instagram/instagram-4.jpg"
          alt=""
          width="250"
          height="250"
          loading="lazy"
        />
      </div>
      <div class="col-span-2 row-span-2 mt-[30px]">
        <img
          class="w-full"
          src="/images/instagram/instagram-5.jpg"
          alt=""
          width="450"
          height="450"
          loading="lazy"
        />
      </div>
    </div>
  </div>
</template>

<style scoped>
.grid-cols-20 {
  grid-template-columns: repeat(20, minmax(0, 1fr));
}

.col-start-14 {
  grid-column-start: 14;
}
</style>
