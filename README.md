# 基于github action的京东自动化签到

# 教程
京东自动签到达成效果

- 每日自动签到领京豆
- 云签到，无需任何设备
- 支持双账号
- 微信定时推送结果

效果展示

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaIibiazicfjUpboYboBJjcj2vFJ5EOibUJliaEoCAET5x8H8lic94gI0DaNEQ/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaIibiazicfjUpboYboBJjcj2vFJ5EOibUJliaEoCAET5x8H8lic94gI0DaNEQ/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iamQUYMpg8dR9ibKFT9aUicVrtnjR2p2dI71mHXMRTIMLZgxSKCe39OMgw/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iamQUYMpg8dR9ibKFT9aUicVrtnjR2p2dI71mHXMRTIMLZgxSKCe39OMgw/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

========================================

**简单教程(简易教程,不懂的问题请百度)**

**帮忙点击文中广告支持一下，才有动力分享更多内容**

**第一步，帐号注册**

1、(拥有)注册一个github帐号

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iav9BgaglZjnN0VowCtbheLR9gexeib79rUfPRhvZ9Gk0V3OlsJNAQHqQ/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iav9BgaglZjnN0VowCtbheLR9gexeib79rUfPRhvZ9Gk0V3OlsJNAQHqQ/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

2、用github账户登录【Sever酱】http://sc.ftqq.com/3.version

微信推送---**绑定你的微信号**

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaGiazicKoFHLmFwRgZ97e60mjTbRBYicJDWBmO5XwHz0OWJkOANhBhKzQg/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaGiazicKoFHLmFwRgZ97e60mjTbRBYicJDWBmO5XwHz0OWJkOANhBhKzQg/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

3、点击上方的【发送消息】，**复制你的key值，保存到文本**，后面用到

（一人只有一个key，如果点重置key，则生成新key，旧key失效）

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaMtialDJlzGBLibCDviaxcGmfiabWdV3Yz2mKibjSFKibFaUib7SWoVibobnXiaw/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaMtialDJlzGBLibCDviaxcGmfiabWdV3Yz2mKibjSFKibFaUib7SWoVibobnXiaw/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

**第二步，获取京东cookie**

1、下载Jdcookie压缩包，下载后解压

**下载地址：https://wws.lanzous.com/后台回复JD获取下载地址**

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3ianOvg9a9Zg2OkwGeQPibuswrpcO8YovILpDibWRCiaqQjHZXzTIyeQubQA/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3ianOvg9a9Zg2OkwGeQPibuswrpcO8YovILpDibWRCiaqQjHZXzTIyeQubQA/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

2、到浏览器的扩展程序----加载解压的扩展—加载Jdcookie文件夹

下图用微软新版edge演示，chrome等浏览器同理

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaEHe8xzlGd2VwhuZ8mte31C0EVKMOd0eAiaFQSxzZI42vweeoAFJV36g/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaEHe8xzlGd2VwhuZ8mte31C0EVKMOd0eAiaFQSxzZI42vweeoAFJV36g/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

下图，显示加载成功

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaI8M4WMicFDAvyibAkwhj18Oz9Wks0Nn2uj1CQvycA4AfL6LpFaAxibfpw/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaI8M4WMicFDAvyibAkwhj18Oz9Wks0Nn2uj1CQvycA4AfL6LpFaAxibfpw/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

4、浏览器打开**https://m.jd.com**，点击【我的】---**手机短信登录**。

成功登录后---点击JDcookie插件（即小金豆）--提示cookies已经复制到剪切板。

我们把**cookie复制到文本**，备用。

（要获取第二个账号的cookie请用其他浏览器获取，不能以退出旧帐号登录新帐号，会导致旧账号cookie失效）

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaOibokHhWVHdBOeA2LQViby68icwea7wHu6FB5zHvfxezxIP4yWDLxqN3g/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaOibokHhWVHdBOeA2LQViby68icwea7wHu6FB5zHvfxezxIP4yWDLxqN3g/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaQy7NncK8OgmDJcCUryXkYyVK2ReyWlsZVxJgNibCPOZWRN7oCLXtBBA/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaQy7NncK8OgmDJcCUryXkYyVK2ReyWlsZVxJgNibCPOZWRN7oCLXtBBA/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

**第三步，部署github action**

1、登录github网站，打开**https://github.com/ZHDeveloper/JD_Sign_Action**

点击右上角的Fork，等待网页跳转至于 【你的ID/ JD_Sign_Action】

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaiaFkAFBFvJicicDkIicr2ZKEQVtIMGp2ISavp5yFVNsm4A3ICh485oo9aQ/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaiaFkAFBFvJicicDkIicr2ZKEQVtIMGp2ISavp5yFVNsm4A3ICh485oo9aQ/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

