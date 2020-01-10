# 动静皆宜博物馆

|  发布日期   |  2019.12   |
| --- | --- |
|  项目名称   |  懂你所动   |
|  文件主人   |  陈蕴晴   |
|  领头设计者 |  陈蕴晴   |
|  领头开发者 |  陈蕴晴   |
|  领头测试者 |  陈蕴晴   |

## 第一部分：PRD价值主张设计15%

### 背景概述

- 随着国家旅游业的高速发展，各地的博物馆成了出行旅游的圣地，博物馆在吸引到各地游客的同时我们也发现了相应的一些问题，比如游览博物馆的体验值，针对一些残障游客，博物馆的设备和设施并不足以支撑他们方便的游览，还有一类是多动症者的游览体验问题，针对这些游客单调的文字说明不足以吸引他们的注意，博物馆在面对动静两个极端层面的用户群体体验还是稍有欠缺，这个项目就是针对这一问题提出了动静皆宜博物馆方案。

### PRD1.产品介绍——价值宣言

- 对于一些身障者（聋哑人）无法听到博物馆现场的解说，我们的产品将针对这一现象利用百度平台种的语音识别API，将博物馆中的语音讲演转变成文字内容，这一功能能够帮助聋哑人士也能充分的体验到博物馆讲演部分。

- 对于一些多动症者，我们则打算使用百度API平台中提供的通用物体和场景识别的功能，帮助多动症者更好的体验博物馆的展览，多动症者多为儿童群体，针对这类群体他们并不能很好的理解博物馆中展品的解释说明，因为不懂所以觉得无趣不能集中精神游览，但是百度AI平台中提供的通用物体和场景识别功能可以将博物馆中的物体识别出更为浅显的解释，帮助多动症者解释展品内容。

### PRD2.产品核心价值

- 利用语音识别的功能，现场翻译讲演，帮助身障者更好的体验博物馆之旅。

- 利用通用物体和场景识别的功能，站在多动症者的角度去帮他们从最简单的物品概念去理解博物馆中的展品。

### PRD3.核心价值与用户痛点

- 身障者（聋哑人）：身障者因为身体某些功能上的残疾无法正常听到博物馆中某些展馆的讲演内容，针对这一用户痛点，我们的产品利用语音识别API，将博物馆中的语音讲演转变成文字内容，这一功能可以解决身障者（聋哑人）在博物馆讲演部分的困扰。

- 多动症者：多动症是一种常见的儿童为异常疾病，类患儿的智力正常或基本正常, 但学习、行为及情绪方面有缺陷，主要表现为注意力不集中，注意短暂，活动过多，情绪易冲动，面对这一用户痛点我们的产品利用了通用物体和场景识别功能向该类用户提供最浅显易懂的解释说明，从物品的基础属性介绍开始，从而提高他们的浏览积极性，同时手机扫描等更多的交互可以激发该类用户的积极性。

### PRD4.需求列表与人工智能API加值
| 用户 | 场景需求 | 重要程度 |
| --- | --- | --- |
| 身障者（聋哑人） | 想观看博物馆讲演却因身体部位残疾不能听到讲演内容 | 重要 |
| 多动症者 | 想了解展品内容却因为内容解释超过可承受的范围理解不了展品解释内容 | 重要 |

#### 人工智能API价值体现

