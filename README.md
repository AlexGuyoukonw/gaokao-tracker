# 2027 高考基础学习进度表

这是一个面向华为平板浏览器的轻量学习进度网页。当前统计五科基础学习视频时长：语文、数学、物理、化学、生物。

## 部署到 GitHub Pages

1. 打开仓库 **Settings → Pages**。
2. 在 **Build and deployment** 中选择 **Deploy from a branch**。
3. Branch 选择 **main**，目录选择 **/(root)**，点击 **Save**。
4. 等待 GitHub Pages 发布完成。网站地址：
   https://alexguyoukonw.github.io/gaokao-tracker/

## 华为平板使用

1. 使用华为浏览器打开上面的网址，第一次打开时保持联网。
2. 等页面加载完成后，打开浏览器菜单，选择“添加至桌面”（不同版本菜单文字可能略有不同）。
3. 以后从桌面图标打开即可。首次成功加载后，Service Worker 会缓存网页外壳，尽可能支持离线再次打开。

## 从电脑迁移旧学习记录

1. 在电脑旧版进度表所在的 Chrome 用户资料中，使用旧版导出脚本导出 JSON 备份。
2. 在华为平板打开：
   https://alexguyoukonw.github.io/gaokao-tracker/import.html
3. 选择电脑传到平板的 JSON 备份，确认导入。
4. 页面会返回主进度表。请核对五科累计时长、总进度和历史记录。

## 数据与隐私说明

- 学习记录只保存在当前浏览器站点的 LocalStorage 和 IndexedDB 中；不会自动上传到 GitHub。
- GitHub 仓库中的网页源代码是公开的，但个人学习记录不包含在仓库文件中。
- 更换浏览器、清除站点数据或重置设备前，请先另行备份学习记录。
- Service Worker 缓存的是网页程序文件，不是学习数据；它不是云端同步或独立备份。
