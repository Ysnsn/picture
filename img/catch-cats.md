---
title: 一起圈小猫猫
date: 2020-08-12 22:27:11
aside: false
top_img: https://cdn.jsdelivr.net/gh/laugh0608/CDN/img/20200812223845.jpg
---

<script src="/myjs/phaser.min.js"></script>
<script src="/myjs/catch-the-cat.js"></script>
<style>
    #catch-the-cat{
      display: flex;
      justify-content: center;
    }
  </style>
<body>
<script>
$(document).ready(function () {
    if(location.href.indexOf("#reloaded")==-1){
        location.href=location.href+"#reloaded";
        location.reload();
    }
})
</script>
  <p>圈小猫小游戏</p>
  <p>游戏规则：点进重置可刷新小猫场景，用鼠标点击浅色圆点，你每点击一下，小猫相应的逃亡一次。如果你成功的将小猫围困在深色之内则获胜，小猫逃到地图边界则输</p>
  <div id="catch-the-cat"></div>
</body>
<script>
  window.game = new CatchTheCatGame({
    w: 11,
    h: 11,
    r: 20,
    backgroundColor: 0xeeeeee,
    parent: 'catch-the-cat',
    statusBarAlign: 'center',
    credit: '大白萝卜'
  });
</script>