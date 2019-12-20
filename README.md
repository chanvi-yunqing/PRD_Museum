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

- 利用百度AI中的通用物体和场景识别功能拍照识别博物馆展品，该功能支持识别动物、植物、商品、建筑、风景、动漫、食材、公众人物等10万个常见物体及场景，接口返回大类及细分类的名称结果，同时支持获取图片识别结果对应的百科信息，接口返回百科词条URL、图片和摘要描述，可选择是否需要返回百科信息。[百度AI通用物体和场景识别详情](https://ai.baidu.com/tech/speech/asr)

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


