<template>
  <view class="w-[100vw] h-[100vh]">
    <swiper
      class="demo-swiper"
      :circular="true"
      previous-margin="60px"
      next-margin="60px"
      @transition="onTransition"
    >
      <swiper-item>
        <view class="demo-swiper-item">
          <view class="demo-swiper-box demo-swiper-box-red">
            Red
          </view>
        </view>
      </swiper-item>
      <swiper-item>
        <view class="demo-swiper-item">
          <!-- 将这里的注释解除掉, 出现bug -->
          <!-- <view class="demo-swiper-box demo-swiper-box-green"> -->
          Green
          <!-- </view> -->
        </view>
      </swiper-item>
      <swiper-item>
        <view class="demo-swiper-item">
          <!-- <view class="demo-swiper-box demo-swiper-box-blue"> -->
          Blue
          <!-- </view> -->
        </view>
      </swiper-item>
    </swiper>
  </view>
</template>

<script setup lang="ts">

const onTransition = (e) => {
  console.log(e)
}

</script>

<style>

.demo-swiper {
  width: 100%;
  height: 30vh;
}

.demo-swiper-item {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.demo-swiper-box {
  width: 80%;
  height: 100%;
}

.demo-swiper-box-red {
  background-color: red;
}

.demo-swiper-box-green {
  background-color: green;
}

.demo-swiper-box-blue {
  background-color: blue;
}

</style>
