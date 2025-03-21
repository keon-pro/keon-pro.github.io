---
layout: default
title: "我的黑色炫富主页"
---

<style>
/* 
  ==============
  黑色主题 + 5个炫富泡泡的交互示例
  ============== 
*/

/* 通用样式：将页面背景设为黑色，文字设为白色 */
body {
  margin: 0;
  padding: 0;
  background-color: #000;
  color: #fff;
  font-family: "Helvetica Neue", Arial, sans-serif;
}

/* 主容器，可以为页面其他元素提供一些内边距 */
.main-container {
  padding: 40px 20px;
  text-align: center;
}

/* 标题样式 */
h1 {
  font-size: 2.2rem;
  margin: 0 0 30px;
}

/* 段落文字 */
p {
  font-size: 1.1rem;
  line-height: 1.6;
  max-width: 800px;
  margin: 0 auto 20px auto;
}

/* 
  ==============
  炫富泡泡（按钮）区域 
  ==============
*/

.bubble-container {
  position: relative;
  width: 100%;
  max-width: 1200px;
  margin: 50px auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
}

/* 每个泡泡的基础样式：圆形、可点击、带有hover效果、动画 */
.bubble {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  display: inline-flex; /* 或可用 block + text-align center 容器 */
  align-items: center;
  justify-content: center;
  text-decoration: none;
  color: #fff;
  font-weight: bold;
  font-size: 0.9rem;
  box-shadow: 0 0 20px rgba(255, 255, 255, 0.5);
  cursor: pointer;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  position: relative;

  /* 添加浮动动画 */
  animation: float-bubble 3s ease-in-out infinite;
}

/* 鼠标悬停时，放大并加强阴影 */
.bubble:hover {
  transform: scale(1.1);
  box-shadow: 0 0 30px rgba(255, 255, 255, 0.8);
}

/* 不同的颜色示例，可根据喜好自行调整 */
.bubble1 {
  background: linear-gradient(135deg, #ff0080, #ffaf00);
}
.bubble2 {
  background: linear-gradient(135deg, #00b2ff, #8cff00);
}
.bubble3 {
  background: linear-gradient(135deg, #8e2de2, #4a00e0);
}
.bubble4 {
  background: linear-gradient(135deg, #c31432, #240b36);
}
.bubble5 {
  background: linear-gradient(135deg, #f12711, #f5af19);
}

/* 自定义一个上下浮动的关键帧动画 */
@keyframes float-bubble {
  0% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-15px);
  }
  100% {
    transform: translateY(0px);
  }
}

/* 可以为每个bubble里的文字/图标再设些微调 */
.bubble span {
  text-align: center;
  line-height: 1.2;
}

/* 加一点媒体查询，移动端略缩小泡泡尺寸(可根据需求增改) */
@media (max-width: 480px) {
  .bubble {
    width: 80px;
    height: 80px;
    font-size: 0.8rem;
  }
}

</style>

<!-- 主容器：放置页面主要文字内容 -->
<div class="main-container">
  <h1>我的黑色炫富主页</h1>
  <p>
    这里是主页内容示例，背景为纯黑色，文字为白色。下面放置了五个“炫富泡泡”，它们在页面中上下浮动、带有炫彩渐变，并且可以点击跳转到不同的页面。请根据自己的项目需求，修改每个泡泡的链接地址及文字说明。
  </p>
</div>

<!-- 5个炫富泡泡/按钮容器 -->
<div class="bubble-container">
  <!-- 点击后跳转到 page1.html，可根据需求换成实际链接，如 /page1/, /page1.md, 其它站点等 -->
  <a href="page1.html" class="bubble bubble1">
    <span>泡泡 1</span>
  </a>
  <a href="page2.html" class="bubble bubble2">
    <span>泡泡 2</span>
  </a>
  <a href="page3.html" class="bubble bubble3">
    <span>泡泡 3</span>
  </a>
  <a href="page4.html" class="bubble bubble4">
    <span>泡泡 4</span>
  </a>
  <a href="page5.html" class="bubble bubble5">
    <span>泡泡 5</span>
  </a>
</div>

<!-- 根据需要可在此处加入更多内容或页脚 -->
<p style="text-align:center; margin-bottom: 40px;">
  你可以在这里加入更多炫酷内容，比如个人简介、项目展示、联系方式等。
</p>
