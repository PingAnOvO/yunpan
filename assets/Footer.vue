<template>
  <footer class="footer">
    <div class="icons">
      <a :href="telegramUrl" target="_blank" rel="noopener noreferrer" class="icon-link" title="Telegram">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 496 512"><path d="M248 8C111 8 0 119 0 256S111 504 248 504 496 393 496 256 385 8 248 8zM363 176.7c-3.7 39.2-19.9 134.4-28.1 178.3-3.5 18.6-10.3 24.8-16.9 25.4-14.4 1.3-25.3-9.5-39.3-18.7-21.8-14.3-34.2-23.2-55.3-37.2-24.5-16.1-8.6-25 5.3-39.5 3.7-3.8 67.1-61.5 68.3-66.7 .2-.7 .3-3.1-1.2-4.4s-3.6-.8-5.1-.5q-3.3 .7-104.6 69.1-14.8 10.2-26.9 9.9c-8.9-.2-25.9-5-38.6-9.1-15.5-5-27.9-7.7-26.8-16.3q.8-6.7 18.5-13.7 108.4-47.2 144.6-62.3c68.9-28.6 83.2-33.6 92.5-33.8 2.1 0 6.6 .5 9.6 2.9a10.5 10.5 0 0 1 3.5 6.7A43.8 43.8 0 0 1 363 176.7z"/></svg>
      </a>
      <a :href="musicUrl" target="_blank" rel="noopener noreferrer" class="icon-link" title="音乐">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path d="M499.1 6.3c8.1 6 12.9 15.6 12.9 25.7l0 72C496 97.1 481.1 96 466 96C345.4 96 249.7 186.9 237.3 303.7c-9.7-5.7-20.8-9-32.7-9c-20.6 0-39 9-51.7 23l0-77.4c0-10.1 4.8-19.7 12.9-25.7l62.5-46.2 0-49.8c0-14.4-9.3-27-22.8-30.7L233.1 4.8C231 4.3 228.9 4 226.8 4c-12.8 0-24.1 7.6-29.9 18.7L146.3 136.3 59.8 95.7c-1.9-.9-4-1.6-6-2.2C41.8 88.1 32 75.7 32 61.1C32 42.5 48.9 28 68.3 31.7l187.6 46.1c12.8 3.2 22.1 15 22.1 28.3l0 55.3 62.5-46.2c8.1-6 12.9-15.6 12.9-25.7l0-72c0-10.1-4.8-19.7-12.9-25.7s-18.9-7.5-28.8-4.2L243.1 33.4C241 34 239 34.8 237.1 35.7L149.6 73.1 70.3 7.8C63.6 2.9 55.3 0 46.8 0C21.2 0 0 21.2 0 47.2c0 17.2 9.2 32.9 24.1 41.4l96 48 80.1 40.1 0 44.6c-10.2-2.5-20.9-3.9-32-3.9C57.3 224 0 281.3 0 352s57.3 128 128 128c65.3 0 119.1-48.9 127-112l257-75.8c16.9-5 28.8-20.4 28.8-38.1l0-144c0-10.1-4.8-19.7-12.9-25.7s-18.9-7.5-28.8-4.2L528 62.2C528 48.7 517.7 37 504.6 37.5l-3.9 .2c-1.1 0-2.2 .2-3.3 .4L355.8 77.5 279 33.8c-8.1-6-18.9-7.5-28.8-4.2L179.8 46.1c-1.1 .3-2.1 .7-3.1 1.1l-3.4 1.7L66.4 4.8C58.3-1.1 48-3.9 37.8-2.2S18.8 7.6 12.9 15.7s-7.5 18.9-4.2 28.8L46.1 179.8c3.2 9.9 12.4 17.5 22.9 19.2s21.1-1.9 28.1-9.1l46.2-62.5 49.8 0c13.3 0 25.1-9.3 28.3-22.1l46.1-187.6c3.2-9.9 12.4-17.5 22.9-19.2s21.1 1.9 28.1 9.1l62.5 46.2 72 0c10.1 0 19.7 4.8 25.7 12.9zM128 448a96 96 0 1 0 0-192 96 96 0 1 0 0 192z"/></svg>
      </a>
      <a :href="tvUrl" target="_blank" rel="noopener noreferrer" class="icon-link" title="电视TV">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512"><path d="M64 64V352H576V64H64zM0 64C0 28.7 28.7 0 64 0H576c35.3 0 64 28.7 64 64V352c0 35.3-28.7 64-64 64H64c-35.3 0-64-28.7-64-64V64zM128 448H512c17.7 0 32 14.3 32 32s-14.3 32-32 32H128c-17.7 0-32-14.3-32-32s14.3-32 32-32z"/></svg>
      </a>
      <a :href="emailUrl" target="_blank" rel="noopener noreferrer" class="icon-link" title="邮箱">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path d="M48 64C21.5 64 0 85.5 0 112c0 15.1 7.1 29.3 19.2 38.4L236.8 313.6c11.4 8.5 27 8.5 38.4 0L492.8 150.4c12.1-9.1 19.2-23.3 19.2-38.4c0-26.5-21.5-48-48-48L48 64zM0 176L0 384c0 35.3 28.7 64 64 64l384 0c35.3 0 64-28.7 64-64l0-208L294.4 339.2c-22.8 17.1-54 17.1-76.8 0L0 176z"></path></svg>
      </a>
    </div>

    <div class="stats">
      访问次数：<span id="vercount_value_site_pv">😯</span>次 | 访客人数：<span id="vercount_value_site_uv">😯</span>人
    </div>

    <div style="margin:10px 0;">© 2025 恶霸PD. All rights reserved.</div>
  </footer>
</template>

<script>
export 默认 {
  name: "Footer"，
  data() {
    return {
      telegramUrl: "https://t.me/+50935318069",
      musicUrl: "https://wyy.pdovo.dpdns.org",
      tvUrl: "https://tv.pdovo.ggff.net",
      emailUrl: "mailto:pinganoxo@gmail.com"
    };
  }
};
</script>

<style scoped>
.footer {
  margin-top: 30px;
  text-align: center;
  padding: 20px;
  background-color: #ffffff77;
  font-size: 16px;
  border-radius: 50% 50% 0 0;
}

.icons {
  display: flex;
  justify-content: center;
  gap: 16px;
  margin-bottom: 25px;
}

.icon-link {
  width: 28px;
  height: 28px;
  display: inline-block;
  fill: #2c2c2c;
  transition: fill 0.3s, transform 0.3s;
}

.icon-link:hover {
  fill: #444;
  transform: scale(1.1);
}

.stats {
  margin: 10px 0;
  color: #444;
}
</style>
