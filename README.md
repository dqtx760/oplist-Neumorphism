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

<!--点击烟花-->
<!--<script async src="https://cdn.jsdelivr.net/gh/mocchen/cssmeihua/js/yanhuabowen.js"></script>-->

<span class="js-cursor-container"></span>
<script async src="https://cdn.jsdelivr.net/gh/mocchen/cssmeihua/js/xiaoxingxing.js"></script>
<!--樱花飘落二选一-->
<script src="https://files.cnblogs.com/files/quaint/sakuraPlus.js"></script>
<!--<script async src="https://cdn.jsdelivr.net/gh/iVampireSP/special-JavaScript/yinghua.js"></script>-->

<!--音乐歌词美化-->
<script src="https://npm.elemecdn.com/granim@2.0.0/dist/granim.min.js"></script>
<script>
var granimInstance = new Granim({
    element: '#canvas-basic',
    direction: 'left-right',
    isPausedWhenNotInView: true,
    states : {
        "default-state": {
            gradients: [
                ['#a18cd1', '#fbc2eb'],
                 ['#fff1eb', '#ace0f9'],
                 ['#d4fc79', '#96e6a1'],
                 ['#a1c4fd', '#c2e9fb'],
                 ['#a8edea', '#fed6e3'],
                 ['#9890e3', '#b1f4cf'],
                 ['#a1c4fd', '#c2e9fb'],
                 ['#fff1eb', '#ace0f9']
           
            ]
        }
    }
});
</script>

<!-- 音乐增强 -->
<script>
  window.initMuscPlus = false;
  window.$q = window.$q || function(val) { return document.querySelector(val) }
  window.$qa = window.$qa || function(val) { return Array.from(document.querySelectorAll(val)) }

  // 生成随机渐变色
  function generateRandomGradient() {
    const randomColor = () => `rgba(${Math.floor(Math.random() * 255)}, ${Math.floor(Math.random() * 255)}, ${Math.floor(Math.random() * 255)}, ${Math.random().toFixed(2)})`;
    const color1 = randomColor();
    const color2 = randomColor();
    darkUIChange();
    return `linear-gradient(to right, ${color1}, ${color2})`;
  }

  ;(function(){
    let style = document.createElement('style')
    style.innerHTML = `
      .music-plus .aplayer .aplayer-lrc { 
        position: fixed; 
        top: 180px; 
        left: 0; 
        right: 0; 
        width: 88%; 
        height: 100px; 
        max-width: 1000px; 
        margin: 0 auto; 
        padding: 50px 0; 
        transform: scale(1.3);
        z-index: 999; 
        background: ${generateRandomGradient()}; /* 随机渐变背景 */
        backdrop-filter: blur(10px); /* 添加高斯模糊效果 */
        box-shadow: 0 4px 8px rgba(0,0,0,0.5); /* 添加阴影，增加立体感 */
        transition: background 0.5s ease; /* 平滑过渡渐变背景 */
      }
      .music-plus .aplayer .aplayer-lrc-current { 
        font-weight: bold; 
        transform: scale(0.95) !important; 
      }
      .music-plus .aplayer .aplayer-lrc p { 
        color: #fff; /* 设置歌词文字颜色为白色 */
        opacity: 1; /* 设置透明度 */
        transform: scale(0.9); 
      }
      .music-control { 
        position: absolute; 
        right: 4px; 
        top: 4px; 
        display: flex; 
        align-items: center; 
      }
      .music-control i { 
        cursor: pointer; 
        width: 22px; 
        height: 22px; 
        display: flex; 
        align-items: center; 
        justify-content: center; 
        font-size: 14px; 
        border-radius: 50%; 
        background: rgba(255, 255, 255, 0.2); /* 控制按钮背景颜色 */
        margin-left: 4px; 
        font-style: normal; 
      }
      /*电脑模式音乐歌词容器设置*/
      @media screen and (min-width: 1200px) {
        .music-plus .aplayer .aplayer-lrc { 
          left: 0; 
          right: 0;
          width: 410px; 
          height: 100px; 
          padding: 100px 0; 
          top: 212px;
        }

      }
    `
    document.body.appendChild(style)

  })();

  setTimeout(() => {
    let stack = document.querySelector('#musicPlus2')
    let span = document.createElement('span')
    span.innerHTML = '|'
    stack.appendChild(span)
    let a = document.createElement('a')
    a.style = `padding: var(--hope-space-1_5); cursor: pointer; `
    a.innerHTML = '音乐加强'
    a.onclick = changeMusic
    stack.appendChild(a)

    document.addEventListener('keydown', function(e) {
      if (e.ctrlKey) {
        const type = ['4', '['].includes(e.key) ? 1 : ['6', ']'].includes(e.key) ? 3 : ['5', '\\'].includes(e.key) ? 2 : null
        if (type) {
          e.preventDefault()
          e.stopPropagation()
          musicMove(type)
        }
      }
    })
  }, 1000)

  function darkUIChange() {
    // 获取当前页面宽度,设置样式
    var documentWidth = $(document).width();
    let widthIsMin = 0;
    if (documentWidth<600){
    widthIsMin = 1;
    }
    // 黑夜模式调整样式
    let isDarkUI= document.querySelector('.hope-ui-dark')
    if (isDarkUI){
     $(".music-plus .aplayer .aplayer-lrc").css("top", "315px");
     // 小屏幕 手机 调整样式
     if(widthIsMin){
        $(".music-plus .aplayer .aplayer-lrc").css("top", "332px");
      }
    }
  
  }

  function changeMusic() {
    let lrcWarp = document.querySelector('.aplayer .aplayer-lrc')
    if (!lrcWarp) return alert('没有找到歌词容器')

    if (!window.initMuscPlus || !$q('.music-control')) {
      let control = document.createElement('div')
      control.className = 'music-control'
      control.innerHTML = `<i onclick="musicMove(1)" title="CTRL+[ 上一曲">◄</i>
      <i onclick="musicMove(2)" title="CTRL+] 上一曲">◼</i>
      <i onclick="musicMove(3)" title="CTRL+\\ 暂停">►</i>`
      document.querySelector('.aplayer-body').append(control)
    }
    window.initMuscPlus = true
    let cls = document.body.className
    if (cls.includes('music-plus')) {
      document.body.className = document.body.className.replace(' music-plus', '')
    } else {
      document.body.className += ' music-plus'
    }

    // 每次切换歌曲时重新生成渐变背景
    lrcWarp.style.background = generateRandomGradient();
    darkUIChange();

  }

  function musicMove(type) {
    if (type == 2) {
      return $q('.aplayer-pic').click()
    }
    let list = $qa(`.aplayer-list li`)
    let ind = list.findIndex(item => item.classList.contains('aplayer-list-light'))
    let index = type == 1 ? ind - 1 : type == 3 ? ind + 1 : ind
    index = index < 0 ? list.length - 1 : index > list.length - 1 ? 0 : index
    list[index].click()

   
  }

