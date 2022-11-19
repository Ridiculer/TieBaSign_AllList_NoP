# 贴吧签到Github Action版

## 今日签到状态

![Baidu Tieba Auto Sign](https://github.com/Ridiculer/TieBaSign_AllList_NoP/workflows/Baidu%20Tieba%20Auto%20Sign/badge.svg)

## 2022-8-23
fork别人的拿来用的，自测可以全关注列表都签到，其他人的都只能签200个。

本来的main里有个send_mail会导致出错我直接删除了

签到时间设置是每天的00:05和6:05，可以自行在workflows/main.yml里面的cron中修改，注意github采用的是美国的时区，实际上要比国内晚8个小时

## 2022-11-19
更新了工作环境的python版本，原来的版本在gtihub中已经不适用


## 使用说明

1. Fork 本仓库，然后点击你的仓库右上角的 Settings，找到 Secrets 这一项，添加一个库秘密变量。其中 `BDUSS` 存放你的 BDUSS。支持同时添加多个帐户，BDUSS 之间用 `#` 隔开即可。

2. 设置好环境变量后点击你的仓库上方的 `Actions` 选项，第一次打开需要点击 `I understand...` 按钮，确认在 Fork 的仓库上启用 GitHub Actions 。

3. 任意发起一次commit，可以参考下图流程修改readme文件。

- 打开`README.md`，点击修改按钮
- 修改任意内容，这里在末尾插入了空格。移动到最下面，点击提交。

4. 至此自动签到就搭建完毕了，可以再次点击`Actions`查看工作记录，如果有`Baidu Tieba Auto Sign`则说明workflow创建成功了。点击右侧记录可以查看详细签到情况。

 


