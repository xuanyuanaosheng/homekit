## 智能家居

目前国内生态最好且开放的智能家居系统就是`小米`了吧，像华为、天猫、京东这些互联网厂商相对差一点，传统的家电设备制造商例如：美的，格力，海尔，一言难尽，传统厂商生态很差。
国外的目前能用的就是苹果的homekit系列了。

## 主要通过HassOS实现不同厂商不同设备的接入

## HassOS的美化
HassOS美化主要适合家里有屏幕，主要用来进行展示，这个可以通过二手平板来展示，主要是为了美观，这个教程也是最多的，可以自行去b站学习。
1.  https://space.bilibili.com/1004644981 

## HassOS的自动化：Node-RED
相对于上面的展示，智能自动化才是智能家居的核心，但是现在大家似乎更关心美化，反而是自动化忽略好多。

## HassOS的第三方插件库：HACS
1.  给HACS增加代理功能： https://bbs.hassbian.com/thread-16136-1-1.html (https://github.com/ryanh7/hacs-proxy)
 

## 第三方设备接入HassOS

### 小米的设备

小米的设备接入最简单也最快捷。HACS里安装安装需要插件：
- Xiaomi MIoT
- Xiaomi Miot Auto (一般这个就足够了)
- Xiaomi Gateway 3 

参考资料：
1. https://space.bilibili.com/1004644981 

### 苹果的设备

在集成里添加 HomeKit，完成后在HA通知下可看到接入HomeKit的二维码，使用iPad或iPhone的家庭App扫描即可，接入后设备将自动同步到家庭App中。

### 海尔的设备
#### HACS里安装需要的插件：
- Node-Red

#### 参考资料
1.  https://bbs.hassbian.com/thread-16180-1-1.html
2.  https://www.haoyizebo.com/posts/f941c767/

### 美的的设备
#### HACS里安装需要的插件：
- Midea AC LAN

#### 参考资料
1. https://bbs.hassbian.com/thread-16812-1-1.html
2. https://www.bilibili.com/video/BV1dT411F7oQ/

### 格力的设备

1.  格力空调通过  Homeassistant 的Gree Climate 组件集成搞定接入 HomeKit

## 第三方生活数据接入

这些国企的开发水平真的没得说，都是外包。

1.  水：根据不同的地区，
- 

2.  电：需要根据不同的地区进行查询，这个和国网电力提供的有关

-  北京电费查询：https://bbs.hassbian.com/thread-13820-1-1.html (https://github.com/georgezhao2010/bj_sgcc_energy)
-  江苏电费查询： https://bbs.hassbian.com/thread-12037-1-1.html
-  南方电网：https://github.com/CubicPill/china_southern_power_grid_stat 

3.  燃气：
- (https://github.com/zhaoyibo/bj_gas)

4. 天气：
- 和风天气：https://bbs.hassbian.com/thread-17286-1-1.html
- 彩云天气：https://bbs.hassbian.com/thread-7399-1-1.html

## 家里其他设备接入

1. 网络设备：

2. 监控设备：

---
## 选用小米的小爱同学作为家里的控制中心
1.  https://www.v2ex.com/t/795240#reply22 （用MQTT来做，使小爱可以语音控制其他设备，就可以通过巴法云的 MQTT使小爱可以控制非小米设备，不需要homeassistant，但是需要自己开发第三方设备的API ）
[小爱同学控制松下浴霸](https://i.imgur.com/m4IksnK.jpeg)
2.  https://bbs.hassbian.com/thread-16180-11-1.html (为了使小爱可以语音控制海尔设备，才用MQTT来做，就可以通过巴法云使小爱可以控制海尔设备)
3.  使用小爱同学控制添加到Homeassistant的非小米设备： https://github.com/al-one/hass-xiaomi-miot/issues/537 (小爱对话记录实体使用场景，需要homeassistant)
4.  给小爱同学赋能，增加Chatgpt人工智能助手：https://github.com/yihong0618/xiaogpt （思路：通过定时轮训小爱同学的对话功能来实现,不需要homeassistant）

### 参考文档
1. homelab 家庭弱电方案分享 : https://taresky.com/network-setup-2022
2. NAS / HomeLab 玩家看过来，这是一份非常赞的 Self-Hosted 清单，包含市面上大多数热门自部署软件。 https://selfh.st/apps/


---
## 家庭智能影音

### 黑群晖
#### 套件中心
- synocommunity：https://packages.synocommunity.com/
- 云梦：https://spk.520810.xyz:666
- 裙下孤魂：http://spk.bobohome.store:8880
- 我不是狂神：https://spk7.imnks.com/

