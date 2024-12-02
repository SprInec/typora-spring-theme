<img src=".assets/logo-spring.png" alt="logo-spring" />

<p align="center">
    一款令人如沐春风的 Typora 灵动主题
    <br/>
    A refreshing and graceful Typora theme, like a gentle spring breeze.
    <br>
    Dynamic Interaction / Custom Configuration
    <br>
    动态交互 / 自定义配置
</p>
<p align="center">
  <a>
    <img src="https://img.shields.io/github/license/SprInec/typora-spring-theme" alt="GitHub license">
  </a>
  <a>
    <img src="https://badgen.net/github/stars/SprInec/typora-spring-theme?color=green&icon=github" alt="GitHub stars">
  </a>
  <a>
    <img src="https://badgen.net/github/commits/SprInec/typora-spring-theme?icon=github" alt="GitHub commits">
  </a>
  <a>
    <img src="https://badgen.net/github/watchers/SprInec/typora-spring-theme?color=purple&icon=github" alt="GitHub watchers">
  </a>
  <a>
      <img src="https://img.shields.io/badge/language-CSS-purple" />
  </a>
</p>



<p align="center">
    <a href="./README.md">English</a>
    ·
    <a>简体中文</a>
</p>

## 目录
- [主题预览](#主题预览)
- [设计元素](#设计元素)
- [自定义配置](#自定义配置)
- [快速安装与应用](#快速安装与应用)
- [Todo List](#Todo-List)
- [致谢](#致谢)
- [许可](#许可)

## 主题预览

<img src=".assets/preview_cn.png" alt="preview_cn"/>

## 设计元素

### 1. 充满春天气息的配色卡

![image-20241113191409991](.assets/image-20241113191409991.png)

### 2. 不同效果的灵动交互

- 一级标题 h1

<p align="center">
    <img src=".assets/h1.gif" width="100%" />
</p>

- 二级标题 h2

<p align="center">
    <img src=".assets/h2.gif" width="80%" />
</p>

- 三、四、五、六级标题 h3 h4 h5 h6

<p align="left">
    <img src=".assets/hx.gif" width="10%" />
</p>

- 段落悬停响应

 <p align="center">
    <img src=".assets/paragraph_hover.gif" width="100%" />
 </p>

- 内联样式

<p align="left">
    <img src=".assets/inline.gif" width="47%" />
</p>

- 无序列表

<p align="left">
    <img src=".assets/ul.gif" width="50%" />
 </p>

- 有序列表

<p align="left">
    <img src=".assets/ol.gif" width="50%" />
</p>

- 图片

 <p align="center">
    <img src=".assets/image.gif" width="100%" />
</p>

- 表格

<p align="center">
    <img src=".assets/table.gif" width="80%" />
</p>

- 代码块

<p align="center">
    <img src=".assets/code_block.gif" width="70%" />
</p>

- 引用块

<p align="center">
    <img src=".assets/blockquote.gif" width="70%" />
</p>

- 警告框

<p align="center">
    <img src=".assets/alert.gif" width="70%" />
</p>

### 3. 风格统一的 Typora 界面

<img align="center" src=".assets/sys.gif" style="zoom:50%;" />

## 自定义配置

### 交互效果配置

可根据需求自定义开启或关闭任意元素的交互效果，具体操作如下：

1. 打开 `spring.css` 文件，在文件开头根据注释找到交互效果配置选项；
2. 根据需求修改对应交互效果的变量值，`0` 为关闭，`1` 为开启；
3. 重启 Typora 即可应用更改。

> [!important]
>
> 1. 若要开启交互效果，请首先将 `–use-dynamic-effect` 设置为 `1`, 然后在针对具体类型进行配置。
> 2. 若要关闭全部的交互效果，直接将 `–use-dynamic-effect` 设置为 `0` 即可。（`–use-dynamic-effect`无法禁用有序列表的部分交互效果，若想要关闭有序列表的全部交互效果，请将 `--list-ol-text-style` 设置为 `italic`）

|         类型         |                      变量名                      |            值            |              功能               |    默认     |
| :------------------: | :----------------------------------------------: | :----------------------: | :-----------------------------: | :---------: |
|     **全局配置**     |              `--use-dynamic-effect`              |          0 / 1           | 关闭全部交互效果 / 使用交互效果 |      1      |
|       一级标题       |               `--h1-hover-effect`                |          0 / 1           |           关闭 / 开启           |      1      |
|       二级标题       |               `--h2-after-effect`                |          0 / 1           |           关闭 / 开启           |      1      |
| 三、四、五、六级标题 |              `--h3-6-hover-effect`               |          0 / 1           |           关闭 / 开启           |      1      |
|         段落         |                `--p-hover-effect`                |          0 / 1           |           关闭 / 开启           |      1      |
|         图片         |               `--img-hover-effect`               |          0 / 1           |           关闭 / 开启           |      1      |
|        引用块        |           `--blockquote-hover-effect`            |          0 / 1           |           关闭 / 开启           |      1      |
|        提示框        |              `--alert-hover-effect`              |          0 / 1           |           关闭 / 开启           |      1      |
|         粗体         |             `--strong-hover-effect`              |          0 / 1           |           关闭 / 开启           |      1      |
|         斜体         |               `--em-hover-effect`                |          0 / 1           |           关闭 / 开启           |      1      |
|        下划线        |                `--u-hover-effect`                |          0 / 1           |           关闭 / 开启           |      1      |
|         高亮         |              `--mark-hover-effect`               |          0 / 1           |           关闭 / 开启           |      1      |
|        删除线        |               `--del-hover-effect`               |          0 / 1           |           关闭 / 开启           |      1      |
|      内联代码块      |              `--code-hover-effect`               |          0 / 1           |           关闭 / 开启           |      1      |
|        代码块        |              `--fence-hover-effect`              |          0 / 1           |           关闭 / 开启           |      1      |
|         列表         | `--list-marker-effect`<br>`--list-ol-text-style` | 0 / 1<br>italic / normal |   关闭 / 开启<br>关闭 / 开启    | 1<br>normal |
|        分割线        |               ` --hr-hover-effect`               |          0 / 1           |           关闭 / 开启           |      1      |
|         表格         |              `--table-hover-effect`              |          0 / 1           |           关闭 / 开启           |      1      |

## 快速安装与应用

1. 在终端使用以下命令将此仓库克隆到本地 **/** 或者您也可以从 [Releases](https://github.com/SprInec/typora-spring-theme/releases) 获取稳定版本的压缩包并解压到本地。

    ```bash
    git clone https://github.com/SprInec/typora-spring-theme.git
    ```

2. 在 Typora 的左上角菜单中点击 ‘主题’，在 ‘主题’ 页面中点击打开 ‘主题文件夹’ 按钮。
3. 将文件 `spring.css` 复制到打开的 Typora 主题文件夹中。
4. 重启 Typora，然后主题列表中就可以选择使用 **Spring** 主题啦。

## Todo List

- [x] 浅色主题 SprIng
- [x] 灵动交互
- [x] 交互效果配置
- [ ] HTML导出配置
- [ ] 文档排版配置
- [ ] 暗色主题 SprIngNight
- [ ] 自定义配色卡
- [ ] 自定义样式
- [ ] 可供选择的多种交互效果
- [ ] [typora-plugin](https://github.com/obgnail/typora_plugin) 统一风格适配 

## [致谢](credits.md)

本项目基于 *typora-mo-theme* 进行了视觉与交互设计的二次开发，[template](template/) 来源于 *typora-theme-Jinxiu/template*。

- [MarMomento/typora-mo-theme](https://github.com/MarMomento/typora-mo-theme)
- [Sophomoresty/typora-theme-Jinxiu](https://github.com/Sophomoresty/typora-theme-Jinxiu)

## 许可

 该项目基于 MIT 开源协议，您可以自由地复制、修改和分发本项目的代码，但请保留原作者的[版权声明](LICENSE)。

<p align="center">
    <img src="https://api.star-history.com/svg?repos=SprInec/typora-spring-theme&type=Date"/>
</p>
