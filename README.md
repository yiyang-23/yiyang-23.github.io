# Yi Yang Personal Homepage

这是一个纯静态个人主页，入口文件是 `index.html`。

## 为什么会“打不开”？
常见原因通常不是代码本身，而是运行方式或部署设置：

1. **直接双击打开文件**（`file://`）在部分环境下会有样式或资源加载异常。  
2. **GitHub Pages 没有启用**，或者仓库还没设为公开。  
3. 网络环境无法访问 Google Fonts（已在本次修改中移除外链字体依赖）。

## 本地打开（推荐）
在仓库根目录运行：

```bash
python3 -m http.server 4173 --bind 127.0.0.1
```

然后访问：

- <http://127.0.0.1:4173>

## GitHub Pages 部署检查
如果你想通过 `https://<username>.github.io` 访问，请确认：

1. 仓库名正确（用户主页仓库应为 `<username>.github.io`）。
2. `Settings -> Pages` 已启用，Source 指向正确分支（通常 `main` / root）。
3. `index.html` 位于仓库根目录。
4. 仓库为公开（或使用支持私有仓库 Pages 的方案）。
