# 朱嵘

> 前端工程化、效率提升、组件复用性、前端业务逻辑开发、代码优化

- 男 / 1996 / 2019届
- 本科 / 江西财经大学软件工程专业
- 期望职位： Web前端工程师

# 联系方式

- 手机：18370153530
- Email：940223872@qq.com
- QQ/微信: 940223872/zsmj1110zsmj

# 个人信息

 - [Github](https://github.com/ZhuRon)
 - [掘金](https://juejin.im/user/5a2f2dce6fb9a045257813b0/posts)
 - 关键词：`记录得失` `追求效率` `热爱开源` `创造价值` `学习新技术` `深入思考问题` 
 
# 实习经历

## 鸿钧科技
> 实习时间（ 2018年8月 ~ 2018年11月 ）
<br/>

### megatech.ai

- 技术栈 `vue`  `node.js` `webpack` `ES6` 

>项目经历： 采用vux作为ui组件库,数据图表方面使用echart，vue-router进行路由管理。八月底开始，十月一号完成第一版demo并且上线进行内部测试。

>项目地址  earth.megatech.today:9999


---

# 开源项目
- [微信小程序-lingvist]()
    - 关键词 `小程序` `WEUI` `iconFont` `掘金` 
    - 地址 https://juejin.im/post/5a312794f265da43231af9c4 
    - 备注 小程序刚火的时候开始学习，因为很喜欢lingvist的ui界面所以仿造其app写了一个

- [React 迁移性学习]()
    - 关键词 `React` `掘金`
    - 地址 https://juejin.im/user/5a2f2dce6fb9a045257813b0/posts
    - 备注 做react的迁移性学习的时候，看了阮一峰老师前几年写的文章于是仿造写了一篇更新语法的文章
- [VUE-党员管理系统]()
    - 关键词 `Vue` `Vuex` `rem` `cube-ui`
    - 地址 https://github.com/ZhuRon/management-system
    - 备注 因为在学校的经历所以准备写这个项目，正准备进行2.0迭代

# 技能清单

- 基础： HTML / JavaScript / CSS
- 前端框架：Vue / React
- 前端工具：Webpack / Gulp / LeSS / Stylus
- 可视化： ECharts
- 后端语言： Node.js
- 版本管理、文档和自动化部署工具：Git 
- 数据库相关： MongoDB / Mongoose 
- 图像编辑工具 ：sketch

# 致谢
感谢您花时间阅读我的简历，期待能有机会和您共事。




# 介于界面改动使一些效果被迫放弃，特此笔记所录
## css做向上向下箭头
.up,.down{
  width:0;
  height:0;
  position:relative;
  border-style:solid;
}
向上
.up{
  border-width:0 10px 10px;
  border-color:transparent transparent red; 透明 透明  灰
}
向下
.down{
  border-width:10px 10px 0;
  border-color:green transparent transparent; 灰 透明 透明 
} 
## 超过两行省略 需要设置宽高
  overflow: hidden;
  display: -webkit-box;
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;
  word-break: break-all;
## 9.17
- 完成了部分路由跳转，首页个股风口，自选股，搜索页个股点击跳转到个股页
this.$router.push({path: '/news/' + this.xxx})
- 获取键值对msg的值
  for (var i in msg) {
    console.log(msg[i])
  }
- 个股，板块，早午报，正文底导
## 9.19
- 数据更改模板不渲染
查看更多想用v-if，没有数据的时候显示暂无搜索结果，后台请求到数据改成数据显示界面，但是值更新界面没有更新，在生命周期函数mounted（html模板渲染完成之后）里面写入this.$set,改变data里面的值，进行判断。
- 改变主页柱状图,完成了主页样式的调整
## 文字公告栏上下滚动
    <transition class="logo-container" name="slide" mode="out-in">
      <div class="logo" :key="text.id">{{text.type}}</div>
    </transition>
## 点赞（vue-star控件）转发 暂停/播放 组件封装
## 9.25
- 调整了个股页面样式
writing-mode: vertical-lr;竖排文字居中
## 9.26
- 调整了登录页设计，添加了logo，重构了智读与热评的页面样式
## 10.8
解决了子路由跳转跳不出去的问题
用this.$router.replace 取代 this.$router.push
这样在history里面就不会有记录，就可以直接跳出去
## 10.10
修改了scroller的组件
解耦了search页面
## 10.15
增加了滚动条滚动到指定位置
document.querySelector('.classname').scrollIntoView()
## 10.16
增加了智能ai界面
## 10.17
增加了个股页面的吸顶,调节了个股页面三个板块更新时候的跳动，增加了静态图片logos
## 10.18
tab导航条默认选项随页面改变
增加404页面
加水纹效果
sticky，安卓部分失效须改写
## 未完成
swiper左右滑动添加
平滑滚动添加
主页水文图控制
转入转出动画
# 10.23
个股页面左右滑动
table页面原生实现图标及图标的上下滑动
ai界面显示输入文字
# 10.29
ai界面大盘模块样式改动
# 10.30
去除横向滚动滚动条
整理了所有照片文件夹命名及文件路径