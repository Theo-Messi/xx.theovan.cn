<template>
  <footer class="bg-alt f12 lh-normal" style="text-align: center; margin: 0 auto">
    <div class="flex flex-grow-1 ma4" style="display: flex; justify-content: center; width: 100%">
      <!-- GitHub Source -->
      <div class="fb6">
        <div class="mb2 fw6 f14">GitHub Source</div>
        <ul>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://github.com/Theo-messi/Theo-Docs">Theo-Docs</a>
          </li>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://github.com/Theo-messi/xx.theovan.cn">玄学宝典</a>
          </li>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://github.com/Theo-messi/share.theovan.cn"
              >阿里云盘资源分享</a
            >
          </li>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://github.com/Theo-Messi/dotfiles">常用配置文件</a>
          </li>
        </ul>
      </div>
      <!-- 合作伙伴 -->
      <div class="fb6">
        <div class="mb2 fw6 f14">合作伙伴</div>
        <ul>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://nf.video/kaIuE">银河录像局</a>
          </li>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://ihezu.love/UKTer6">奈飞小铺</a>
          </li>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://fbinv01.fbaff.cc/auth/register?code=RZP3"
              >FlyingBird</a
            >
          </li>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://patriot.ninja/aff.php?aff=1471">Bridge The Wise</a>
          </li>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://sms-activate.org/?ref=8170513">SMS-Activate</a>
          </li>
        </ul>
      </div>
      <!-- 观影指南 -->
      <div class="fb6">
        <div class="mb2 fw6 f14">观影指南</div>
        <ul>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://doc.theovan.cn/streaming/Netflix-guide">Netflix</a>
          </li>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://doc.theovan.cn/streaming/Disney-introduce"
              >Disney+</a
            >
          </li>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://doc.theovan.cn/streaming/Spotify">Spotify Premium</a>
          </li>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://doc.theovan.cn/streaming/YouTube">YouTube Premium</a>
          </li>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://doc.theovan.cn/streaming/Hulu">Hulu</a>
          </li>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://doc.theovan.cn/streaming/HBO-Max">HBO Max</a>
          </li>
        </ul>
      </div>
      <!-- 友情链接 -->
      <div class="fb6">
        <div class="mb2 fw6 f14">相关链接</div>
        <ul>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://doc.theovan.cn/">Theo-Docs</a>
          </li>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://xx.theovan.cn/">玄学宝典</a>
          </li>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://share.theovan.cn/">阿里云盘资源分享</a>
          </li>
          <li class="mb2">
            <a class="external-link" target="_blank" href="https://vitepress.dev/">VitePress</a>
          </li>
        </ul>
      </div>
    </div>

    <!-- 底部信息栏 -->
    <div class="flex" style="display: inline-block">
      <span class="ml1">
        <a target="_blank" href="https://beian.miit.gov.cn/">
          <i class="fas fa-earth-americas" style="margin-right: 4px"></i>鄂ICP备2024060426号</a
        >
      </span>
      <span class="ml1">
        <a target="_blank" href="https://beian.mps.gov.cn/">
          <i class="fas fa-shield" style="margin-right: 4px"></i>粤公网安备44200102445439号</a
        >
      </span>
    </div>
    <div class="flex ma4" style="display: inline-block">
      <span class="ml1">
        Copyright <i class="far fa-copyright"></i> 2019 - {{ new Date().getFullYear() }}
        <a target="_blank" href="https://github.com/Theo-messi">Theo-Messi</a>. All Rights Reserved
      </span>
    </div>
  </footer>
</template>
<style lang="scss" scoped>
/* 页脚 */
footer {
  width: 100%;

  a:hover {
    -webkit-text-decoration: underline dotted;
    text-decoration: underline dotted;
  }

  .has-sidebar ~ & {
    display: none;
  }
}

.external-link {
  position: relative;
  display: inline-block;
  padding-right: 10px;

  &::after {
    content: '\f061';
    font-family: 'Font Awesome 6 Free';
    font-weight: 900;
    font-size: 0.5rem;
    position: absolute;
    color: var(--vp-c-text-3);
    transform: rotate(-45deg);
  }
}

.bg-alt {
  background: var(--vp-c-bg-alt);
}

.lh-normal {
  line-height: normal;
}

.flex {
  display: flex;

  &-grow-1 {
    flex-grow: 1;
  }
}

.ma4 {
  margin: 1.5rem;
}

.ma2 {
  margin: 1rem;
}

.ml0 {
  margin-left: 0.5rem;
}

.ml1 {
  margin-left: 1rem;
}

.mb2 {
  margin-bottom: 0.5rem;
}

.f12 {
  font-size: 12px;
}

.f14 {
  font-size: 13px;
}

.fw6 {
  font-weight: 600;
}

.fb6 {
  flex-basis: 20rem;
}

@media screen and (min-width: 960px) {
  .flex-l {
    display: flex;
  }
}

@media screen and (max-width: 768px) {
  .ma4 {
    margin-left: auto; /* 左边距自动 */
    margin-right: auto; /* 右边距自动 */
    width: 100%; /* 宽度100% */
    max-width: 95%; /* 最大宽度为屏幕宽度的95% */
  }
}
</style>
