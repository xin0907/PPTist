<p align="center">
    <img src='/public/icons/android-chrome-192x192.png' />
</p>

<p align="center">
    <a href="https://www.github.com/pipipi-pikachu/PPTist/stargazers" target="_black">
        <img src="https://img.shields.io/github/stars/pipipi-pikachu/PPTist?logo=github" alt="stars" />
    </a>
    <a href="https://www.github.com/pipipi-pikachu/PPTist/network/members" target="_black">
        <img src="https://img.shields.io/github/forks/pipipi-pikachu/PPTist?logo=github" alt="forks" />
    </a>
    <a href="https://www.github.com/pipipi-pikachu/PPTist/blob/master/LICENSE" target="_black">
        <img src="https://img.shields.io/github/license/pipipi-pikachu/PPTist?color=%232DCE89&logo=github" alt="license" />
    </a>
    <a href="https://www.typescriptlang.org" target="_black">
        <img src="https://img.shields.io/badge/language-TypeScript-blue.svg" alt="language">
    </a>
    <a href="https://github.com/pipipi-pikachu/PPTist/issues" target="_black">
        <img src="https://img.shields.io/github/issues-closed/pipipi-pikachu/PPTist.svg" alt="issue">
    </a>
</p>


# 🎨 PPTist
> 一个基于 Vue3.x + TypeScript 的在线演示文稿（幻灯片）应用，还原了大部分 Office PowerPoint 常用功能，支持 文字、图片、形状、线条、图表、表格、视频、音频、公式 几种最常用的元素类型，每一种元素都拥有高度可编辑能力，同时支持丰富的快捷键和右键菜单，力求还原桌面应用级体验。支持导出本地 PPTX 文件，支持移动端基础编辑和预览。您可以在此基础上搭建自己的在线幻灯片应用。

