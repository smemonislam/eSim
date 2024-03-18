<template>
  <div class="brands">
    <div class="item" v-for="(image, index) in brandImages" :key="index">
      <img :src="image.src" :alt="image.alt" />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      brandImages: [
        { src: "img/image-1.png", alt: "Brand" },
        { src: "img/image-2.png", alt: "Brand" },
        { src: "img/image-3.png", alt: "Brand" },
        { src: "img/image-6.png", alt: "Brand" },
        { src: "img/image-5.png", alt: "Brand" },
        { src: "img/image-8.png", alt: "Brand" },
        { src: "img/image-9.png", alt: "Brand" },
        { src: "img/image-4.png", alt: "Brand" },
        { src: "img/image-10.png", alt: "Brand" },
      ],
    };
  },
};
</script>
