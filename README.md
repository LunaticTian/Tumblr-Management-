# Tall开发笔记



<br>
## 功能列表

* 信息聚合查询
	* 汤不热检索
	* 3DM游戏检索
	* 电影信息/下载检索
	* 妹子图/random
	* 音乐搜索/试听
	* 图书搜索查询
	* 未完待续....
* 会员管理
	* 用户注册
	* 修改密码
	* 找回密码
	* 人物头衔
	* 积分充值
	* 积分兑换 
* 后台管理
	* 用户管理
	* 充值管理
	* 信息聚合
		* 添加
		* 查询
		* 修改
		* 删除
* 留言 

## 开发思路

设计初全平台兼容，所以以Restful API规范。

信息聚合数据为两大部分:
1.第一部分以汤不热和3DM为代表的前行爬取为基础进行内容的检索和呈现。
2.第二部分以音乐搜索图书查询为代表的第三方提供的api接口。


## 适配平台
1.web
2.Android
3.IOS

## 开发语言

服务端：java

开发框架：

* maven
* jersey
* mybatis
* spring
* springMVC

## 相关API重点

API鉴权对于rustful是比较重要的点，所以这里采用CSDN的[Restful Api的访问控制方法](https://blog.csdn.net/linlzk/article/details/50748580)。<br>
Token时间有效值(动态生成)

再着就是怎样让本项目方便进行二次开发，项目最终是基于SSM的，但是前期因为笔者不熟悉，只能先采用maven以及jersey进行开发。
在实现功能模块后进行框架的对接，这也是目前比较折中的方案。








