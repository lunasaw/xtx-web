<template>
  <div>
    <ul>
      <base-brand-item v-for="(image, index) in imageList" :key="index" :image="image" @clickItem="itemClick"></base-brand-item>
    </ul>
  </div>
</template>

<script>
import BaseBrandItem from '@/components/BaseBrandItem.vue'

export default {
  data () {
    return {
      images: [
        {
          src: require('@/assets/images/hot1.png'),
          alt: "Image 1",
          link: "#"
        },
        {
          src: require('@/assets/images/hot2.png'),
          alt: "Image 2",
          link: "#"
        },
        {
          src: require('@/assets/images/hot3.png'),
          alt: "Image 3",
          link: "#"
        },
        {
          src: require('@/assets/images/hot4.png'),
          alt: "Image 4",
          link: "#"
        },
        {
          src: require('@/assets/images/hot5.png'),
          alt: "Image 5",
          link: "#"
        },
        // Add more image objects here
      ]
    };
  },
  components: {
    BaseBrandItem
  },
  computed: {
    imageList () {
      // 使用计算属性提取图片文件名并返回一个新的包含图片信息的数组
      return this.images.map(image => ({
        ...image,
        fileName: this.getImageFileName(image.src)
      }));
    }
  },
  methods: {
    itemClick (image) {
      // 处理图片点击事件
      console.log(image);
    },
    getImageFileName (src) {
      // 从 src 属性中提取文件名
      const pathSegments = src.split('/');
      return pathSegments[pathSegments.length - 1];
    }
  }
}
</script>

<style>
</style>