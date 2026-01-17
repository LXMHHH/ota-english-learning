# OTA英语学习工具 - Streamlit Cloud 部署指南

## 📱 部署到Streamlit Cloud（免费）

### 前提条件
- ✅ GitHub账号（你已经有了）
- ✅ Streamlit Cloud账号（使用GitHub登录即可）

---

## 🚀 部署步骤

### 第一步：准备GitHub仓库

1. **登录GitHub** (https://github.com)

2. **创建新仓库**
   - 点击右上角 "+" → "New repository"
   - 仓库名称：`ota-english-learning`
   - 设置为 **Public**（公开仓库，免费部署）
   - 勾选 "Add a README file"
   - 点击 "Create repository"

3. **上传项目文件**
   
   方式一：通过GitHub网页上传
   - 在仓库页面点击 "Add file" → "Upload files"
   - 将以下文件拖拽上传：
     ```
     ota-english-cloud/
     ├── app.py              ← 主程序
     ├── requirements.txt    ← 依赖包
     └── .streamlit/
         └── config.toml     ← 配置文件
     ```
   - 点击 "Commit changes"

   方式二：使用Git命令（如果你熟悉Git）
   ```bash
   cd ota-english-cloud
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/你的用户名/ota-english-learning.git
   git push -u origin main
   ```

---

### 第二步：部署到Streamlit Cloud

1. **访问Streamlit Cloud**
   - 打开 https://share.streamlit.io/
   - 点击 "Sign in with GitHub"
   - 授权Streamlit访问你的GitHub账号

2. **创建新应用**
   - 点击 "New app"
   - 选择你的仓库：`你的用户名/ota-english-learning`
   - Branch: `main`
   - Main file path: `app.py`
   - App URL: 自定义一个网址（例如：`ota-english`）

3. **点击 "Deploy!"**
   - 等待2-3分钟，Streamlit会自动安装依赖并启动应用
   - 部署成功后会显示你的应用链接

4. **获取应用链接**
   - 你的应用链接格式：`https://你的用户名-ota-english-learning-app-xxxxx.streamlit.app`
   - 这个链接可以在任何设备上访问！

---

## 📱 添加到手机主屏幕（像APP一样使用）

### iPhone/iPad (Safari)

1. 在Safari浏览器打开你的应用链接
2. 点击底部的 **分享按钮** (方框带向上箭头)
3. 向下滚动，找到 **"添加到主屏幕"**
4. 点击 **"添加"**
5. 完成！现在你的主屏幕上有一个OTA英语学习的图标了

### Android (Chrome)

1. 在Chrome浏览器打开你的应用链接
2. 点击右上角 **三个点菜单**
3. 选择 **"添加到主屏幕"** 或 **"安装应用"**
4. 点击 **"添加"**
5. 完成！应用图标会出现在主屏幕上

---

## 🎯 使用效果

添加到主屏幕后：
- ✅ 像原生APP一样打开（全屏显示）
- ✅ 没有浏览器地址栏
- ✅ 可以离线缓存部分内容
- ✅ 随时随地学习OTA英语

---

## 🔧 更新应用

如果你想修改应用内容：

1. 在GitHub仓库中编辑文件
2. 提交更改（Commit changes）
3. Streamlit Cloud会自动检测更改并重新部署
4. 等待1-2分钟，刷新应用即可看到更新

---

## 💡 常见问题

### Q: 部署是免费的吗？
A: 是的！Streamlit Cloud提供免费的公开应用托管。

### Q: 应用会一直在线吗？
A: 是的，只要你的GitHub仓库存在，应用就会一直在线。如果长时间无人访问，应用会进入休眠状态，首次访问时需要几秒钟唤醒。

### Q: 可以设置为私有应用吗？
A: 免费版只支持公开应用。如果需要私有应用，需要升级到付费版。

### Q: 手机上使用流畅吗？
A: 非常流畅！应用已经针对手机屏幕优化，支持触摸操作。

### Q: 可以分享给同事使用吗？
A: 当然可以！直接把应用链接发给他们即可。

---

## 📞 需要帮助？

如果部署过程中遇到问题：
1. 检查 `requirements.txt` 文件是否正确
2. 查看Streamlit Cloud的部署日志（Logs）
3. 确保所有文件都已上传到GitHub

---

## 🎉 完成！

现在你有了一个：
- 📱 可以在手机上使用的OTA英语学习APP
- 🌐 可以随时随地访问的在线应用
- 🔄 可以随时更新内容的灵活工具
- 👥 可以分享给团队使用的学习平台

开始你的OTA英语学习之旅吧！🚀
