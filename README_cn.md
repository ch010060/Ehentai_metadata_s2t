# 本分支專案摘要
此分支專案是原專案 Ehentai metadata 插件的繁體中文版

*Note*
1. 本插件使用的opencc原始碼來自 opencc-python (https://github.com/yichen0831/opencc-python). License: Apache License 2.0
2. 本插件使用的資料來自 OpenCC (https://github.com/BYVoid/OpenCC). License: Apache License 2.0
3. Python軟體基金會原始碼 (GPL Compatible)
4. 本插件使用的部分函式來自 TradSimpChinese (https://github.com/Hopkins1/TradSimpChinese). Licenese: GPL3

- - -
<img src="/image/telegram.png" width="200" height="200" alt="插件开发"/>


[![Telegram](/image/TelegramBots.svg)](https://t.me/+TAT5NFNLhI83MTc1)

这个插件可以从[E站](https://e-hentai.org/)上下载本子的元数据。

**主要特点**

- 这个插件可以下载题名、作者、评分、tags、封面。
- 如果你输入了你在`exhentai.org`的cookies，这个插件可以从[ExHentai.org](https://exhentai.org/)上下载元数据。

**一些需要注意的事**

- 由于E-Hentai并没有独立的作者字段，插件所提供的题名与作者是通过正则表达式识别出来的。
- 由于E站的特殊性，大陆地区需要使用梯子，插件才能正常运行
- 适用于calibre中python3的所有版本

**安装方法**

1. 打开calibre客户端，选择界面中的首选项
2. 进入之后我们选择，从文件中加载插件选项
3. 选择我们下载好的插件zip安装包，选择插件路径
4. 然后就会提示我们是否安装插件我们选择是
5. 选择完之后，插件安装完成
6. 若有其它警告一律选是，重启客户端后看是否安装成功

**数据库配置**

1. 安装好插件后
2. 将数据库文件（EhTagTranslation.db）安装在你想保存位置
3. 在插件中勾选Chinese_Exhentai，再在下面EhTagTranslation_db文本框中输入数据库文件位置。如：

&emsp;&emsp;&emsp;&emsp;位置为E:\Code\python\Ehentai_metadata\EhTagTranslation.db

&emsp;&emsp;&emsp;&emsp;文本框中填写E:\Code\python\Ehentai_metadata


**特别感谢**

该插件由wuyingren的[doujinshi_metadata_plugins](https://github.com/yingziwu/doujinshi_metadata_plugins)思路改写。

该数据库来自EhTagTranslation的[Database](https://github.com/EhTagTranslation/Database)数据改造而来

**版本历史**

**Version 2.3.2** - 2022-11-22

- 优化插件搜索能力
- 去除Chinese Tags复选框


**Version 2.3.1** - 2022-11-07

- 修复e站改版数据搜索不到问题


**Version 2.3.0** - 2022-8-21

- 去除上传者标签
- 解决存在多个画师和社团时只会添加一个问题


**Version 2.2.7** - 2022-8-20

- 解决在Calibre 6版本Accurate_Label闪退问题


**Version 2.2.6** - 2022-5-4

- 解决在本子语言是英语或未定义的情况下把 tag 转为单词首字母大写
- 在语言未定义的情况下, 可以根据是否具有日文标题来设定漫画的语言为日语
- 修复一些小问题


**Version 2.2.5** - 2022-4-21

- 增加自定义代理的选项


**Version 2.2.4** - 2022-4-17

- 修改从标题中获取作者等信息的正则表达式
- 增加了解析到的元信息的种类
- 正确处理漫画具有多语言的情况


**Version 2.2.3** - 2022-4-5

- 将accurate_url的输入改为弹出框输入
- 选择Accurate_Label后插件将会从输入的e站accurate_url：https://exhentai.org/g/21843\*\*/175ff141\*\*/来获取标签数据



**Version 2.2.2** - 2022-4-3

- 增加复选框Accurate_Label
- 选择Accurate_Label后插件将会从输入的e站accurate_url：https://exhentai.org/g/21843\*\*/175ff141\*\*/来获取标签数据


**Version 2.2.1** - 2022-4-2

- 增加复选框Chinese Tags
- 选择Chinese Tags后插件将只搜索中文本子来获取标签数据，降低获取时间


**Version 2.2.0** - 2022-3-31

- 增加是否翻译功能
- 更改翻译数据库方式，需要手动添加数据源


**Version 2.1.1** - 2022-3-30

- 解决无法进入里站问题
- cookie填写项增加igneous值


**Version 2.1.0** - 2021-8-25

- 将标签变得更简洁
- 将部分标签改为中文



**Version 1.1.0** - 2021-4-5

- Initial release

