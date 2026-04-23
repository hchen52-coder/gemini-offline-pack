# Gemini CLI 离线安装包下载器

这个项目使用 GitHub Actions 自动从 npm 下载 @google/gemini-cli 离线包并发布到 GitHub Release。

## 使用方法

### 1. 创建 GitHub 仓库
把这个项目推送到你的 GitHub 仓库。

### 2. 手动触发下载
- 进入你的 GitHub 仓库
- 点击 **Actions** 标签
- 选择 **Download and Release Gemini CLI** 工作流
- 点击 **Run workflow** 按钮
- 可以指定版本号（默认 0.39.0）
- 点击 **Run workflow**

### 3. 下载离线包
工作流运行完成后，进入 **Release** 页面下载生成的 .tgz 文件。

### 4. 本地安装
```bash
# 解压 tgz 文件
tar -xzf google-gemini-cli-0.39.0.tgz

# 安装
npm install -g ./package
```

或者直接将 tgz 文件作为本地包安装：
```bash
npm install -g ./google-gemini-cli-0.39.0.tgz
```

## 版本
当前默认版本：0.39.0