</script>
<!---去掉底部文字--->

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

<!--点击烟花-->
<!--<script async src="https://cdn.jsdelivr.net/gh/mocchen/cssmeihua/js/yanhuabowen.js"></script>-->

<span class="js-cursor-container"></span>
<script async src="https://cdn.jsdelivr.net/gh/mocchen/cssmeihua/js/xiaoxingxing.js"></script>
<!--樱花飘落二选一-->
<script src="https://files.cnblogs.com/files/quaint/sakuraPlus.js"></script>
<!--<script async src="https://cdn.jsdelivr.net/gh/iVampireSP/special-JavaScript/yinghua.js"></script>-->

<!--音乐歌词美化-->
<script src="https://npm.elemecdn.com/granim@2.0.0/dist/granim.min.js"></script>
<script>
var granimInstance = new Granim({
    element: '#canvas-basic',
    direction: 'left-right',
    isPausedWhenNotInView: true,
    states : {
        "default-state": {
            gradients: [
                ['#a18cd1', '#fbc2eb'],
                 ['#fff1eb', '#ace0f9'],
                 ['#d4fc79', '#96e6a1'],
                 ['#a1c4fd', '#c2e9fb'],
                 ['#a8edea', '#fed6e3'],
                 ['#9890e3', '#b1f4cf'],
                 ['#a1c4fd', '#c2e9fb'],
                 ['#fff1eb', '#ace0f9']
           
            ]
        }
    }
});
</script>

