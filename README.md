FFmpeg 音视频格式转换命令清单
这个仓库整理了 macOS 环境下使用 FFmpeg 进行音频提取、视频格式转换的常用命令，涵盖无损提取、格式兼容、设备适配等场景，适合需要高效处理音视频文件的开发者和爱好者。
📂 仓库文件说明
文件名	内容说明
音频提取转换常用命令清单.md	包含从视频中提取音频、音频格式转换（如 WAV→FLAC、AAC→MP3）的详细命令及参数说明
视频格式转换常用命令清单.md	包含视频格式转换（如 MP4→MKV、H.264→H.265）、压缩、设备适配、批量处理等场景的命令集合
🚀 快速使用前提
确保你的 macOS 已安装 FFmpeg：
bash
# 若未安装 Homebrew，先执行以下命令安装（国内推荐清华源）
/bin/bash -c "$(curl -fsSL https://cdn.jsdelivr.net/gh/ineo6/homebrew-install/install.sh)"

# 安装 FFmpeg
brew install ffmpeg
🔍 命令分类导航
音频相关
音频提取（从视频中分离音频）
无损音频转换（WAV→FLAC 等）
有损音频转换（MP3、AAC 等压缩格式）
多音轨处理与批量操作
视频相关
基础格式转换（MP4↔MKV 等）
视频压缩（降低码率 / 分辨率）
[H.265/HEVC 高效编码](视频格式转换常用命令清单.md# 三、H.265/HEVC 编码（高效压缩）)
设备适配（iPhone、安卓、电视）
视频片段截取与帧提取
批量视频处理
❓ 常见问题
命令执行报错 ffmpeg: command not found请确认已通过 Homebrew 成功安装 FFmpeg，或检查终端的环境变量配置。
转换后音质 / 画质不符合预期可调整命令中的码率（-b:v/-b:a）、压缩级别（-compression_level）、质量系数（-crf/-q:a）等参数，具体参考对应命令的说明。
如果在使用过程中遇到问题，欢迎在仓库中提交 Issue，或根据命令清单中的参数说明自行调整。
