---
title: 'SA:MP脚本资源'
date: 2019-02-16 16:46:04
tags: 
  - GTA-SA
  - SAMP
  - SAMP-笔记
categories: GTA-SA
---
# IDs
## Sound IDs
> * 切换声音必须先使用声音ID 0来停止当前正在播放的声音ID。
> * 从0.3.7-R2起：
>	* 声音ID 1可用于禁用内部0（默认）环境声音（风噪声）。(提示:它可以帮助创建更逼真的假装内饰)
>	* 声音ID 0可以另外用于返回游戏的正常室外环境轨道。

<!--more-->

--------------------------------------------------

> 0.3.7-R2声音（由Vince和BigETI发现）

<!-- 改变最左侧一列宽度 -->
<style>
table th:first-of-type {
	width: 100px;
}
</style>

sound ID 	|	机器翻译		|	原文
------------|-------------------|----------------
2-59		|	警察电台		|	police radio
66-134		|	广播广告		|	radio adverts
135-136		|	通风			|	Ventilation
137			|	Ammu-Nation内部	|	Ammu-Nation interior
138			|	区域51内部		|	Area 51 interior
139			|	颁奖典礼音乐	|	awards ceremony music
140			|	迪斯科（摇滚）	|	Disco (Rock)
141			|	让我们为Bumble（Bee Bee Gone）音乐做好准备	|	Let's Get Ready to Bumble (Bee Bee Gone) music
142			|	与1185相同		|	same as 1185
143			|	Marco的小酒馆音乐	|	Marco's Bistro music
144			|	晚餐音乐		|	Diner music
145			|	与1097相同		|	same as 1097
146			|	赌场音乐		|	casino music
147			|	迪斯科（电子）	|	Disco (Electro)
148			|	飞机内部嗡嗡声	|	Plane interior humming
149			|	与1183相同		|	same as 1183
150			|	与1068相同		|	same as 1068
151			|	风扇			|	Fan
152			|	酒吧（外面？）	|	Bar (outside?)
153			|	与1062相同		|	same as 1062
154			|	通风			|	Ventilation
155-156		|	飞机内部嗡嗡声	|	plane interior humming
157			|	迪斯科（嘻哈）	|	Disco (Hip-Hop)
158			|	通风			|	Ventilation
159-160		|	赛马			|	Horse race
161			|	与1187相同		|	same as 1187
162			|	迪斯科（嘻哈）	|	Disco (Hip-Hop)
163			|	通风			|	Ventilation
164-165		|	航母升降机		|	aircraft carrier lift
166			|	暴动			|	Riot
167			|	雨				|	Rain
168			|	飞机内部		|	Plane interior
169			|	特技比赛		|	Stunt race
170			|	脱衣舞俱乐部	|	Strip club
171			|	迪斯科（岩石）：枪炮玫瑰 - 欢迎来到丛林	|	Disco (Rock): Guns N' Roses - Welcome To The Jungle
172			|	一些黑暗的主题	|	Some dark theme
173			|	输送带？		|	Conveyor belt?
174			|	水				|	Water
175			|	迪斯科			|	Disco
176			|	SA介绍音乐		|	SA intro music
177-179		|	迪斯科			|	Disco
179			|	Lowrider挑战	|	Lowrider challenge
180			|	Lowrider挑战	|	Lowrider challenge
181			|	Lowrider挑战	|	Lowrider challenge
182			|	任务通过主题/财产购买	|	mission passed theme / property bought
183			|	任务通过		|	Mission passed
184			|	语音线			|	Voice line
185-314		|	播放FM			|	Playback FM
315-469		|	K-ROSE			|	K-ROSE
470-625		|	K-DST（534罗德斯图尔特 - 今晚年轻人心旷神怡）	|	K-DST (534 Rod Stewart - Young hearts be free tonight)
626-668 	|	语音样本		|	Voice samples
669			|	女朋友约会失败的音乐（“他妈的你我不会做你告诉我的”）	|	girlfriend date failed music (fuck you I won't do what you tell me)
670			|	女友约会成功音乐|	girlfriend date success music
671-766 	|	语音线路（743  -  Big Smoke的订单）	|	Voice lines (743 - Big Smoke's order)
767-945 	|	弹跳FM			|	Bounce FM
946-999 	|	SF-UR			|	SF-UR
----
> 这些声音ID适用于每个版本！

| sound ID     	| 机翻                                   	| Name                               	|
|--------------	|----------------------------------------	|------------------------------------	|
| 1002         	| 声音 _ CEING _ VENENT _ LAND           	| SOUND_CEILING_VENT_LAND            	|
| 1009         	| 声音 _ 博内特 _ 登                     	| SOUND_BONNET_DENT                  	|
| 1027         	| 财富的圆轮 _                           	| SOUND_WHEEL_OF_FORTUNE_CLACKER     	|
| 1035         	| 声音 _ SHUTTER _ 门 _ START            	| SOUND_SHUTTER_DOOR_START           	|
| 1036         	| 声音 _ 切割机 _ 门 _ 停止              	| SOUND_SHUTTER_DOOR_STOP            	|
| 1039         	| 声音 _ PARACHUT _ OPEN                 	| SOUND_PARACHUTE_OPEN               	|
| 1052         	| 声音 _ 模拟 _ 购买 _ 武器              	| SOUND_AMMUNATION_BUY_WEAPON        	|
| 1053         	| 声音 _ 模拟 _ 购买 _ 武器 _ 装饰       	| SOUND_AMMUNATION_BUY_WEAPON_DENIED 	|
| 1054         	| 声音 _ 购物 _ 购买                     	| SOUND_SHOP_BUY                     	|
| 1055         	| 声音 _ 购物 _ 购买 _ 代理              	| SOUND_SHOP_BUY_DENIED              	|
| 1056         	| SOUND_RACE_321                         	| SOUND_RACE_321                     	|
| 1057         	| 声音 _ 比赛 _ 去                       	| SOUND_RACE_GO                      	|
| 1058         	| 声音 _ 部分 _ 任务 _ 完成              	| SOUND_PART_MISSION_COMPLETE        	|
| 1062 (music) 	| 声音 _ GOGO _ TRACK _ START            	| SOUND_GOGO_TRACK_START             	|
| 1063 (music) 	| 声音 _ GOGO _ TRACK _ STOP             	| SOUND_GOGO_TRACK_STOP              	|
| 1068 (music) 	| 声音 _ DUAL _ TRACK _ START            	| SOUND_DUAL_TRACK_START             	|
| 1069 (music) 	| 声音 _ DUAL _ TRACK _ STOP             	| SOUND_DUAL_TRACK_STOP              	|
| 1076 (music) 	| 声音 _ BEE _ TRACK _ START             	| SOUND_BEE_TRACK_START              	|
| 1077 (music) 	| 声音 _ BEE _ TRACK _ 停止              	| SOUND_BEE_TRACK_STOP               	|
| 1083         	| 声音 _ ROULETTE _ ADD _ CASH           	| SOUND_ROULETTE_ADD_CASH            	|
| 1084         	| 声音 _ ROULETTE _ 删除 _ CASH          	| SOUND_ROULETTE_REMOVE_CASH         	|
| 1085         	| 声音 _ ROULETTE _ NO _ CASH            	| SOUND_ROULETTE_NO_CASH             	|
| 1095         	| 声音 _ 自行车 _ 包装 _ 离合器          	| SOUND_BIKE_PACKER_CLUNK            	|
| 1097 (music) 	| 声音 _ 奖 _ 跟踪 _ 开始                	| SOUND_AWARD_TRACK_START            	|
| 1098 (music) 	| 声音 _ 奖 _ 跟踪 _ 停止                	| SOUND_AWARD_TRACK_STOP             	|
| 1100         	| 声音 _ MESH _ GATE _ OPEN _ START      	| SOUND_MESH_GATE_OPEN_START         	|
| 1101         	| 声音 _ 迈特 _ 开放 _ 停止              	| SOUND_MESH_GATE_OPEN_STOP          	|
| 1130         	| 声音 _ PUNCH _ PED                     	| SOUND_PUNCH_PED                    	|
| 1131         	| 声音 _ 放大 _ 枪 _ 碰撞                	| SOUND_AMMUNATION_GUN_COLLISION     	|
| 1132         	| 声音摄像机 _ 射击                      	| SOUND_CAMERA_SHOT                  	|
| 1133         	| 声音 _ 购买 _ 汽车 _ MOD               	| SOUND_BUY_CAR_MOD                  	|
| 1134         	| 声音 _ 购买 _ CAR _ 恢复               	| SOUND_BUY_CAR_RESPRAY              	|
| 1135         	| 声音 _ 棒球 _ 蝙蝠 _ 打 _ PED          	| SOUND_BASEBALL_BAT_HIT_PED         	|
| 1136         	| 声音 _ STUMP _ PED                     	| SOUND_STAMP_PED                    	|
| 1137         	| 声音 _ 检查点 _ 放大器                 	| SOUND_CHECKPOINT_AMBER             	|
| 1138         	| 声音 _ 检查点 _ 绿色                   	| SOUND_CHECKPOINT_GREEN             	|
| 1139         	| 声音 _ 检查点 _ 红色                   	| SOUND_CHECKPOINT_RED               	|
| 1140         	| 声音 _ 汽车 _ 斯马斯 _ 汽车            	| SOUND_CAR_SMASH_CAR                	|
| 1141         	| 声音 _ 汽车 _ 沙马克 _ 门              	| SOUND_CAR_SMASH_GATE               	|
| 1142         	| 声音 _ OTB _ TRACK _ START             	| SOUND_OTB_TRACK_START              	|
| 1143         	| 声音 _ OTB _ TRACK _ STOP              	| SOUND_OTB_TRACK_STOP               	|
| 1144         	| 声音 _ PED _ HIT _ WATER _ SPLASH      	| SOUND_PED_HIT_WATER_SPLASH         	|
| 1145         	| 声音 _ 餐厅 _ 培训 _ 碰撞              	| SOUND_RESTAURANT_TRAY_COLLISION    	|
| 1147         	| 声音 _ 甜品 _ HORN                     	| SOUND_SWEETS_HORN                  	|
| 1148         	| 声音 _ MAGNET _ 车辆 _ COLLION         	| SOUND_MAGNET_VEHICLE_COLLISION     	|
| 1149         	| 声音 _ 物业 _ 购买                     	| SOUND_PROPERTY_PURCHASED           	|
| 1150         	| 声音 _ 皮卡 _ 标准                     	| SOUND_PICKUP_STANDARD              	|
| 1153         	| 声音 _ GARAGE _ 门 _ START             	| SOUND_GARAGE_DOOR_START            	|
| 1154         	| 声音 _ 车库 _ 门 _ 停止                	| SOUND_GARAGE_DOOR_STOP             	|
| 1163         	| 声音 _ PED _ COLAPSE                   	| SOUND_PED_COLLAPSE                 	|
| 1165         	| 声音 _ 舒特 _ 门 _ 慢点 _ 开始         	| SOUND_SHUTTER_DOOR_SLOW_START      	|
| 1166         	| 声音 _ 舒特 _ 门 _ 慢速停止            	| SOUND_SHUTTER_DOOR_SLOW_STOP       	|
| 1169         	| 声源 _ 餐厅 _ CJ _ PUKE                	| SOUND_RESTAURANT_CJ_PUKE           	|
| 1183 (music) 	| 声音 _ 驾驶 _ 奖 _ 跟踪 _ 开始         	| SOUND_DRIVING_AWARD_TRACK_START    	|
| 1184         	| 声音 _ 驾驶 _ 奖 _ 跟踪 _ 停止         	| SOUND_DRIVING_AWARD_TRACK_STOP     	|
| 1185 (music) 	| 声音 _ 自行车 _ 奖 _ 跟踪 _ 开始       	| SOUND_BIKE_AWARD_TRACK_START       	|
| 1186         	| 声音 _ 自行车 _ 奖 _ 跟踪 _ 停止       	| SOUND_BIKE_AWARD_TRACK_STOP        	|
| 1187 (music) 	| 声音 _ PILOT _ 奖 _ TRACK _ START      	| SOUND_PILOT_AWARD_TRACK_START      	|
| 1188         	| 声音 _ PILOT _ 奖 _ TRAK _ STOP _ STOP 	| SOUND_PILOT_AWARD_TRACK_STOP       	|
| 1190         	| 声音 _ 地图                            	| SOUND_SLAP                         	|

-----
> 旧名单

|	sound ID	|	机翻						|	原文											|
|---------------|-------------------------------|---------------------------------------------------|
|	39047		|	“哪里是我的手机!!”			|	" where's my cellphone!! "						|
|	39051		|	“这是正确的把你的手放在那里”|	" that's right put your hands there "			|
|	39052		|	“圣洁他妈的我有我的手机”	|	" Holy fuck I've got my phone "					|
|	39074		|	“我在听......”				|	" I'm listening ... "							|
|	39076		|	“啊哈，真有趣”				|	" Aha , real interesting "						|
|	50002		|	“只是尝试朋克！试试吧！”	|	" Just Try Punk ! Just Try It ! "				|
|	50004		|	“你现在就是我的世界！”		|	" You're My World Now ! "						|
|	50050		|	“告诉我的妻子我爱她”		|	" Tell My Wife I Love Her "						|
|	50051		|	“我进去了”					|	" I'm going in "								|
|	50052		|	“地狱！”					|	" What The Hell ! "								|
|	50053		|	“呃，我的咖啡”				|	" Uh , My Coffee "								|
|	50094		|	“等等，想想你在做什么”		|	" Wait Wait , think about what you're doing "	|
|	100001		|	“来吧，时间就是金钱”		|	" Come On , time is money "						|
|	100005		|	“不是这车！”				|	" Not This Car ! "								|
|	100006		|	“我的老板会杀了我”			|	" My boss is gonna kill me "					|
|	100007		|	“还有另一个提示”			|	" There goes another tip "						|
|	100008		|	“OH NO MAN！”				|	" OH NO MAN ! "									|
|	100009		|	“今天不能变得更糟”			|	" Today couldn't get any worse "				|
|	100010		|	“这不好”					|	" This is not good "							|
|	100011		|	“你白痴”					|	" You Idiot "									|
|	100012		|	“向外看！”					|	" Look Out! "									|
|	100013		|	“你在做什么？！”			|	" What Are You Doing?! "						|
|	100014		|	“Heeeeey”					|	" Heeeeey "										|
|	100015		|	“哦他妈的”					|	" Oh Fuck "										|
|	100016		|	“他妈的是什么”				|	" What The Fuck "								|
|	100017		|	“嘿嘿！”					|	" Hey Man ! "									|


<!--more-->