# font minify
> 从字体包中提取3500常用汉字，英文字母以及数字进行字体包压缩
## 用法
```
npm install
```

### 设置好字体引用
- 创建一个font文件夹以便管理字体包，压缩完后会将原来字体备份在新建的隐藏文件夹中
- 将下载好的字体包放到font文件夹
- 设置index.css
``` css
// 设置字体名称已经引用路径
@font-face {
  font-family: '字体名';
  src: url('./font/字体包路径'); // 支持 ttf、woff2、woff、eot、svg
  font-weight: normal;
  font-style: normal;
}
h1 {
    font-family: '字体名';
}
```

### 压缩
```
npm run build
```
> 命令执行完后，原来字体包会被替换成被压缩过的字体包，同时备份了原来字体包在.font-spider文件夹（隐藏文件夹）

### 引用工具
[字蛛](http://font-spider.org/)

### 免费字体
- [思源黑体: 简体中文 ttf 版本](https://github.com/aui/free-fonts/archive/KaiGenGothic-1.001-SimplifiedChinese.zip)
- [思源黑体: 繁体中文 ttf 版本](https://github.com/aui/free-fonts/archive/KaiGenGothic-1.001-TraditionalChinese.zip)
- [思源黑体: 中、日、韩 ttf 版本](https://mega.nz/#!PZxFSYQI!ICvNugaFX_y4Mh003-S3fao1zU0uNpeSyprdmvHDnwc)
- [开源图标字体: Font Awesome](http://fontawesome.io)