<!-- 音乐增强 -->
<script>
  window.initMuscPlus = false;
  window.$q = window.$q || function(val) { return document.querySelector(val) }
  window.$qa = window.$qa || function(val) { return Array.from(document.querySelectorAll(val)) }

  // 生成随机渐变色
  function generateRandomGradient() {
    const randomColor = () => `rgba(${Math.floor(Math.random() * 255)}, ${Math.floor(Math.random() * 255)}, ${Math.floor(Math.random() * 255)}, ${Math.random().toFixed(2)})`;
    const color1 = randomColor();
    const color2 = randomColor();
    darkUIChange();
    return `linear-gradient(to right, ${color1}, ${color2})`;
  }

  ;(function(){
    let style = document.createElement('style')
    style.innerHTML = `
      .music-plus .aplayer .aplayer-lrc { 
        position: fixed; 
        top: 180px; 
        left: 0; 
        right: 0; 
        width: 88%; 
        height: 100px; 
        max-width: 1000px; 
        margin: 0 auto; 
        padding: 50px 0; 
        transform: scale(1.3);
        z-index: 999; 
        background: ${generateRandomGradient()}; /* 随机渐变背景 */
        backdrop-filter: blur(10px); /* 添加高斯模糊效果 */
        box-shadow: 0 4px 8px rgba(0,0,0,0.5); /* 添加阴影，增加立体感 */
        transition: background 0.5s ease; /* 平滑过渡渐变背景 */
      }
      .music-plus .aplayer .aplayer-lrc-current { 
        font-weight: bold; 
        transform: scale(0.95) !important; 
      }
      .music-plus .aplayer .aplayer-lrc p { 
        color: #fff; /* 设置歌词文字颜色为白色 */
        opacity: 1; /* 设置透明度 */
        transform: scale(0.9); 
      }
      .music-control { 
        position: absolute; 
        right: 4px; 
        top: 4px; 
        display: flex; 
        align-items: center; 
      }
      .music-control i { 
        cursor: pointer; 
        width: 22px; 
        height: 22px; 
        display: flex; 
        align-items: center; 
        justify-content: center; 
        font-size: 14px; 
        border-radius: 50%; 
        background: rgba(255, 255, 255, 0.2); /* 控制按钮背景颜色 */
        margin-left: 4px; 
        font-style: normal; 
      }
      /*电脑模式音乐歌词容器设置*/
      @media screen and (min-width: 1200px) {
        .music-plus .aplayer .aplayer-lrc { 
          left: 0; 
          right: 0;
          width: 410px; 
          height: 100px; 
          padding: 100px 0; 
          top: 212px;
        }

      }
    `
    document.body.appendChild(style)

  })();

  setTimeout(() => {
    let stack = document.querySelector('#musicPlus2')
    let span = document.createElement('span')
    span.innerHTML = '|'
    stack.appendChild(span)
    let a = document.createElement('a')
    a.style = `padding: var(--hope-space-1_5); cursor: pointer; `
    a.innerHTML = '音乐加强'
    a.onclick = changeMusic
    stack.appendChild(a)

    document.addEventListener('keydown', function(e) {
      if (e.ctrlKey) {
        const type = ['4', '['].includes(e.key) ? 1 : ['6', ']'].includes(e.key) ? 3 : ['5', '\\'].includes(e.key) ? 2 : null
        if (type) {
          e.preventDefault()
          e.stopPropagation()
          musicMove(type)
        }
      }
    })
  }, 1000)

  function darkUIChange() {
    // 获取当前页面宽度,设置样式
    var documentWidth = $(document).width();
    let widthIsMin = 0;
    if (documentWidth<600){
    widthIsMin = 1;
    }
    // 黑夜模式调整样式
    let isDarkUI= document.querySelector('.hope-ui-dark')
    if (isDarkUI){
     $(".music-plus .aplayer .aplayer-lrc").css("top", "315px");
     // 小屏幕 手机 调整样式
     if(widthIsMin){
        $(".music-plus .aplayer .aplayer-lrc").css("top", "332px");
      }
    }
  
  }

  function changeMusic() {
    let lrcWarp = document.querySelector('.aplayer .aplayer-lrc')
    if (!lrcWarp) return alert('没有找到歌词容器')

    if (!window.initMuscPlus || !$q('.music-control')) {
      let control = document.createElement('div')
      control.className = 'music-control'
      control.innerHTML = `<i onclick="musicMove(1)" title="CTRL+[ 上一曲">◄</i>
      <i onclick="musicMove(2)" title="CTRL+] 上一曲">◼</i>
      <i onclick="musicMove(3)" title="CTRL+\\ 暂停">►</i>`
      document.querySelector('.aplayer-body').append(control)
    }
    window.initMuscPlus = true
    let cls = document.body.className
    if (cls.includes('music-plus')) {
      document.body.className = document.body.className.replace(' music-plus', '')
    } else {
      document.body.className += ' music-plus'
    }

    // 每次切换歌曲时重新生成渐变背景
    lrcWarp.style.background = generateRandomGradient();
    darkUIChange();

  }

  function musicMove(type) {
    if (type == 2) {
      return $q('.aplayer-pic').click()
    }
    let list = $qa(`.aplayer-list li`)
    let ind = list.findIndex(item => item.classList.contains('aplayer-list-light'))
    let index = type == 1 ? ind - 1 : type == 3 ? ind + 1 : ind
    index = index < 0 ? list.length - 1 : index > list.length - 1 ? 0 : index
    list[index].click()

   
  }

</script>
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