等待网页跳转为以下画面

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iays1jN89caFUkXDuxwp5sHwCcfJ9jTU0DokxF4dbrDBMuCHicKcicSFRg/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iays1jN89caFUkXDuxwp5sHwCcfJ9jTU0DokxF4dbrDBMuCHicKcicSFRg/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

2、点击settings—secrets—new secrets

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3ia3IfNFaeIkYmsiaCVtR3Za6VTsQibZ6yibm5UBQqQd1CrZdHGVPCdy0jew/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3ia3IfNFaeIkYmsiaCVtR3Za6VTsQibZ6yibm5UBQqQd1CrZdHGVPCdy0jew/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

新建 **JD_COOKIE** ，填入刚刚获取的cookie

新建 **PUSH_KEY** ，填入第一步获取的server酱的key

【若要双账号登录签到，则再新建 **JD_DUAL_COOKIE**，填入第二个账号cookie】

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaQfJia7Z98FJXl1hsETEvFZ7OjuAN4SdCdz5oabxZMbotk5ZTu7Bn5FQ/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaQfJia7Z98FJXl1hsETEvFZ7OjuAN4SdCdz5oabxZMbotk5ZTu7Bn5FQ/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaIDsZuDJpvaZic6OBzZv1t1JbOqf1wqWKjb8zN6dL61vMJMk0sdQKa4Q/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaIDsZuDJpvaZic6OBzZv1t1JbOqf1wqWKjb8zN6dL61vMJMk0sdQKa4Q/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

3、点击顶栏的Actions，点击**绿色**按钮，启用 Actions。

至此，完成了所有部署。

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3ia8bmP6QYp2G6gzbjEdjx1LLI186M4picOZUibbv569NrMzdlIZZUTGJcg/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3ia8bmP6QYp2G6gzbjEdjx1LLI186M4picOZUibbv569NrMzdlIZZUTGJcg/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaoBIAOTaO8RDvUOicuoBzEKIBVpgNxypcSrVrJFXWibH4EbHhRHXIMV7A/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaoBIAOTaO8RDvUOicuoBzEKIBVpgNxypcSrVrJFXWibH4EbHhRHXIMV7A/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

4、测试是否部署成功，可以手动**点亮**STAR（空心变成实心），程序会运行一次。

再点灭，再点亮，程序再运行一次。懂了吗？

[https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaAibptqTdhoFibjm0aGzPzJURGlhHgdOEYcquMiayiah1KFS6uF7EgPuZ8A/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1](https://mmbiz.qpic.cn/mmbiz_png/aD12XkDvgDgyVFLFVISRicbqiaJz3fNW3iaAibptqTdhoFibjm0aGzPzJURGlhHgdOEYcquMiayiah1KFS6uF7EgPuZ8A/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

5、如果收到短信推送（通常30S左右），说明成功了。

如不成功，请认真阅读教程。

后续程序每天4点帮你签到。

## 介绍

> 使用NobyDa “京东多合一签到脚本”为基础，移植到github actions自动化执行。



## 触发方式
* 点亮`Star`
* 凌晨4点定时执行
*  自定义：.github/workflows/work.yaml 编辑

## 使用用法
* 点击右上角 `Fork` 项目；
* `Settings` -> `Secrets` 中添加京东cookie、Server酱SCKEY
	- `JD_COOKIE`：京东cookie
	- `PUSH_KEY`：Server酱SCKEY
* 点击`Star`，任务会自动执行，运行进度和结果可以在`Actions`页面查看；
* 当任务运行完成时，会将运行结果和错误信息打包到`Artifacts`，可自行下载查看；

## 获取京东cookie

* 使用项目中的Chrome插件：`JDCookie`
* Chrome中拓展程序开启`开发者模式`；
* 点击`加载已解压的拓展程序`，选择`JDCookie`目录；
* 登录[领京豆](https://bean.m.jd.com/)；
* 点击`JDCookie`即可拷贝京东cookie

## 获取Server酱SCKEY

* github 授权登录[Server酱](http://sc.ftqq.com/3.version)官网
* 在`发送消息`拷贝SCKEY



## 效果截图

![WechatIMG3](./images/WechatIMG3.jpeg)

![WechatIMG4](./images/WechatIMG4.jpeg)


## 参考项目
* [NobyDa/Script/JD-DailyBonus](https://github.com/NobyDa/Script/blob/master/JD-DailyBonus/JD_DailyBonus.js)
* [ruicky/jd-sign-bot](https://github.com/ruicky/jd_sign_bot)
* [jerrykuku/luci-app-jd-dailybonus](https://github.com/jerrykuku/luci-app-jd-dailybonus)
