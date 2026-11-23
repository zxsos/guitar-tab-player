<div align="center">

# Guitar TAB Player

极简指弹吉他六线谱在线练习播放器，支持连续看谱、逐拍高亮、精细变速与本地产物包导入。

[在线使用](https://zxsos.github.io/guitar-tab-player/) · [配套编配 Skill](https://github.com/zxsos/fingerstyle-guitar-tab-skill)

<a href="https://zxsos.github.io/guitar-tab-player/"><img src="docs/cover.png" width="760" alt="Guitar TAB Player"></a>

</div>

## 特性

- **行业原谱无损直读（内置 `CoderLine/alphaTab`）** — 直接拖入 `.gp` / `.gp3`–`.gp5` / `.gpx` / `.musicxml` / `.mxl` / `.atex` 原谱即可矢量 SVG 无损渲染 + `alphaSynth` 实时吉他音源演奏 + 多音轨切换，并自动提取逐音数据联动 **2D 实时指板**与 **3D 下落轨道**
- **连续无分页看谱 + 逐拍染色** — 按时间轴自动聚焦当前乐句并滚动，点击任意小节即可跳转播放
- **0.25×–1.5× 滑块精细变速** — 支持拖动滑块以 `0.05×` 步进调节与 8 档快捷预设，双引擎同步变速
- **ZIP 一键导入与实时校验** — 打开「导入」窗口或直接拖入原谱文件、`.zip` 产物包、文件夹，自动逐项校验
- **纯前端本地运行零上传** — 所有解包、渲染、音频合成与解码均在浏览器本地完成

## ZIP 产物包结构

```text
*_bundle.zip
├── sync_manifest.json        # 同步时间轴与切片坐标（缺失时自动识谱并支持校准）
├── *.mp3                     # 试听音频（支持 mp3 / wav / m4a / ogg）
├── previews/
│   └── page-*.png            # 高清谱面预览图
└── *.pdf                     # 原版矢量六线谱（可选）
```

可通过配套的 [fingerstyle-guitar-tab-skill](https://github.com/zxsos/fingerstyle-guitar-tab-skill) 一键编配并打包生成新曲目的 `*_bundle.zip`。

## License

[MIT](LICENSE)