<b>在线体验地址👉：[https://pipipi-pikachu.github.io/PPTist/](https://pipipi-pikachu.github.io/PPTist/)</b>


# 👀 前排提示
1. 本项目是一个 “Web 幻灯片应用” ，而不是 “低代码平台”、“H5 编辑器”、“图片编辑器” 、“白板应用”等。
2. 本项目的目标受众是<b>有【Web 幻灯片】开发需求的开发者</b>，提供的链接只是一个演示地址，不提供任何在线服务。你不应该直接将本项目作为工具使用，也不支持一键部署。
如果你只是需要一个服务或工具，可以选择更优秀和成熟的产品，例如：[石墨文档](https://shimo.im/)、[金山文档](https://www.kdocs.cn/)、[Slidev](https://sli.dev/)、[revealjs](https://revealjs.com/) 等。
3. 本项目是基于 DOM 的渲染方案，优点是简单易上手。但是相比 Canvas 渲染的方案，在复杂场景下性能会存在一定的差距，所以如果你对性能有较高的要求，本项目可能不是一个好的选择/参考方向。
4. 这里总结了一些[常见问题](https://github.com/pipipi-pikachu/PPTist/blob/master/doc/Q&A.md)，第一次提 Issues 和 PR 时，务必提前阅读此文档。


# 🚀 项目运行
```
npm install

npm run dev
```


# 📚 功能列表
### 基础功能
- 历史记录（撤销、重做）
- 快捷键
- 右键菜单
- 导出本地文件（PPTX、JSON、图片、PDF）
- 导入导出特有 .pptist 文件
- 打印
### 幻灯片页面编辑
- 页面添加、删除
- 页面顺序调整
- 页面复制粘贴
- 背景设置（纯色、渐变、图片）
- 设置画布尺寸
- 网格线
- 标尺
- 画布缩放、移动
- 主题设置
- 演讲者备注（富文本）
- 幻灯片模板
- 翻页动画
- 元素动画（入场、退场、强调）
- 选择面板（隐藏元素、层级排序、元素命名）
- 查找/替换
- 批注
### 幻灯片元素编辑
- 元素添加、删除
- 元素复制粘贴
- 元素拖拽移动
- 元素旋转
- 元素缩放
- 元素多选（框选、点选）
- 多元素组合
- 多元素批量编辑
- 元素锁定
- 元素吸附对齐（移动和缩放）
- 元素层级调整
- 元素对齐到画布
- 元素对齐到其他元素
- 多元素均匀分布
- 拖拽添加图文
- 粘贴外部图片
- 元素坐标、尺寸和旋转角度设置
- 元素超链接（链接到网页、链接到其他幻灯片页面）
#### 文字
- 富文本编辑（颜色、高亮、字体、字号、加粗、斜体、下划线、删除线、角标、行内代码、引用、超链接、对齐方式、序号、项目符号、段落缩进、清除格式）
- 行高
- 字间距
- 段间距
- 首行缩进
- 填充色
- 边框
- 阴影
- 透明度
- 竖向文本
#### 图片
- 裁剪（自定义、按形状、按纵横比）
- 滤镜
- 着色（蒙版）
- 翻转
- 边框
- 阴影
- 替换图片
- 重置图片
- 设置为背景图
#### 形状
- 绘制任意多边形
- 绘制任意线条（未封闭形状模拟）
- 替换形状
- 填充色
- 边框
- 阴影
- 透明度
- 翻转
- 形状格式刷
- 编辑文字（支持富文本，与文字元素的富文本编辑功能近似）
#### 线条
- 颜色
- 宽度
- 样式
- 端点样式
#### 图表（柱状图、条形图、折线图、面积图、散点图、饼图、环形图）
- 图表转换
- 数据编辑
- 背景填充
- 主题色
- 坐标系与坐标文字颜色
- 其他图表设置
- 边框
- 图例
#### 表格
- 行、列添加删除
- 主题设置（主题色、表头、汇总行、第一列、最后一列）
- 合并单元格
- 单元格样式（填充色、文字颜色、加粗、斜体、下划线、删除线、对齐方式）
- 边框
#### 视频
- 预览封面设置
- 自动播放
#### 音频
- 图标颜色
- 自动播放
- 循环播放
#### 公式
- LaTeX编辑
- 颜色设置
- 公式线条粗细设置
### 幻灯片放映
- 全部幻灯片预览
- 画笔、黑板工具
- 计时器工具
- 激光笔
- 自动放映
- 演讲者视图
### 移动端
- 基础编辑
    - 页面添加、删除、复制、备注、撤销重做
    - 插入文字、图片、矩形、圆形
    - 元素通用操作：移动、缩放、旋转、复制、删除、层级调整、对齐
    - 元素样式：文字（加粗、斜体、下划线、删除线、字号、颜色、对齐方向）、填充色
- 基础预览
- 播放预览


# 🎯 开发
目前没有完整的开发文档，但下面这些文档可能会对你有一些帮助：
- [项目目录与数据结构](https://github.com/pipipi-pikachu/PPTist/blob/master/doc/DirectoryAndData.md)
- [画布与元素的基本原理](https://github.com/pipipi-pikachu/PPTist/blob/master/doc/Canvas.md)
- [如何自定义一个元素](https://github.com/pipipi-pikachu/PPTist/blob/master/doc/CustomElement.md)


# 📄 版权声明/开源协议
[AGPL-3.0 License](https://github.com/pipipi-pikachu/PPTist/blob/master/LICENSE) | Copyright © 2020-PRESENT [pipipi-pikachu](https://github.com/pipipi-pikachu)

# 🧮 商业用途
- 如果你希望将本项目商用盈利，我希望你能尊重开源，严格遵循 AGPL-3.0 协议，回馈开源社区；
- 如果你因为任何原因，必须要闭源商用，无法执行 AGPL-3.0 协议，可以选择：
    1. 使用早期的 [Apache 2.0 LICENSE 版本](https://github.com/pipipi-pikachu/PPTist/archive/f1a35bb8e045124e37dcafd6acbf40b4531b69aa.zip)（建议）；
    2. 成为项目的贡献者，大致包括：
        - 你的代码被本项目作为依赖引用；
        - 你给本项目提交过重要的 PR 并且被合并；
        - 你参与过本项目的设计，也包括对各种功能/模块的实现或Bug的修复提供了有价值的思路；
        - 注1：满足条件的单位在商用前请先联系作者确认资格，避免误会。
        - 注2：先违反协议后再成为贡献者不在此项范围；
    3. 邮件联系作者付费商用（如果可以，我更希望你一起加入到开源社区中来）；