## blog��ϰ
****
### Hexoʹ��

1.hexo init

2.hexo install

3.npm install-deployer-git --save

4.git clone https://gitee.com/Lhcfl/hexo-theme-anatolo.git themes/Anatolo
����ֱ����������zip����ѹ������Ŀ¼�£�������ΪAnatolo

5.��װ������

npm install hexo-renderer-pug --save

npm install hexo-renderer-stylus --save

6.���ã�
����_config.example.ymlΪ_config.yml
�޸�hexo��Ŀ¼�µ� _config.yml �� theme: Anatolo

7.hexo new post ����

8.��md�ļ���source�ļ�������
****
### Next����8.xʹ�ü�¼

#### �������������

1. ȥ��ҳ���������������Ӵ��룬�ŵ�
```
C:\Users\wangzihan\Desktop\blog1\themes\next\layout\_macro\sidebar.njk 
```
�ļ��У��ǵ÷��м� Щ��λ�ã���ĩβû�á�

#### ����͸��
```
C:\Users\wangzihan\Desktop\blog1\themes\next\source\css\_schemes\Gemini\index.styl
```
�ļ��£���29�У���rgba(255,255,255,0.7)

#### ͷ����ת

���������ļ��£�

```
avatar:
  # Replace the default image and set the url here.
  url: /images/favicon-32x32-next.png
  # If true, the avatar will be displayed in circle.
  rounded: true #�����Բ��չʾ
  # If true, the avatar will be rotated with the cursor.
  rotated: true #����ǿ�����ת
```

#### ��������

##### 1.����ͼ
��
```
C:\Users\wangzihan\Desktop\blog1\source\_data\style1.styl
```
Ŀ¼�£����ļ�style1.styl���༭ͼƬ��ַ�����ñ���ͼƬ�Ĳ���
��20���йأ��йر����Ķ��ڴ����ã�
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

##### 2.������Ч

�ļ���װ��
```
C:\Users\wangzihan\Desktop\blog1\themes\next\source\lib\theme-next-canvas-nest
```

ֻ��װ��canvas_nest

```
canvas_nest: # ���米��
  enable: true
  onmobile: true # display on mobile or not
  color: '0,0,0' # RGB values, use ',' to separate
  opacity: 0.5 # the opacity of line: 0~1
  zIndex: -1 # z-index property of the background
  count: 150 # the number of lines
```
����Ϊtrue��������


#### �Ķ�ԭ��

�������
```
<!-- more -->
```

#### �����

���������ļ���
```
live2d:
  enable: true
  scriptFrom: local
  pluginRootPath: live2dw/
  pluginJsPath: lib/
  pluginModelPath: assets/
  tagMode: false
  model:
    use: live2d-widget-model-koharu  #ѡ������ģ��
  display: #����λ�úʹ�С
    position: right
    width: 150
    height: 300
  mobile:
    show: true #�Ƿ����ֻ�����ʾ
```
��[lived2d]( https://github.com/xiazeyu/live2d-widget-models)����ģ��
ʹ��npm����������
```
 use: live2d-widget-model-koharu  #ѡ������ģ��
```
#### δ�����

[�ο����������2d����ģ��Ԥ��](https://blog.csdn.net/as480133937/article/details/100138838?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522164760572416782248533224%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=164760572416782248533224&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~rank_v31_ecpm-10-100138838.142^v2^pc_search_result_control_group,143^v4^control&utm_term=hexo+next+valine&spm=1018.2226.3001.4187)