# | AiNiee-ChatGPT:AI翻译改变世界RPG!
<p align="center">
  <a href="https://github.com/NEKOparapa/AiNiee-chatgpt">
    <img src="https://github.com/Abcuders/AiNiee-chatgpt/blob/main/Example%20image/logo.png">
  </a>
<p>

***
[![ GitHub 许可证](https://img.shields.io/github/license/NEKOparapa/AiNiee-chatgpt)](https://github.com/NEKOparapa/AiNiee-chatgpt/LICENSE) [![GitHub release](https://img.shields.io/github/v/release/NEKOparapa/AiNiee-chatgpt)](https://github.com/NEKOparapa/NEKOparapa/releases/)
> 这是一款基于`Mtool`或`Translator++`的 chatgpt自动批翻译工具,主要是用来翻译各种RPG游戏
> [教程视频](https://www.bilibili.com/video/BV18c411K7WN) [下载地址](https://github.com/NEKOparapa/AiNiee-chatgpt/releases)
# 🏕️ 环境支持
***
 * ℹ️要使用本工具您必须需要`🐍Python3环境` `🟪好用的魔法工具` `🔵Mtool/🔴Translator++` `🤖Chat-GPT`的支持
 
# 💡 提醒&帮助&常见问题建议
 ***
 * **`🐍Python3环境`**:您可以在[🐍Python官网](https://www.python.org/downloads/windows/)下载合适的版本进行安装,我们建议安装3.10及以上的版本,同时我们建议也不要安装3.8版本,可能出现会**无法兼容**的问题(群友反馈)
   >  🐍Python使用的AI相关库和UI相关库:`openai` `PyQt5` `PyQt-Fluent-Widgets[full]` `openpyxl` `sentence-transformers`
   
   您可以使用`Cmd` `PowerShell`等Shell**进入项目目录**运行以下命令通过`清华源`以安装相关依赖(注意不要直接使用pip进行install,因为可能导致**Fatal error in launcher: Unable to create process using pip问题❗❗❗**的发生),也可以运行我们的`自动依赖安装脚本`,相关介绍放在后文
   ``` 
   python3 -m pip install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple
   ```
   
 * **`🟪好用的魔法工具`**:我们**强烈建议**您选择优质稳定的代理工具,不然api接口会频繁报错无法连接,错误代码443或者一直没有回复
 * **`🔵Mtool/🔴Translator++`**:[🔵Mtool下载地址](https://afdian.net/a/AdventCirno?tab=feed)  [🔴Translator++下载地址](https://dreamsavior.net/download/)[🔴Translator++ Github简体中文文档地址](https://github.com/zyf722/TranslatorPlusPlusChineseWiki)
   > 两者免费版本就可以,新人推荐Mtool,如果希望能够自行校正,构建用户词典,获得更好的翻译效果,推荐Translator++
* **`🤖Chat-GPT`**:建议您新建一个API_Key,并且最好在使用期间不要和其他程序一起使用,不然容易达到请求次数限制,现在有很多店铺卖10-30的120美元余额的key或者账号,可以翻译十几个游戏（我们没有店铺,不提供任何代购帮助）
* **`💾IDE软件`**:我们建议您使用`VScode` `pycharm` 等软件[VScode下载地址](https://code.visualstudio.com/)
* <b>😏经过几个版本的优化,从以前的翻译1mb大小json文件花费3刀左右,已经减少到1.5刀左右,所以大家在进行翻译前,掂量一下自己的账号余额</b>
* <b>特别注意,在翻译到最后99%时,因为要处理难翻译的文本,所以要处理蛮长一段时间,输出日志更新很慢,要保持耐心等待(除非频繁报错)</b>

# 📝使用方法
***
> 🆗在您检查所有的环境依赖都安装完毕了,请按照下面的步骤进行操作
* 1.🖱️首先双击运行`初始化依赖环境.cmd`,安装完成后会自动生成一个`启动AiNiee-chatgpt4.cmd`文件在项目目录下(**如果您已手动安装完🐍Python依赖,也请运行这一步,脚本不会再安装一次,`启动AiNiee-chatgpt4.cmd也会自动生成的`**)
* 2.🖱️双击`启动AiNiee-chatgpt4.cmd`,在账号设置页面配置你的账号信息以及`API KEY`
    > 🔥官方账号配置示例:<br>
    > <img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/官方账号设置.png" width="400" height="300"><br>
    > 官方账号配置说明:<br>
    > `启用该平台`: 如果使用该平台的AI进行翻译,请勾上<br>
    >`账号类型`: 是你账号类型,免费用户基本只能并发两三个线程翻译任务,而付费用户可以并发几十个,大幅缩减翻译时间<br>
    > `模型选择`: 默认都是GPT3.5,如果你的账号获得了GPT4的使用资格,请选择付费账号（48h后）和模型gpt-4来进行翻译,并且可以把Lines设置为80<br>
    >`API KEY`: 填入你的api_key<br>
    >`代理地址`: 可以不输入,如果需要设置代理时,再则填入http://<代理ip>:<代理端口>,示例：`http://127.0.0.1:10081`<br>

    > 🎐代理账号配置示例:<br>
    > <img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/代理账号设置.png" width="400" height="300"><br> 
    > 代理账号配置说明:<br>
    >`API KEY`: 填入国内代理平台给你生成的API KEY<br>
    >`域名地址`: 填入国内代理平台提供的请求地址,如OpenAI-sb平台提供的请求地址是`api.openai-sb.com`,则填入：`https://api.openai-sb.com/v1`
* 3.✅点击请求测试,测试网络是否通畅,请求是否成功
    ><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/请求成功.png" width="400" height="300"> 
* 4-1.如果使用`🔵Mtool`进行翻译请根据以下步骤操作
    > 1.使用Mtool打开游戏,并在翻译功能界面,选择导出游戏原文文件,会在游戏根目录生成：ManualTransFile.json<br>
    ><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Mtool/导出原文1.png" width="400" height="300"><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Mtool/导出原文2.png" width="400" height="300"><br>
    > 2.在`AiNiee-chatgpt`界面选择`🔵Mtool项目`,并配置翻译设置<br>
    >配置示例:<br>
    ><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Mtool/翻译设置Mtool.png" width="400" height="300"><br>
    >配置说明:<br>
    >`Lines`: 是每次请求翻译的文本行数。行数设置越大,整体的翻译效果会更好,上下文更加流畅,但每次请求回复速度会越慢,回复的内容越容易出错,建议gpt3.5模型不要设置超过50,gpt4模型不超过90<br>
    >`错行检查`: 是针对AI回复内容的检查功能,因为AI在翻译时有时会把上下文一起翻译,并放到一个文本行中,导致回复的文本错行,对不上原文。开启这个功能,会对AI回复内容进行检查,会增加时间和花销,追求翻译质量可开<br>
    >`Prompt`: 是系统提示词,用于告诉chatgpt任务目标的命令语。希望大家有空去探索一下Prompt的写法,如果写得越好,AI酱就能更能准确回复译文格式,以你想要的写作风格进行翻译。只要在Prompt里加上"以json文件格式回复译文",程序就能够处理<br>
    >`文件位置`: 是选择你需要翻译的原文文件,也是ManualTransFile.json文件
    >`输出文件夹`: 是选择翻译后文件的存储文件夹<br>
* 5-1.🖱️点击**开始翻译**按钮,看控制台输出日志或者进度条。之后等待翻译进度到百分百,自动生成翻译好的文件Tradata.json在输出文件夹中
    > 正在进行翻译<br>
    ><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Mtool/控制台正在翻译.png" width="400" height="300"><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Mtool/UI界面正在翻译.png" width="400" height="300">
   
   😪这个过程比较煎熬,通常我翻译1mb的json文件,就得花一个小时左右,免费玩家就是这样的,而付费玩家,使用多线程功能,可以基本在20分钟左右翻译完成

    > 已经完成翻译<br>
    ><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Mtool/控制台翻译完成.png" width="400" height="300"><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Mtool/UI界面翻译完成.png" width="400" height="300">

   回到`🔵Mtool`工具,依然在翻译功能界面,选择加载翻译文件,选择Tradata.json文件即可
    > <img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Mtool/导入译文.png" width="400" height="300"> 

* 4-2.如果使用`🔴Translator++`进行翻译请根据以下步骤操作
    > 1.🖱️打开`🔴Translator++`,选择“start a new project”,根据你的游戏图标来选择对应的游戏引擎<br>
    ><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Tpp/新建工程1.png" width="400" height="300"><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Tpp/新建工程2.png" width="400" height="300"><br>
    > 2.选择你的游戏文件,创建新工程,软件会自动解包和导入游戏数据<br>
    ><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Tpp/新建工程3.png" width="400" height="300"><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Tpp/新建工程4.png" width="400" height="300">

  当弹出提示框,问你：**Do you  also want to load JavaScript files**时,选择**Cancel**,加载脚本里的文本修改容易出错,而且大多都是脚本注释,翻译了也没用

    > 3.🖱️点"Options"按钮,选择"Preferences",选择"UI Language",选择简体中文,方便之后操作<br>
    ><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Tpp/汉化设置1.png" width="400" height="300"><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Tpp/汉化设置2.png" width="400" height="300"><br>
    > 4.点左上角的导出工程,选择导出格式为XML格式到你指定的文件夹,生成data文件夹<br>
    ><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Tpp/导出工程1.png" width="400" height="300"><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Tpp/导出工程2.png" width="400" height="300">
 
  当弹出提示框,问如何处理标记列,就点击红色和选择**Do not process row with selected tag**,或者不设置直接导出,因为这工具暂时存在bug,无法过滤标记内容
    > 5.在AiNiee界面,选择`🔴Translator++项目`,配置翻译设置<br>
    > 配置示例<br>
    > <img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Tpp/翻译配置Tpp.png" width="400" height="300"><br>
    > 配置说明:<br>
    > `项目文件夹`: 选择之前`🔴Translator++`导出的项目文件夹data<br>
    > `输出文件夹`: 选择翻译后项目文件夹的存储文件夹<br>
* 5-2.🖱️点**开始翻译**按钮,等待翻译进度到百分百,生成翻译好的data文件夹在输出文件夹中,翻译中的备份会在在Backup Folder文件夹的data里<br>
    > 1.回到`🔴Translator++`+,点击导入工程,选择从电子表格导入翻译,点击“Import Folder”,选择输出文件夹里的data文件夹,点击导入<br>
    ><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Tpp/导入工程1.png" width="400" height="300">
    ><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Tpp/导入工程2.png" width="400" height="300"><br>
    >对**红色标签内容进行修改**,这些内容不能翻译,以免出现错误。还有对导入时缺行的内容进行自翻译

  🖱️右键左侧区域,移到"全部选择",选择"Create Automation",选择"对每行",复制粘贴下面的代码运行
  ```JavaScript
  if (this.tags) {
    if (this.tags.includes("red")) this.cells[1]=this.cells[0];
  }
  ```
    > <img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Tpp/处理错误1.png" width="400" height="300"><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Tpp/处理错误1.png" width="400" height="300">
  
  查看左边文件有哪个没有到达百分百的,寻找到空行并自行翻译
* 5-3.最后选择导出工程,选择导出到文件夹,指定**你的游戏目录里的data文件夹的上一级文件夹**,原文件会被替换,请注意备份原游戏
    ><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Tpp/修改游戏1.png" width="400" height="300"><img src="https://github.com/NEKOparapa/AiNiee-chatgpt/blob/main/Example%20image/Tpp/修改游戏2.png" width="400" height="300">

# 🕹️ 工具功能说明
***
* 😊如果您希望翻译从其他语言到中文,可以尝试修改Prompt词,把`日语`换成源语言,**英语除外**,因为已经被设置过滤了  
* `关于🔵Mtool项目的实时备份功能`
  >进行`🔵Mtool项目`翻译时,运行中会实时输出`TrsData.json`和`ManualTransFile.json`存储在`Backup Folder文件夹`里,`Backup Folder文件夹`里面的`ManualTransFile.json`是还没有翻译的数据,`TrsData.json`是现在已经翻译好的数据。如果因为意外中断了,把文件夹里的文件A(`TrsData.json`)放置其他地方保存,再选择备份文件夹里面的`ManualTransFile.json`开始翻译,生成新的文件B(`TrsData.json`),然后把文件B里的数据复制粘贴到文件A里面
* `关于🔴Translator++项目的实时备份功能`
  >运行中会实时输出data文件夹存储在`Backup Folder文件夹`里,在每个表格里,如果原文文本已经被翻译,译文会写在第二列,如果没有被翻译,则第二列继续为空,所以出现意外时,可直接选择`备份文件夹里data文件夹`来继续翻译 
* `词义检查`
  >是原文与译文的词义相似度检测功能,用来判断译文是否翻译错误,以解决AI翻译时错行的问题。开启这个功能会**耗费一段不短的时间进行检查**,而且会将错误内容进行重翻译,也会增加开销,**而非常非常吃性能**,性能越好,速度越快,CPU利用率会达到100%,**请慎重使用❗❗❗**
  (这个功能使用到了huggingface上的开源模型multilingual-MiniLM-L12-v2,第一次使用时会下载500mb的模型文件在C盘的.cache文件夹中,之后使用就不用了)

# 🍵 NEKO酱的个人BB
***
* 虽然有点编程基础,但还是第一次用🐍Python写程序,不是相关从业者,写法奇奇怪怪莫要怪。后续我不知道有没有时间去更新维护。既然已经开源了,就交给其他大佬了

* 🤖AI酱实在太厉害啦,一边写一边问她,什么都能回答,帮我写,帮我改bug,heart,heart,heart。

* 建了一个📮QQ交流群821624890,群里只用于反应bug,功能建议,以及prompt词交流,不要分享各种游戏资源,发黄键镇

# 🧉 A酱也小BB一下
***
* 大佬好厉害,我只能帮大佬写写md,虽然写的不是很漂亮，但尽力了😭
* 希望大家有机会也来我仓库玩玩(x
# 🧰 类似工具
***
 * 一个根据MTool导出其翻译结果用GPT翻译的项目
https://github.com/XHXJ/json-GPT-translator

 * 对已解包的GalGame脚本文件实行ChatGPT自动化翻译
https://github.com/Lilyltt/GalUpTs

# 🧾 声明
***
该款AI翻译工具仅供个人合法用途,任何使用该工具进行直接或者间接非法盈利活动的行为,均不属于授权范围,也不受到任何支持和认可
