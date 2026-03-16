# Yi Yang Personal Homepage

这是一个纯静态学术主页仓库，页面入口是 `index.html`。

## 当前目录结构

```text
.
├── assets
│   ├── css
│   │   └── styles.css      # 全站样式
│   ├── docs
│   │   └── .gitkeep        # 预留给 CV / Bio / PDF
│   └── images
│       └── .gitkeep        # 预留给头像 / 论文配图 / favicon
├── index.html              # 页面结构与内容
└── README.md
```

## 维护约定

- 页面内容集中改 `index.html`，适合修改个人简介、新闻、论文、经历、奖项。
- 页面样式集中改 `assets/css/styles.css`。
- 头像、论文封面、截图放到 `assets/images/`。
- CV、论文 PDF、个人简介等文件放到 `assets/docs/`，再从 `index.html` 里挂链接。

## 本地预览

在仓库根目录运行：

```bash
python3 -m http.server 4173 --bind 127.0.0.1
```

然后访问 <http://127.0.0.1:4173>。

## GitHub Pages 部署检查

如果想通过 `https://<username>.github.io` 访问，请确认：

1. 仓库名是 `<username>.github.io`。
2. `Settings -> Pages` 已启用，Source 指向正确分支的根目录。
3. `index.html` 位于仓库根目录。
4. 仓库可被 GitHub Pages 正常发布。
