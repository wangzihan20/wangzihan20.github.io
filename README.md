blog练习
===================
Hexo使用

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