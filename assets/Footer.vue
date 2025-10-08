<template>
  <footer class="footer">
    <div class="icons">
      <!-- Telegram -->
      <a href="https://t.me/+50935318069" target="_blank" rel="noopener noreferrer" class="icon-link" title="Telegram">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 496 512">
          <path d="M248,8C111.033,8,0,119.033,0,256s111.033,248,248,248,248-111.033,248-248S384.967,8,248,8Zm121.7,169.5-40.7,191c-3.1,14.1-11.3,17.6-22.9,10.9l-63.5-46.8-30.6,29.5c-3.4,3.4-6.2,6.2-12.7,6.2l4.6-65.3,118.9-107.4c5.2-4.6-1.1-7.2-8.1-2.6L176,281.4l-63.2-19.8c-13.7-4.3-14-13.7,2.9-20.4l246.9-95C374.3,141.7,376.3,142.8,369.7,177.5Z"/>
        </svg>
      </a>

      <!-- 邮箱 -->
      <a href="mailto:pinganoxo@gmail.com" target="_blank" rel="noopener noreferrer" class="icon-link" title="邮箱">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">
          <path d="M48 64C21.5 64 0 85.5 0 112c0 15.1 7.1 29.3 19.2 38.4L236.8 313.6c11.4 8.5 27 8.5 38.4 0L492.8 150.4c12.1-9.1 19.2-23.3 19.2-38.4c0-26.5-21.5-48-48-48L48 64zM0 176L0 384c0 35.3 28.7 64 64 64l384 0c35.3 0 64-28.7 64-64l0-208L294.4 339.2c-22.8 17.1-54 17.1-76.8 0L0 176z"/>
        </svg>
      </a>

      <!-- 音乐 -->
      <a href="https://wyy.pdovo.dpdns.org" target="_blank" rel="noopener noreferrer" class="icon-link" title="音乐">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">
          <path d="M511.99,32v384c0,53.02-42.98,96-96,96H96c-53.02,0-96-42.98-96-96V32C0,14.33,14.33,0,32,0h448C497.67,0,512,14.33,512,32z M96,448h320c17.67,0,32-14.33,32-32V96H64v320C64,433.67,78.33,448,96,448z"/>
        </svg>
      </a>

      <!-- 电视 -->
      <a href="https://tv.pdovo.ggff.net" target="_blank" rel="noopener noreferrer" class="icon-link" title="电视">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512">
          <path d="M592 0H48C21.49 0 0 21.49 0 48v352c0 26.51 21.49 48 48 48h544c26.51 0 48-21.49 48-48V48C640 21.49 618.51 0 592 0zM576 384H64V64h512v320zm-64 96H128c-17.67 0-32 14.33-32 32v32h448v-32c0-17.67-14.33-32-32-32z"/>
        </svg>
      </a>
    </div>

    <div class="stats">
      访问次数：<span id="site_pv">加载中...</span> 次 |
      访客人数：<span id="site_uv">加载中...</span> 人
    </div>

    <div class="powered">
      Powered by <a href="https://workers.cloudflare.com/" target="_blank" rel="noopener noreferrer">Cloudflare Workers</a>
    </div>

    <div style="margin-top:10px;">© 2025 PingAn. All rights reserved.</div>
  </footer>
</template>

<script>
export 默认 {
  name: "Footer"，
  mounted() {
    // 使用 countapi 统计访问次数
    const pvKey = "yunpan_pingan_pv";
    const uvKey = "yunpan_pingan_uv";

    // 访问次数
    fetch(`https://api.countapi.xyz/hit/pingan/${pvKey}`)
      。键，然后(res => res.json())
      。键，然后(data => {
        document.getElementById("site_pv")。innerText = data.value;
      })
      。catch(() => {
        document.getElementById("site_pv")。innerText = "❌";
      });

    // 访客人数
    fetch(`https://api.countapi.xyz/hit/pingan/${uvKey}`)
      .then(res => res.json())
      .then(data => {
        document.getElementById("site_uv").innerText = data.value;
      })
      .catch(() => {
        document.getElementById("site_uv").innerText = "❌";
      });
  },
};
</script>

<style scoped>
.footer {
  margin-top: 30px;
  text-align: center;
  padding: 20px;
  background-color: #ffffff90;
  font-size: 16px;
  border-radius: 50% 50% 0 0;
}

.icons {
  display: flex;
  justify-content: center;
  gap: 20px;
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
  fill: #000;
  transform: scale(1.1);
}

.stats {
  margin: 10px 0;
  color: #333;
}

.powered {
  margin-top: 10px;
  color: #444;
}

.powered a {
  color: #444;
  text-decoration: none;
}

.powered a:hover {
  color: #000;
}
</style>
