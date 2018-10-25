<template>
    <div class="profile-header lite-bot-line">
        <div class="prf-detail m-avatar-box m-box">
            <div class="m-img-box">
                <img src="https://tvax3.sinaimg.cn/crop.25.0.518.518.180/9c590277ly8fhimdyw3ubj20go0eewfl.jpg" />
            </div>
 
            <div class="m-box-col m-box-dir m-box-center">
                <h3>{{ userName }}</h3>
            </div>
        </div>

        <div class="m-box">
            <div class="number-box">
                <h3>微博</h3>
            </div>
            <div class="number-box">
                <h3>关注</h3>
            </div>
            <div class="number-box">
                <h3>粉丝</h3>
            </div>
        </div>

    </div>
</template>

<script>
export default {
  name: "Profile",
  props: {
    userName: String,
    userDetail: String,
    weiboAmount: Number,
    follower: Number,
    following: Number
  }
};
</script>

<style lang="less">

.m-box {
  display: flex;
}

.m-img-box ::before {
    position: absolute;
    z-index: 2;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    border: 1px solid rgba(0, 0, 0, 0.05);
    border-radius: 50%;
    border-color: hsla(0,0%,90%,.15);
}

.m-img-box {
      display: inline-block;
  object-fit: cover;
}

.m-avatar-box {
  border-radius: 50%;
  position: relative;
}

.profile-header {
  position: relative;
  background-repeat: no-repeat;
  background-position: 50%;
  background-size: cover;
  background: #fff;
}

.lite-bot-line {
  border-top-width: 0;
  border-right-width: 0;
  border-bottom-width: 1px;
  border-left-width: 0;
  border-color: #e6e6e6;
  border-style: solid;
}

.number-box {
    margin-right: 10rem;
    cursor: pointer;
}

.profile-header.prf-detail .m-img-box {
    width: 4rem;
    height: 4rem;
    margin-right: .9375rem;
}
</style>
