# Openlist新拟态戏法
新拟态之风盛行日久，然终不过是视觉骗术。世间美化仓库遍地，皆如"粉饰太平"之辈，涂抹颜色，堆砌阴影，自以为得计。唯独这一家"玄牝之司"，偏要装神弄鬼，弄出个什么"新拟态"来。

这"新拟态"，说来可笑。它既不是扁平的，又不完全是立体的；既要光，又要影，却不使人看清真面目。活像个"两面人"，站在光暗之交，左右逢源。更可笑的是，别人家的美化如同"绣花枕头"，只管外表光鲜。这厮却要"探囊取物"，深入OPENLIST五脏六腑，将那些"阴面"、"阳面"都算计得明明白白。它像个"偷窥者"，躲在前者内部，暗中观察每个元素的起承转合。

此仓库虽弄出新花样，终究也是「[以巧补拙](https://xodnytdcaw.feishu.cn/wiki/LXNDw3bCLiwpOdktmnOcV9mincc?fromScene=spaceOverview)」。

[TOC]




## 效果如下

![备用方案](https://cdnv2.ruguoapp.com/FvU4aZaInUkmkieAplYR8VrxxcPYv3.png)




## 使用方法

- **自定义头部**
（在后台设置-全局，找到自定义头部）

```XML
<style type="text/css">
body {
  /* 新拟态核心色调 */
  --neumorph-bg: #f0f0f3;
  --shadow-dark: rgba(163, 177, 198, 0.5);
  --shadow-light: rgba(255, 255, 255, 0.8);

  /* 仅修改背景部分（不影响 flex/布局） */
  background: var(--neumorph-bg) !important;
  background-image: none !important;  /* 确保无额外背景图干扰 */
  
  /* 纯背景新拟态（不干扰内容） */
  position: relative;  /* 确保背景覆盖完整 */
}

/* 添加一个伪元素作为背景层（避免影响内容布局） */
body::before {
  content: "";
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: -1;  /* 确保在底层 */
  
  /* 新拟态背景效果 */
  background: var(--neumorph-bg);
  box-shadow:
    inset 6px 6px 12px var(--shadow-dark),
    inset -6px -6px 12px var(--shadow-light);
}

/* 以下所有代码保持原样，不修改宽度、高度或布局 */
.markdown-body, 
.main-content {
  width: 100%;
  max-width: 800px;
  padding: 30px;
  margin: 0 auto;
  text-align: center;
}

.hope-c-PJLV-idaeksS-css,
.hope-c-hOYTCS,
.hope-c-PJLV-igScBhH-css {
  background: var(--neumorph-bg) !important;
  border-radius: 15px !important;
  box-shadow: 
    8px 8px 15px var(--shadow-dark),
    -8px -8px 15px var(--shadow-light) !important;
  border: none !important;
  transition: all 0.3s ease;
  padding: 15px 25px !important;
  margin: 10px auto !important;
  display: inline-block !important;
  cursor: pointer;
}

.markdown-body pre,
.hope-c-ctSAUo {
  background: var(--neumorph-bg) !important;
  box-shadow: 
    inset 3px 3px 5px var(--shadow-dark),
    inset -3px -3px 5px var(--shadow-light) !important;
  border-radius: 10px !important;
  padding: 15px !important;
  margin: 0 auto 20px !important;
  max-width: 90%;
}

.footer {
  text-align: center !important;
  margin-top: 30px;
  opacity: 1 !important;
}

.copyright {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

@media screen and (max-width: 960px) {
  body {
    padding: 10px;
  }
  
  .markdown-body,
  .main-content {
    padding: 15px;
    max-width: 95%;
  }
}
</style>
```

- **自定义内容**

```XML
<div id="customize" style="">

</div>
</center>
<br>
</center></div>
<!--延迟加载范围到这里结束-->
</div>

<!--延迟加载配套使用JS-->
<script>
    let interval = setInterval(() => {
        if (document.querySelector(".footer")) {
            document.querySelector("#customize").style.display = "";
            clearInterval(interval);
        }
    }, 100);
</script>

<!-- 移除了所有动态效果相关代码：烟花、小星星、樱花飘落、渐变背景、音乐增强 -->

<!---去掉底部文字--->
<style type="text/css"> .footer { display: none !important; } </style>
```

## 元数据

```XML
<div style="text-align: center; margin: 0 auto; max-width: 800px; padding: 20px;">
  <!-- 图片：强制居中 -->
  <img 
    src="https://mmbiz.qpic.cn/mmbiz_gif/gz2sdHyQbaZc0dIlEbMqjanFnBSmeLcww0YAecX8fuicqdUW4goZhMlKxhdaNzMDA9XgZD5CfffmqsEqkUibrySA/640?wx_fmt=gif&from=appmsg" 
    alt="小猫编程动图" 
    style="display: block; margin: 10px auto; max-width: 80%; border-radius: 8px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);"
  >

  <!-- 社交图标：增强型居中方案 -->
  <div style="
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    gap: 12px;
    margin: 30px auto;
    padding: 0 10px;
    width: 100%;
  ">
    <a href="https://blog.csdn.net/2402_82616859?type=blog" target="_blank" rel="noopener noreferrer" style="flex-shrink: 0;">
      <img src="https://img.shields.io/badge/📖_大强同学-FF4D4D?style=flat-square&logo=c&logoColor=white" alt="CSDN" style="max-height: 28px;">
    </a>
    <a href="https://twitter.com/dqtx760" target="_blank" rel="noopener noreferrer" style="flex-shrink: 0;">
      <img src="https://img.shields.io/badge/🐦_dqtx760-1DA1F2?style=flat-square&logo=x&logoColor=white" alt="Twitter" style="max-height: 28px;">
    </a>
    <a href="https://www.youtube.com/@dqtx760/videos" target="_blank" rel="noopener noreferrer" style="flex-shrink: 0;">
      <img src="https://img.shields.io/badge/🎬_dqtx760-FF0000?style=flat-square&logo=youtube&logoColor=white" alt="YouTube" style="max-height: 28px;">
    </a>
    <a href="https://xodnytdcaw.feishu.cn/wiki/BtjSwIjMuiISo7kNFiQcMMXcnKc?fromScene=spaceOverview" target="_blank" rel="noopener noreferrer" style="flex-shrink: 0;">
      <img src="https://img.shields.io/badge/📚_教程合集-00A1E9?style=flat-square&logo=feishu&logoColor=white" alt="飞书文档" style="max-height: 28px;">
    </a>
    <a href="https://bento.me/dqtx" target="_blank" rel="noopener noreferrer" style="flex-shrink: 0;">
      <img src="https://img.shields.io/badge/🍱_Bento-FFDD54?style=flat-square&logo=bento&logoColor=black" alt="Bento" style="max-height: 28px;">
    </a>
    <a href="https://github.com/dqtx760" target="_blank" rel="noopener noreferrer" style="flex-shrink: 0;">
      <img src="https://img.shields.io/badge/💻_GitHub-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub" style="max-height: 28px;">
    </a>
    <!-- 新增Linktree链接 -->
    <a href="https://link3.cc/dqtx760" target="_blank" rel="noopener noreferrer" style="flex-shrink: 0;">
      <img src="https://img.shields.io/badge/🔗_Linktree-39E09B?style=flat-square&logo=linktree&logoColor=white" alt="Linktree" style="max-height: 28px;">
    </a>
  </div>

  <!-- 文艺文字：居中优雅显示 -->
  <p style="
    font-family: 'Ma Shan Zheng', 'Noto Sans SC', sans-serif;
    font-size: 1.4rem;
    color: #5c5c5c;
    margin: 30px 0;
    line-height: 1.8;
    letter-spacing: 1px;
    text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
  ">
<strong>人间忽晚，山河已秋。 <span style="color: red;">技术支持微信：dqtx33</span></strong>
</p>
<div id="customize" style="">
                        </a >
                    </span>
                </span>
        <center class="dibu">
            <div style="font-size: 13px; font-weight: bold;">
                             <span class="nav-item">
                    <a class="nav-link" href="https://space.bilibili.com/491358682/upload/video0" target="_blank">
                        <i class="fa-duotone fa-envelope-open" style="color:#409EFF" aria-hidden="true">
                        </i>
                        B站 |
                    </a >
                </span>
                <!--后台入口-->
                <span class="nav-item">
                    <a class="nav-link" href="/@manage">
                        <i class="fa-solid fa-folder-gear" style="color:#409EFF;" aria-hidden="true">
                        </i>
                        管理 |
                    </a >
                </span>
                <span class="nav-item">
                    <a class="nav-link" href="/" target="_blank">
                        <i class="fas fa-edit" style="color:#409EFF" aria-hidden="true">
                        </i>
                        主页 
                    </a >
                </span>
                
```
