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
    <img src="https://badgen.net/github/watchers/SprInec/typora-spring-theme?color=purple" alt="GitHub watchers">
  </a>
  <a>
      <img src="https://img.shields.io/badge/language-CSS-purple" />
  </a>
</p>



<p align="center">
    <a>English</a>
    ·
    <a href="./README_cn.md">简体中文</a>
</p>

## Catalog
- [Preview](#Preview)
- [Feature](#Feature)
- [Custom Configuration](#Custom-Configuration)
- [Installation](#Installation)
- [Todo List](#Todo-List)
- [Credits](#Credits)
- [License](#License)

## Preview

![preview](.assets/preview.png)

## Feature

### 1. Spring-themed color palette

![image-20241113191409991](.assets/image-20241113191409991.png)

### 2. Flexible interaction with different effects

- h1

  <p align="center">
    <img src=".assets/h1.gif" width="100%" />
  </p>

- h2

  <p align="center">
    <img src=".assets/h2.gif" width="80%" />
  </p>

- h3 h4 h5 h6

  <p align="left">
    <img src=".assets/hx.gif" width="10%" />
  </p>

- Paragraph Hover Responsiveness

  <p align="center">
    <img src=".assets/paragraph_hover.gif" width="100%" />
  </p>

- Inline styles

  <p align="left">
    <img src=".assets/inline_en.gif" width="65%" />
  </p>

- Unordered list

  <p align="left">
    <img src=".assets/ul.gif" width="50%" />
  </p>

- Ordered List

  <p align="left">
    <img src=".assets/ol.gif" width="50%" />
  </p>

- Image

  <p align="center">
    <img src=".assets/image.gif" width="100%" />
  </p>

- Table

  <p align="center">
    <img src=".assets/table.gif" width="80%" />
  </p>

- Code block

  <p align="center">
    <img src=".assets/code_block.gif" width="70%" />
  </p>

- blockquote

  <p align="center">
    <img src=".assets/blockquote.gif" width="70%" />
  </p>

- Alert

  <p align="center">
    <img src=".assets/alert.gif" width="70%" />
  </p>

### 3. Typora interface with unified style

<img align="center" src=".assets/sys.gif" style="zoom:50%;" />

## Custom Configuration

### Interaction Effect Configuration

You can customize the interactive effects of any element to be turned on or off as needed. The specific operations are as follows:

1. Open the `spring.css` file and find the interactive effect configuration options according to the comments at the beginning of the file;

2. Modify the variable value of the corresponding interactive animation as required, `0` means off, `1` means on;

3. Restart Typora to apply the changes.

> [!important]
>
> 1. To enable interactive effects, first set `--use-dynamic-effect` to `1`, and then configure it for specific types.
>
> 2. To turn off all interactive effects, simply set `–use-dynamic-effect` to `0`. (`–use-dynamic-effect` cannot disable some interactive effects of ordered lists. If you want to turn off all interactive effects of ordered lists, set `--list-ol-text-style` to `italic`)

|           Type           |                   Variable Name                   |          Values           |                        Function                         |   Default   |
| :----------------------: | :-----------------------------------------------: | :-----------------------: | :-----------------------------------------------------: | :---------: |
| **Global Configuration** |              `--use-dynamic-effect`               |           0 / 1           | Turn off all interactive effect/ Use interactive effect |      1      |
|            H1            |                `--h1-hover-effect`                |           0 / 1           |                      Close / Open                       |      1      |
|            H2            |                `--h2-after-effect`                |           0 / 1           |                      Close / Open                       |      1      |
|       H3 H4 H5 H6        |               `--h3-6-hover-effect`               |           0 / 1           |                      Close / Open                       |      1      |
|        Paragraph         |                `--p-hover-effect`                 |           0 / 1           |                      Close / Open                       |      1      |
|          Image           |               `--img-hover-effect`                |           0 / 1           |                      Close / Open                       |      1      |
|        Blockquote        |            `--blockquote-hover-effect`            |           0 / 1           |                      Close / Open                       |      1      |
|          Alert           |              `--alert-hover-effect`               |           0 / 1           |                      Close / Open                       |      1      |
|          Strong          |              `--strong-hover-effect`              |           0 / 1           |                      Close / Open                       |      1      |
|          Italic          |                `--em-hover-effect`                |           0 / 1           |                      Close / Open                       |      1      |
|        Underline         |                `--u-hover-effect`                 |           0 / 1           |                      Close / Open                       |      1      |
|       Marked text        |               `--mark-hover-effect`               |           0 / 1           |                      Close / Open                       |      1      |
|       Deleted text       |               `--del-hover-effect`                |           0 / 1           |                      Close / Open                       |      1      |
|       Inline code        |               `--code-hover-effect`               |           0 / 1           |                      Close / Open                       |      1      |
|        Code block        |              `--fence-hover-effect`               |           0 / 1           |                      Close / Open                       |      1      |
|           List           | `--list-marker-effect`<br/>`--list-ol-text-style` | 0 / 1<br/>italic / normal |              Close / Open<br>Close / Open               | 1<br>normal |
|         Divider          |               ` --hr-hover-effect`                |           0 / 1           |                      Close / Open                       |      1      |
|          Table           |              `--table-hover-effect`               |           0 / 1           |                      Close / Open                       |      1      |

## Installation

1. Use the following command in your terminal to clone this repository locally **/** or you can get the stable version compressed package from [Releases](https://github.com/SprInec/typora-spring-theme/releases) and unzip it locally.

    ```bash
    git clone https://github.com/SprInec/typora-spring-theme.git
    ```

2. Click ‘Themes’ in the menu of Typora, and click the ‘Open Theme Folder’ button to open it on the ‘Themes’ page.

3. Copy the file `spring.css` into the opened Typora theme folder.

4. Restart Typora, and then you can choose to use the **Spring** theme in the ‘Themes’ list.

## Todo List

- [x] Light theme SprIng
- [x] Smart Interaction
- [x] Interactive animation configuration
- [ ] HTML export configuration
- [ ] Document layout configuration
- [ ] Dark theme SprIngNight
- [ ] Custom color palette
- [ ] Custom style
- [ ] A variety of interactive effects to choose from
- [ ] [typora-plugin](https://github.com/obgnail/typora_plugin) unified style adaptation

## [Credits](credits.md)

This project is based on *typora-mo-theme* for secondary development of visual and interactive design. The [template](template/) comes from *typora-theme-Jinxiu-template*. 

- [MarMomento/typora-mo-theme](https://github.com/MarMomento/typora-mo-theme)
- [Sophomoresty/typora-theme-Jinxiu](https://github.com/Sophomoresty/typora-theme-Jinxiu)

## License

This project is based on the MIT open source protocol. You can freely copy, modify and distribute the code of this project, but please keep the original author's [LICENSE](LICENSE).

<p align="center">
    <img src="https://api.star-history.com/svg?repos=SprInec/typora-spring-theme&type=Date"/>
</p>
