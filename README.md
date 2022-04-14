## blog练习
****
### Hexo使用

1.hexo init

2.hexo install

3.npm install-deployer-git --save

4.git clone https://gitee.com/Lhcfl/hexo-theme-anatolo.git themes/Anatolo
或者直接下载主题zip包解压至主题目录下，重命名为Anatolo

5.安装依赖：

npm install hexo-renderer-pug --save

npm install hexo-renderer-stylus --save

6.配置：
复制_config.example.yml为_config.yml
修改hexo根目录下的 _config.yml ： theme: Anatolo

7.hexo new post 名称

8.该md文件在source文件夹下面
****
### Next主题8.x使用记录

#### 添加网易云音乐

1. 去网页版网易云生成链接代码，放到
```
C:\Users\wangzihan\Desktop\blog1\themes\next\layout\_macro\sidebar.njk 
```
文件中，记得放中间 些的位置，放末尾没用。

#### 版面透明
```
C:\Users\wangzihan\Desktop\blog1\themes\next\source\css\_schemes\Gemini\index.styl
```
文件下，第29行，改rgba(255,255,255,0.7)

#### 头像旋转

主题配置文件下：

```
avatar:
  # Replace the default image and set the url here.
  url: /images/favicon-32x32-next.png
  # If true, the avatar will be displayed in circle.
  rounded: true #这个是圆形展示
  # If true, the avatar will be rotated with the cursor.
  rotated: true #这个是靠近旋转
```

#### 背景设置

##### 1.背景图
在
```
C:\Users\wangzihan\Desktop\blog1\source\_data\style1.styl
```
目录下，打开文件style1.styl，编辑图片地址，设置背景图片的参数
第20行有关，有关背景的都在此配置，
```
custom_file_path:
  #head: source/_data/head.njk
  #header: source/_data/header.njk
  #sidebar: source/_data/sidebar.njk
  #postMeta: source/_data/post-meta.njk
  #postBodyEnd: source/_data/post-body-end.njk
  #footer: source/_data/footer.njk
  #bodyEnd: source/_data/body-end.njk
  #variable: source/_data/variables.styl
  #mixin: source/_data/mixins.styl
  #style: source/_data/styles.styl
  style: source/_data/style1.styl
```

##### 2.背景动效

文件安装在
```
C:\Users\wangzihan\Desktop\blog1\themes\next\source\lib\theme-next-canvas-nest
```

只安装了canvas_nest

```
canvas_nest: # 网络背景
  enable: true
  onmobile: true # display on mobile or not
  color: '0,0,0' # RGB values, use ',' to separate
  opacity: 0.5 # the opacity of line: 0~1
  zIndex: -1 # z-index property of the background
  count: 150 # the number of lines
```
设置为true即可运行


#### 阅读原文

文中添加
```
<!-- more -->
```

#### 面板娘

博客配置文件下
```
live2d:
  enable: true
  scriptFrom: local
  pluginRootPath: live2dw/
  pluginJsPath: lib/
  pluginModelPath: assets/
  tagMode: false
  model:
    use: live2d-widget-model-koharu  #选择哪种模型
  display: #放置位置和大小
    position: right
    width: 150
    height: 300
  mobile:
    show: true #是否在手机端显示
```
在[lived2d]( https://github.com/xiazeyu/live2d-widget-models)下载模型
使用npm命令，随后配置
```
 use: live2d-widget-model-koharu  #选择哪种模型
```
#### 未完待续

[参考这个，还有2d人物模型预览](https://blog.csdn.net/as480133937/article/details/100138838?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522164760572416782248533224%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=164760572416782248533224&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~rank_v31_ecpm-10-100138838.142^v2^pc_search_result_control_group,143^v4^control&utm_term=hexo+next+valine&spm=1018.2226.3001.4187)