<h1 align="center">
  Alist-MikananiRss
</h1>
<p align="center">
  从<a href="https://mikanani.me/">蜜柑计划</a>的RSS订阅源中自动获取番剧更新并通过Alist离线下载至对应网盘
</p>  
<p align="center">
  并结合使用ChatGPT分析资源名，将资源重命名为Emby可解析的格式。（现为纯自用脚本分享，代码质量差请见谅）
</p>  

## 准备工作 
1. 请自行参照[Alist](https://github.com/alist-org/alist)项目文档部署Alist，并搭建好Aria2离线下载（暂未支持QBit）
2. 自行注册蜜柑计划账户，订阅番剧，获取订阅链接

## 如何使用
1. 下载源码
```shell
git clone https://github.com/TwooSix/Alist-MikananiRss.git && cd Alist-MikananiRss
```
2. 安装依赖(Python==3.11)
```shell
pip install -r requirements.txt
```
3. 在目录下新建一个`config.py`配置文件，并填写配置文件，具体填写示例见`example.py`

4. 运行代码：`python main.py`  

5. Enjoy

## 开启订阅更新通知（可选）
### Telegram 通知
在`config.py`中加入以下配置
```python
TELEGRAM_NOTIFICATION = True # 开启Telegram通知，为 False 则关闭
BOT_TOKEN = "你的 BOT_TOKEN"
USER_ID = "你的 USER_ID"
```

## 重命名效果展示
<div align=center>
<img src="https://github.com/TwooSix/Alist-MikananiRss/blob/master/imgs/show_pic1.png"/>
</div>

