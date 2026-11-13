$readmeContent = @"
# nclash (Modified Version)

基于原项目 [FlClash](https://github.com/chen08209/FlClash) 修改与优化。

## 修改说明
在原作者优秀代码的基础上，本版本进行了以下定向优化：
- **内核升级**：核心已平滑升级至 v0.8.99 版本，提升协议兼容性与安全性。
- **性能优化**：开启 Android R8 极致混淆与资源压缩，减小 APK 体积，提升加载效率。
- **纯净界面**：彻底移除了原版移动端右上角的 PRE / DEBUG 调试标记，提供更纯净的视觉体验。
"@
$readmeContent | Set-Content README.md
..\git\cmd\git.exe add README.md
..\git\cmd\git.exe commit -m "docs: update project description"
..\git\cmd\git.exe -c http.proxy=socks5://127.0.0.1:10808 push https://hvos-cn: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@github.com/hvos-cn/nclash.git main
