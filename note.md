
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