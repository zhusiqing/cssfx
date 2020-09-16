<template>
  <div ref="recommend" class="recommend">
    <a class="nicelinks" href="http://nicelinks.site/?utm_source=cssfx.lovejade.cn">
      <img
        class="qrcode"
        src="https://image.nicelinks.site/nicelinks-miniprogram-code-removebg-preview.png?imageView2/1/w/200/h/200/interlace/1/ignore-error/1"
        alt="倾城之链"
      />
      <div class="desc">
        <div>
          <p class="title"><strong>倾城之链</strong>，倾心缔造，痴心为你</p>
          <p>旨在云集全球优秀网站，探索互联网中更广阔的世界；</p>
        </div>
        <p>你可以轻松发现、学习、分享更多有用或有趣的事物。</p>
      </div>
    </a>
  </div>
</template>

<script>
export default {
  mounted() {
    this.$nextTick(() => {})
  }
}
</script>

<style>
.recommend {
  display: block;
  overflow: hidden;
  width: 520px;
  padding: 10px;
  margin: 0 auto;
  box-shadow: 0 1px 3px hsla(0, 0%, 0%, 0.05);
  border-radius: 4px;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell,
    'Helvetica Neue', Helvetica, Arial, sans-serif;
  line-height: 1.5;
  font-size: 12px;
  background-color: hsl(237, 37%, 24%);
  transform: scale(0.9);
}

.recommend .nicelinks {
  display: inline-block;
  height: 100px;
  color: inherit;
  text-decoration: none;
  display: flex;
}
.nicelinks .qrcode {
  width: 100px;
  height: 100px;
}
.nicelinks .desc {
  width: 400px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: space-between;
  letter-spacing: 2px;
  padding-left: 15px;
}
.title {
  font-size: 14px;
}

@media screen and (max-width: 768px) {
  .recommend {
    width: 100%;
  }
}
</style>
