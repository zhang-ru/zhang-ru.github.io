# 部署PicGO


昨日刚刚把博客搭好，文字可以随便的写了，但是还有一个问题就是Markdown中要包含图片就需要有图床了。我在网上找教程的过程中，发现了图床管理工具PicGo。

PicGo除了有需要安装的桌面版，在Vs Code中也有扩展工具，只需要在扩展市场中搜索并安装就好了（***推荐***）。使用起来也比较简单，在设置中找到，按照指示填写即可：

![20210125100505](https://cdn.jsdelivr.net/gh/zhang-ru/imagebed@main/img/20210125100505.png)

![20210125100639](https://cdn.jsdelivr.net/gh/zhang-ru/imagebed@main/img/20210125100639.png)


### 关于图床的选择
我先后尝试了Github、七牛、Gitee、SMMS这几个，设置步骤也都大差不差，这里主要说说缺点吧：
- Github:国内图片不显示，需要TZ才能正常显示
- 七牛：存储空间网址30天会更新一次，意味着要一个月进行一次设置
- Gitee:VS Code的PicGo插件不支持
- SMMS:空间有限，5GB

### 我的选择
在我试了各种图床后准备选择SMMS的时候，偶然看到一篇[博客](https://www.pianshen.com/article/81731334012/)说到Github可以用CDN加速的办法解决国内访问速度的问题。本着Geek能用Github就要用Github的精神（~~穷~~），我最终转回了Github的怀抱。这里学到的知识点就是代理路径：
> https://cdn.jsdelivr.net/gh/[用户名]/[仓库名]@[分支名]

