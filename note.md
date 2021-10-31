项目描述： 完成电商网站，我们要完成 首页、列表页、详情页、注册页面的制作。

设计目标：
1、保证浏览器 ie7 以上 火狐，360 safari chrome等兼容，先不管低版本的浏览器项目
2、熟悉 css+div 布局、页面搭建
3、了解常用电商类网站的布局模式
4、为后期品优购移动端铺垫。

几点思考：
1）开发工具，vscode ps 主流浏览器
2）技术栈： HTML 结构 + CSS 布局。

规范：
html 规范
图片规范
CSS规范
命名规范
    目录命名规范： 样式文件夹：css； 文件夹 js  样式类图片文件夹：img  产品类图片文件夹： upload 
    字体类： fonts

    class命名规范
#### 样式文件分类
css 初始化文件，都统一放在 base.css 文件夹里面。
公共样式，放在 common.css中

#### iconmoon

字体文件下载，两个网站：
阿里图标：
icoMoon

自己制作icon图标

1、下载字体包

推荐网站：http://icomoon.io
阿里icon font字库 


#### SEO优化，就是搜索引擎优化
1、三大标签在； title  description Keywords;
一般SEO优化，有对应的人员进行设计，我们只要把这些标签写到代码中即可。
优化网站的三大标签： title description

···
    <title>优品购-正品低价、品质保障、配送及时、轻松购物</title>
    <meta name="description" content="优品购JD.COM-专业的综合网上购物，销售家电，xxxxxx">
    <meta name="Keywords" content="网上购物、网上商城、手机、笔记本、电脑。。">
  
#### 字体图标使用

2、引入字体
@font-face {
     font-family: 'icomoon';
     src:  url('fonts/icomoon.eot?7kkyc2');
     src:  url('fonts/icomoon.eot?7kkyc2#iefix') format('embedded-opentype'),
       url('fonts/icomoon.ttf?7kkyc2') format('truetype'),
       url('fonts/icomoon.woff?7kkyc2') format('woff'),
       url('fonts/icomoon.svg?7kkyc2#icomoon') format('svg');
     font-weight: normal;
     font-style: normal;
   }
3、使用字体

span {
            font-size: 50px;
            font-family: 'icomoon';
            color: black;
    }

    <span>
        
    </span>

4、追加字体，找到文件中的 select.json文件，导入回icomoon.io 上,然后就能继续选择添加图标，import icons，然后再重新下载，替换以前的文件即可。

##### logo 优化
1、logo 里面首先放一个 h1标签，目的是为了提前告诉搜索引擎，这个地方很重要
2、h1里面在放一个 连接a，可以返回首页的，给连接一个大小和 logo背景图片
3、连接里面发文（网站名称），但是文字不要显示出来，要用 text-indent【首行缩进】 移到盒子外面。然后 overflow：hidden；
font-size：0px；

4、最后给连接 一个title这样，鼠标方到logo上。就可以看到提示文字。