- 利用百度AI中的语音识别功能将音频流转录为应用程序可以向用户显示或作为命令输入操作的文本，将60秒以内的语音精准识别为文字，可适用于手机语音输入、智能语音交互、语音指令、语音搜索等短语音交互场景，使用大规模数据集训练语言模型，根据语音的内容理解和停顿智能匹配合适的标点符号（包括，。！？），使识别结果的表现方式贴合表述，更加可懂。[百度AI语音识别详情](https://ai.baidu.com/tech/speech/asr)

- 利用百度AI中的通用物体和场景识别功能拍照识别博物馆展品，该功能支持识别动物、植物、商品、建筑、风景、动漫、食材、公众人物等10万个常见物体及场景，接口返回大类及细分类的名称结果，同时支持获取图片识别结果对应的百科信息，接口返回百科词条URL、图片和摘要描述，可选择是否需要返回百科信息。[百度AI通用物体和场景识别详情](https://ai.baidu.com/tech/imagerecognition/general)

### PRD5.人工智能概率性与用户痛点

#### 通用物体与场景识别

- 用户先输入一张图片
![输入图像](https://images.gitee.com/uploads/images/2019/1220/113415_4f011a97_1648233.png "图像1.png")

- 返回图像数据
![返回数据](https://images.gitee.com/uploads/images/2019/1220/113507_684b8ea6_1648233.png "图像2.png")

- 百度AI通用物体和场景识别可以根据用户拍摄照片，识别图片中物体名称及百科信息，提高用户交互体验，这一交互功能可以提高多动症群体的参馆积极性，同时扫描后返回的数据内容较为浅显，返回的内容都是一些基础的物体属性，能够更好的帮助多动症者理解博物馆中的展品，同时提高用户的参馆体验。

#### 百度AI语音识别详细介绍

- 技术领先识别准确：采用领先国际的流式端到端语音语言一体化建模方法，融合百度自然语言处理技术，近场中文普通话识别准确率达98%

- 多语种和多方言识别：支持普通话和略带口音的中文识别；支持粤语、四川话方言识别；支持英文识别

- 深度语义解析：支持50多个领域的语义理解，如：天气，交通，娱乐等。还可接入智能对话定制与服务平台UNIT自定义语义理解和对话服务，让您更准确地理解用户意图

- 中文标点智能断句：使用大规模数据集训练语言模型，根据语音的内容理解和停顿智能匹配合适的标点符号（包括，。！？），使识别结果的表现方式贴合表述，更加可懂

- 数字格式智能转换：根据语音内容理解可以将数字序列、小数、时间、分数、基础运算符正确转换为数字格式，使得识别的数字结果更符合使用习惯，直观自然

- 支持自助训练专属模型：支持在语音自训练平台上自助训练模型，上传词汇文本即可零代码完成训练，精准提升业务领域词汇识别率5-25%，并可专属使用

### 原型设计

#### 原型1：交互界面设计（语音识别）

![语音识别](https://images.gitee.com/uploads/images/2020/0110/114737_19870662_1648233.png "识别1.png")

- 以上界面是语音识别界面，当用户点击开始识别按钮是，界面显示识别中的状态，当用户选择结束识别时，界面弹出相关的语音识别结果，操作过程如上图所示。


- 交互界面（通用物体和场景识别功能）

![物体识别1](https://images.gitee.com/uploads/images/2020/0110/114939_41e5899a_1648233.png "识别2.png")

- 以上界面时物体识的功能，就是通用物体和场景识别功能，用户选择识物功能后app会打开摄像功能对物体进行识别，经过2~3秒的时间后识别出对应的结果，用户可以点击识别出相对应的图片。

![物体识别2](https://images.gitee.com/uploads/images/2020/0110/115009_acbfe432_1648233.png "识别3.png")

- 让用户选择了识别出来相对应的图片后，页面跳转至对应的资料解释页面，如上图所示。

#### 原型3：原型文档

- [动静皆宜博物馆原型链接](http://nfunm010.gitee.io/museum)

- [动静皆宜博物馆原型下载](https://gitee.com/NFUNM010/museum)

### API 产品使用关键AI或机器学习之API的输出入展示 

#### API使用水平（语音识别）

- 技术领先识别准确：采用领先国际的流式端到端语音语言一体化建模方法，融合百度自然语言处理技术，近场中文普通话识别准确率达98%

- 多语种和多方言识别：支持普通话和略带口音的中文识别；支持粤语、四川话方言识别；支持英文识别

- 深度语义解析：支持50多个领域的语义理解，如：天气，交通，娱乐等。还可接入智能对话定制与服务平台UNIT自定义语义理解和对话服务，让您更准确地理解用户意图

- 中文标点智能断句：使用大规模数据集训练语言模型，根据语音的内容理解和停顿智能匹配合适的标点符号（包括，。！？），使识别结果的表现方式贴合表述，更加可懂

- 数字格式智能转换：根据语音内容理解可以将数字序列、小数、时间、分数、基础运算符正确转换为数字格式，使得识别的数字结果更符合使用习惯，直观自然

- 支持自助训练专属模型：支持在语音自训练平台上自助训练模型，上传词汇文本即可零代码完成训练，精准提升业务领域词汇识别率5-25%，并可专属使用

##### 代码调用尝试

- 输入
```
from aip import AipSpeech

""" 你的 APPID AK SK """
APP_ID = '你的 App ID'
API_KEY = '你的 Api Key'
SECRET_KEY = '你的 Secret Key'

client = AipSpeech(APP_ID, API_KEY, SECRET_KEY)
```

#### API使用水平（通用物体和场景识别）
 
- 识别物体或场景名称：支持识别动物、植物、商品、建筑、风景、动漫、食材、公众人物等10万个常见物体及场景，接口返回大类及细分类的名称结果

- 获取百科信息：支持获取图片识别结果对应的百科信息，接口返回百科词条URL、图片和摘要描述，可选择是否需要返回百科信息

#### 代码调用尝试

- 输入

```
# encoding:utf-8

import requests
import base64

'''
通用物体和场景识别
'''

request_url = "https://aip.baidubce.com/rest/2.0/image-classify/v2/advanced_general"
# 二进制方式打开图片文件
f = open('[本地文件]', 'rb')
img = base64.b64encode(f.read())

params = {"image":img}
access_token = '[调用鉴权接口获取的token]'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/x-www-form-urlencoded'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())

```

- 输出
```
HTTP/1.1 200 OK
x-bce-request-id: 73c4e74c-3101-4a00-bf44-fe246959c05e
Cache-Control: no-cache
Server: BWS
Date: Tue, 18 Oct 2016 02:21:01 GMT
Content-Type: application/json;charset=UTF-8
{
	"log_id": 327863200205075661,
	"result_num": 5,
	"result": [{
		"score": 0.967622,
		"root": "公众人物",
		"baike_info": {
			"baike_url": "http://baike.baidu.com/item/%E6%96%B0%E5%9E%A3%E7%BB%93%E8%A1%A3/8035884",
			"image_url": "http://imgsrc.baidu.com/baike/pic/item/91ef76c6a7efce1b27893518a451f3deb58f6546.jpg",
			"description": "新垣结衣(Aragaki Yui)，1988年6月11日出生于冲绳县那霸市。日本女演员、歌手、模特。毕业于日出高中。2001年，参加《nicola》模特比赛并获得最优秀奖。2005年，因出演现代剧《涩谷15》而作为演员出道。2006年，参演校园剧《我的老大，我的英雄》；同年，她还出版了个人首本写真集《水漾青春》。2007年，她从日出高校毕业后开始专注于演艺发展，并发表个人首张音乐专辑《天空》；同年，新垣结衣还主演了爱情片《恋空》，而她也凭借该片获得了多个电影新人奖项。2010年，主演爱情片《花水木》。2011年，主演都市剧《全开女孩》。2012年，相继参演现代剧《Legal High》、剧情片《剧场版新参者：麒麟之翼》。2013年，主演都市剧《飞翔情报室》。2014年，她主演了剧情片《黎明的沙耶》。2016年，主演爱情喜剧《逃避虽可耻但有用》，并凭借该剧获得了多个电视剧女主角奖项。2017年，主演爱情片《恋爱回旋》，凭借该片获得第60届蓝丝带奖最佳女主角；同年11月，她还凭借医疗剧《Code Blue 3》获得第94届日剧学院赏最佳女配角。"
		},
		"keyword": "新垣结衣"
	},
	{
		"score": 0.716067,
		"root": "人物-人物特写",
		"keyword": "头发"
	},
	{
		"score": 0.421281,
		"root": "商品-穿戴",
		"keyword": "围巾"
	},
	{
		"score": 0.22347,
		"root": "商品-五金",
		"keyword": "拉链"
	},
	{
		"score": 0.028031,
		"root": "商品-穿戴",
		"keyword": "脖套"
	}]
}

```

### API使用比较分析

百度AI（语音识别）：电话语音实时识别采用针对呼叫中心场景专门训练的语音识别模型，将电话语音实时精准识别为文字，支持MRCP等多种接入方式，适配常见呼叫中心软硬交换，提供MRCP Server，Linux C++ SDK，Java SDK，API等多种接入方式；支持时间戳、语速检测支持返回客服、客户双侧对话语音识别结果及每句话的时间戳、语速等信息。应用场景有如下几部分，客服话术辅助，在客服与客户对话过程中，实时将对话语音转为文字，基于对话内容为客服提供话术提示。提升客服人员操作效率，降低通话时长。提升客服服务标准化程度及销售转化；语音应答机器人，实时识别客户语音，精准转成文字，判断客户意图，为客户提供对应服务。降低进线量，降低客服人力成本。也可以基于识别内容，进行问题分发或提示，提升服务效率；智能语音机器人回访，通过实时语音识别，将客户语音识别为文字，完成回访对话流程。提升回访效率，将重复性的电话回访交由机器完成，降低客服人力成本。实时语音质检，实时将客服及客户的对话过程转文字，并对其中的对话内容进行实时全量质检。及时发现服务瑕疵，实时进行干预，提升客服服务质量。

百度AI（通用物体和场景识别）：准确性高，基于百度海量数据，利用深度学习技术及高精度算法不断迭代模型，准确率业界领先
标签体系丰富；可识别出10万+物体及场景标签，并在不断丰富中，持续提供更精细的识别服务，简单易用，支持标准化接口封装，调用简单，只需上传单张图片，即可获取识别结果；应用场景有图片内容分析与推荐，对用户浏览的图片或观看的视频内容进行识别，根据识别结果给出相关内容推荐或广告展示。广泛应用于新闻资讯类、视频类app等内容平台中；拍照识图，根据用户拍摄照片，识别图片中物体名称及百科信息，提高用户交互体验，广泛应用于智能手机厂商、拍照识图及科普类app中；拍照闯关趣味营销，设计线上营销活动，根据用户拍摄照片，自动识别图片中物体信息是否符合活动要求，提升用户交互体验，减少人工审核成本。




