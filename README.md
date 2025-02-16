# 在线音乐播放器功能介绍

## 核心功能
- **搜索音乐**：🔍 通过关键词搜索音乐。
- **音乐播放/暂停**：▶️ 控制音乐播放或暂停。
- **歌词同步显示**：📃 自动同步并显示当前播放歌曲的歌词。
- **播放列表管理**：🎵 管理您的播放列表，轻松添加和移除歌曲。
- **音量控制**：🔊 调节音量大小。
- **进度控制**：⏩ 通过拖动进度条来调整播放位置。
- **迷你播放器**：🎵 当关闭主播放器时自动显示，提供快速控制。

## 界面特点
- **毛玻璃效果设计**：💡 增添界面美观度。
- **响应式布局**：📱 适应各种屏幕尺寸。
- **深色主题**：🌗 提供更好的视觉体验，尤其是在低光环境下。
- **优雅的动画过渡**：🎨 让用户体验更加流畅。
- **直观的交互体验**：👆 易于使用的用户界面。

## 使用方法
### 基础配置
1. 下载项目文件。
2. 部署到任意 Web 服务器。
3. 通过浏览器访问 `index.html` 文件开始使用。

## API 接口

### 搜索接口

```json
// 搜索接口
URL: https://us.jx23.cn/other/test/gcList.php
Method: POST
Params: {
    "content": "string" // 搜索关键词
}
Response: {
    "code": number,  // 200 表示成功
    "msg": "string",   // 响应信息
    "data": [        // 歌曲列表
        {
            "title": "string",  // 歌曲名称
            "artist": "string", // 艺术家
            "mp3": "string",    // 音频文件地址
            "poster": "string", // 封面图片地址
            "lrc": "string"     // 歌词文件地址
        }
    ]
}
```
## API 接口
播放器主要使用以下API接口：
- 搜索功能：支持按歌名、歌手等关键词进行搜索。
- 播放控制：包括播放/暂停、上一首/下一首等功能。
- 歌词显示：自动同步显示当前播放歌词，并高亮当前播放行。
- 迷你播放器：提供在关闭主播放器时的基本控制选项。

## 自定义开发
### 样式修改
主要样式变量位于CSS部分，可以根据需要进行调整。

### 扩展功能
可以通过修改现有代码来添加新的功能，如新的播放控制、自定义搜索逻辑等。

## 注意事项
- 需要现代浏览器支持。
- 建议使用HTTPS协议。
- 确保音频文件支持跨域访问。
- 建议使用CDN加速资源加载。
- 注意处理音频文件的版权问题。

## 技术栈
- HTML5
- CSS3
- JavaScript (ES6+)
- Web Audio API
- Fetch API

## 开源协议
本项目采用 MIT License 开源。

## 贡献指南
欢迎提交Issue和Pull Request来完善这个项目！
1. Fork本仓库。
2. 创建新的功能分支。
3. 提交更改。
4. 发起Pull Request。

## 联系方式
如有问题或建议，欢迎通过Issue反馈！
