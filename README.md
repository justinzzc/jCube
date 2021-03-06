# jCube
a jquery plugin to create 3d cube


> 只需添加一行js脚本就可以创建出一个可以拖动旋转的3d立方体.
> [https://justinzzc.github.io/jCube/](https://justinzzc.github.io/jCube/)

##用法

### 安装

~~~ javascript
> bower install jCube
~~~

### 基本使用方法

~~~ html
<head>
    <script src="jquery.min.js"></script>
    <script src="../dist/jCube.min.js"></script>
</head>

<body>
...

<div class="room">

</div>
...

<script>
    $(function(){
       $('.room').jCube({
           wallWidth:635,
           wallHeight:664,
           cube:{
               back:'a/back.jpg',
               front:'a/front.jpg',
               left:'a/left.jpg',
               right:'a/right.jpg',
               top:'#90c0c0',
               bottom:'#9f5d3b'
           },
           perspectiveRate:1.21
       });
    });
</script>
</body>

~~~




##配置项

+ 可用配置项
 - 墙纸宽度 wallWidth , 墙纸高度 wallHeight
 - 立方体背景配置 cube
 - 墙面附加物配置 attach
 - 立方体class名称 cubeClass
 - 视角调整比例 perspectiveRate
 
 
###默认配置

~~~ javascript
{
    wallWidth: 300,
    wallHeight: 300,
    cube: {
        front: 'white',
        back: 'white',
        left: '#d3d3d3',
        right: '#d3d3d3',
        top: '#f3f3f3',
        bottom: '#ddd'
    },
    attach: {
        front: '',
        back: '',
        left: '',
        right: '',
        top: '',
        bottom: ''
    },
    cubeClass: 'room-cube',
    perspectiveRate: 1,
    viewLimit: {
        xMin: -15,
        xMax: 15,
        yMin: -360,
        yMax: 360
    }
}
~~~



###详细请查看 
- [demo页面1-立方体](https://justinzzc.github.io/jRoom/demo/test3.html)

###捐赠donate
![](https://justinzzc.github.io/imgs/donate.jpg)