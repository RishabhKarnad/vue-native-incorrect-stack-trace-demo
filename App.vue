<script>
export default {
  data() {
    return {
      message: 'Hello',
    };
  },
  methods: {
    p() {
      this.message += '!';
    },
  },
  mounted() {
    function t() {
      throw new Error('Mock error');
    }
    t();
    console.log(10 < 20);
  },
};
</script>

<template>
  <view class="container">
    <text class="text-color-primary">My Vue Native App</text>
    <text class="text-color-primary">{{ message }}</text>
    <button title="Press" @press="p" />
  </view>
</template>

<style>
.container {
  background-color: white;
  align-items: center;
  justify-content: center;
  flex: 1;
}
.text-color-primary {
  color: blue;
}
</style>
