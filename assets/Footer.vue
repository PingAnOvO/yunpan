<template>
  <footer class="footer">
    <div class="icons">
      <a href="https://t.me/+50935318069" target="_blank" rel="noopener noreferrer" class="icon-link" title="Telegram">
        <svg viewBox="0 0 24 24"><path d="M9.93 15.57l-.39 3.72c.56 0 .8-.24 1.09-.52l2.62-2.47 5.43 3.96c1 .56 1.71.27 1.97-.92l3.57-16.73c.33-1.51-.56-2.1-1.52-1.74L1.08 9.63C-.42 10.21-.4 11 .79 11.33l4.43 1.38L19.1 5.26c.66-.4 1.26-.18.77.25"/></svg>
      </a>
      <a href="mailto:pinganoxo@gmail.com" class="icon-link" title="邮箱">
        <svg viewBox="0 0 512 512"><path d="M48 64C21.5 64 0 85.5 0 112c0 15.1 7.1 29.3 19.2 38.4L236.8 313.6c11.4 8.5 27 8.5 38.4 0L492.8 150.4c12.1-9.1 19.2-23.3 19.2-38.4c0-26.5-21.5-48-48-48L48 64zM0 176L0 384c0 35.3 28.7 64 64 64l384 0c35.3 0 64-28.7 64-64l0-208L294.4 339.2c-22.8 17.1-54 17.1-76.8 0L0 176z"/></svg>
      </a>
      <a href="https://wyy.pdovo.dpdns.org" target="_blank" rel="noopener noreferrer" class="icon-link" title="音乐">
        <svg viewBox="0 0 24 24"><path d="M9 17a3 3 0 1 0 2.83 2H19V5h-2v8.12A3.001 3.001 0 0 0 9 17Z"/></svg>
      </a>
      <a href="https://tv.pdovo.ggff.net" target="_blank" rel="noopener noreferrer" class="icon-link" title="电视">
        <svg viewBox="0 0 24 24"><path d="M4 6h16v10H4V6zm0 12h16v2H4v-2zm8-14l4 4H8l4-4z"/></svg>
      </a>
    </div>

    <div style="margin-top:10px;">© 2025 PingAn. All rights reserved.</div>
  </footer>
</template>

<script>
export 默认 {
  name: "Footer"
};
</script>

<style scoped>
.footer {
  margin-top: 30px;
  text-align: center;
  padding: 20px;
  background: rgba(255,255,255,0.7);
  font-size: 16px;
  border-radius: 50% 50% 0 0;
}
.icons {
  display: flex;
  justify-content: center;
  gap: 16px;
  margin-bottom: 20px;
}
.icon-link {
  width: 28px;
  height: 28px;
  fill: #333;
}
</style>
