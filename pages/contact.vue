<template>
  <div class="bg-apple-green">
    <meta-tags :title="title" :description="description" />
    <div
      class="container mx-auto pt-[86px] pb-[100px] px-[17.5px] md:px-[30px] md:pt-[165px] md:pb-[112px] 2xl:px-[55px]"
    >
      <breadcrumbs :breadcrumbs="breadcrumbs" color="#A3A3A3" />
      <h1
        class="mt-[20px] font-serif font-light text-[32px] leading-[32px] md:text-[90px] md:leading-[80px]"
      >
        Contact
      </h1>

      <div class="mt-[50px] xl:grid xl:grid-cols-2 xl:mt-[80px]">
        <div class="md:grid md:grid-cols-2">
          <div
            class="font-serif font-light text-[24px] leading-[35px] md:w-[180px]"
          >
            Want to get in touch?
          </div>
          <div class="mt-[10px] md:mt-0">
            <a
              class="block font-light leading-[32px] md:text-[20px] md:leading-[40px]"
              href="mailto:info@lolavanpraag.com"
              >info@lolavanpraag.com</a
            >
          </div>
        </div>
        <div class="mt-[50px] md:grid md:grid-cols-2 xl:mt-0">
          <div
            class="font-serif font-light text-[24px] leading-[35px] md:w-[180px]"
          >
            Follow Lola on
          </div>
          <div class="mt-[10px] md:mt-0">
            <a
              class="block font-light leading-[32px] md:text-[20px] md:leading-[40px]"
              href="https://www.instagram.com/lolavanpraag/"
              target="_blank"
              rel="nofollow noreferrer noopener"
            >
              Instagram
            </a>
            <a
              class="block font-light leading-[32px] md:text-[20px] md:leading-[40px]"
              href="https://www.linkedin.com/in/lola-van-praag/"
              target="_blank"
              rel="nofollow noreferrer noopener"
              >LinkedIn</a
            >
          </div>
        </div>
      </div>

      <div
        class="border-t border-[#97D039] mt-[25.5px] pt-[24.5px] md:grid md:grid-cols-2 md:mt-[50px] md:pt-[50px] 2xl:grid-cols-4"
      >
        <div
          class="font-serif font-light text-[24px] leading-[35px] md:w-[180px]"
        >
          Find my work at the following gallery
        </div>
        <div class="mt-[10px] md:mt-0">
          <a
            class="block font-light leading-[32px] md:text-[20px] md:leading-[40px]"
            href="https://www.rademakersgallery.com/"
            target="_blank"
            rel="nofollow noreferrer noopener"
          >
            Rademarkers Gallery
          </a>
        </div>
      </div>

      <div
        class="border-t border-[#97D039] mt-[24.5px] pt-[25.5px] md:mt-[50px] md:pt-[50px]"
      >
        <h2 class="font-serif font-light text-[24px] leading-[35px]">
          Shoot me a message!
        </h2>
        <form
          class="mt-[20px] md:mt-[40px]"
          name="Contactformulier"
          method="POST"
          data-netlify="true"
        >
          <input type="hidden" name="form-name" value="Contactformulier" />
          <div class="md:grid md:grid-cols-2 md:gap-x-[113px]">
            <input
              class="block w-full pb-[17px] pl-[20px] bg-apple-green border-b border-black font-light text-[14px] leading-[19px] placeholder-black rounded-none outline-none focus:border-electric-pink focus:placeholder-[#62822D]"
              type="text"
              name="fname"
              placeholder="First name*"
            />
            <input
              class="block w-full mt-[40px] pb-[17px] pl-[20px] bg-apple-green border-b border-black font-light text-[14px] leading-[19px] placeholder-black rounded-none outline-none focus:border-electric-pink focus:placeholder-[#62822D] md:mt-0"
              type="text"
              name="lname"
              placeholder="Last name*"
            />
            <input
              class="block w-full mt-[40px] pb-[17px] pl-[20px] bg-apple-green border-b border-black font-light text-[14px] leading-[19px] placeholder-black rounded-none outline-none focus:border-electric-pink focus:placeholder-[#62822D] md:mt-[60px]"
              type="email"
              name="email"
              placeholder="E-mail address*"
            />
            <input
              class="block w-full mt-[40px] pb-[17px] pl-[20px] bg-apple-green border-b border-black font-light text-[14px] leading-[19px] placeholder-black rounded-none outline-none focus:border-electric-pink focus:placeholder-[#62822D] md:mt-[60px]"
              type="tel"
              name="phone"
              placeholder="Telephone number*"
            />
            <input
              class="block w-full mt-[40px] pb-[17px] pl-[20px] bg-apple-green border-b border-black font-light text-[14px] leading-[19px] placeholder-black rounded-none outline-none focus:border-electric-pink focus:placeholder-[#62822D] md:mt-[60px]"
              type="text"
              name="subject"
              placeholder="Subject"
            />
            <input
              class="block w-full mt-[40px] pb-[17px] pl-[20px] bg-apple-green border-b border-black font-light text-[14px] leading-[19px] placeholder-black rounded-none outline-none focus:border-electric-pink focus:placeholder-[#62822D] md:row-start-4 md:mt-[60px]"
              type="textarea"
              name="comment"
              placeholder="Comment*"
            />
          </div>
          <button
            class="mt-[50px] bg-electric-pink h-[60px] px-[62px] lowercase md:mt-[60px]"
            type="submit"
          >
            Send
          </button>
        </form>
      </div>
    </div>
    <marquee class="sticky bottom-0" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      breadcrumbs: [
        { name: "Home", link: "/" },
        { name: "Contact", link: "/contact" },
      ],
      title: "Contact",
      description:
        "Want to get in touch? Fill out the contact form  or follow our accounts on social media.",
    };
  },
};
</script>
