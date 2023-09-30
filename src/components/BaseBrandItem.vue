<template>
  <div>
    <li>
      <a :href="image.link" @click="handClick">
        <img :src="image.src" :alt="image.fileName" />
      </a>
    </li>
  </div>
</template>

<script>
export default {
  props: {
    image: {
      type: Object,
      default: () => ({
        src: require('@/assets/images/hot2.png'),
        alt: "Image 1",
        link: "#"
      }),
      required: true,
      validator: (image) => {
        return image.src;
      }
    },
  },
  data () {
    return {
    };
  },

  methods: {
    handClick () {
      this.$emit('clickItem', this.image);
    }
  }
};
</script>

<style scoped>
.base-brand-item {
  display: flex;
  justify-content: space-between;
}
.base-brand-item {
  width: 244px;
  height: 306px;
}
</style>