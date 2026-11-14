# Aaim · Linux 版

常驻 Linux 桌面的 AI 助手介绍页 —— 单个 `index.html`，内联全部 CSS / JS / 图标，无外部依赖。

**在线预览：** https://lugui906.github.io/aaiml/

## 下载

| 项目 | 值 |
|---|---|
| 文件 | `aaim_1.3.4_amd64.deb` |
| 版本 | 1.3.4 |
| 架构 | amd64（x86_64） |
| 大小 | 62,493,196 字节（约 59.6 MB） |
| Installed-Size | 116,664 KB |
| 包名 | `aaim` |
| 依赖 | python3 ≥ 3.10、python3-gi、gir1.2-gtk-4.0、tesseract-ocr、tesseract-ocr-chi-sim |
| 安装位置 | `/opt/aaim`；`/usr/bin/aaim` 是指向它的软链接 |
| 用户数据 | `~/.aaim` |
| 下载地址 | https://wwaye.lanzoue.com/ibgna4fzv35e |
| 提取密码 | `hqb2` |
| SHA-256 | `32875f24e8953e56dbda0af1e580ed6782303ca1272fa34486f2ed460ddcc7ca` |

安装：

```bash
sudo apt install ./aaim_1.3.4_amd64.deb
```

用 `apt` 而非 `dpkg -i`，让系统自动补依赖。deb 自带精简 Java 运行时与 Office 的 Python 依赖
（python-docx / openpyxl / python-pptx），目标机不需要联网 pip 安装。

## 本地查看

```bash
xdg-open index.html
# 或
python3 -m http.server 8000
```

## 说明

页面内容依据 deb 包元数据（`dpkg-deb -f` / `-c`）与随包文档编写。deb 本体不在此仓库。
