<template>
  <div class="body" ref="mybody" :style="{'height':'800px'}">
    <div class="box">
      <span class="box1">
        <img src="../../public/img/download_pattern_left (1).png" alt />
      </span>
      <span class="box2">
        <img src="../../public/img/download_pattern_right.png" alt />
      </span>
    </div>
    <div class="title">秀动</div>
    <p class="detail">看现场演出听原创音乐的专业移动票务平台</p>
    <button class="btn" onclick="Xz()">下载安装</button>
  </div>
</template>
<script>

export default {
  mounted () {
    // this.$refs.mybody.style.height = window.innerHeight
    console.log(this.$refs.mybody.style.height)
  }
}
</script>
<style lang="scss" scoped>
// * {
//   margin: 0;
//   padding: 0;
// }
// div {
//   display: block;
// }
.body {
  background: url("/img/bg.jpg") no-repeat;
  background-size: 100%;
  font-size: 0.16rem;
}
.box {
  width: 100%;
  height: 3.3rem;
}
.box1 {
  position: absolute;
  left: -0.08rem;
}
.box2 {
  position: absolute;
  right: -0.08rem;
}
.box1 img {
  width: 0.9rem;
}
.box2 img {
  width: 0.9rem;
}

.title {
  position: absolute;
  width: 70%;
  left: 15%;
  top: 2.3rem;
  text-align: center;
  font-size: 0.24rem;
  padding-bottom: 0.2rem;
}
.detail {
  position: absolute;
  top: 3.5rem;
  text-align: center;
  color: #bbb;
  left: 12%;
  font-size: 0.16rem;
}

.btn {
  position: absolute;
  left: 20%;
  top: 4.5rem;
  width: 60%;
  height: 0.44rem;
  color: #ffffff;
  font-size: 0.16rem;
  background: #32b2a7;
  border-radius: 0.25rem;
  border: 0.01rem solid #e1e1e1;
}
</style>
