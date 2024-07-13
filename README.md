<div align="center">
<h1 align="center">原始项目: AdBlock-Acceleration<br><img align='middle' src='https://anay.cosr.eu.org/?text=@Bush2021/filters'></img></h1>
<img align='middle' src='https://anay.cosr.eu.org/?repo=Silentely/AdBlock-Acceleration'></img>
<br>
<img src="https://img.shields.io/github/forks/Silentely/AdBlock-Acceleration?color=orange">
<img src="https://img.shields.io/github/issues/Silentely/AdBlock-Acceleration?color=green">
<br>
<img src="https://img.shields.io/github/license/Silentely/AdBlock-Acceleration?color=ff69b4">
<img src="https://img.shields.io/github/languages/code-size/Bush2021/filters?color=blueviolet">
<img src="https://img.shields.io/badge/dynamic/json?label=GitHub%20Followers&query=%24.data.totalSubs&url=https%3A%2F%2Fapi.spencerwoo.com%2Fsubstats%2F%3Fsource%3Dgithub%26queryKey%3DSilentely&labelColor=282c34&color=181717&logo=github&longCache=true "关注数量">
<br>
<img src="https://app.fossa.com/api/projects/git%2Bgithub.com%2FSilentely%2FAdBlock-Acceleration.svg?type=small">
</div>

# 项目简介

国际/中国加速过滤广告规则订阅

# 公告 

* **2024年03月21日，清理仓库，更新部分链接。** 

## 🔖 过滤工具推荐

过滤工具：
* 🌍 浏览器扩展
  * [uBlock Origin](https://github.com/gorhill/uBlock)
  * [uBlock Origin Lite (for MV3)](https://github.com/uBlockOrigin/uBOL-home)
  * [AdGuard](https://adguard.com)
* 📺 路由器端
  * [AdGuard Home](https://adguard.com/zh_cn/adguard-home/overview.html)
* 📱 移动端
  * [AdGuard for Android](https://adguard.com/zh_cn/adguard-android/overview.html)
  * [AdGuard for iOS](https://adguard.com/zh_cn/adguard-ios/overview.html)
* 💻 桌面端（全局去广告）
  * [AdGuard for Windows](https://adguard.com/zh_cn/adguard-windows/overview.html)
  * [AdGuard for macOS](https://adguard.com/zh_cn/adguard-mac/overview.html)

🙅‍♂️但是这类工具都存在一个痛点，因为规则基本都托管在境外服务器，导致更新极其缓慢，甚至无法成功更新。

💥 这个项目就是为了解决这一难题，无需通过任何代理即可光速更新规则。

## 🕹 项目原理
项目使用了 GitHub Actions 在每天 UTC 时间每隔 3 小时更新下载一次最新规则，然后推送到 GitHub Repo。  
配合使用四个网站提供的全球加速 CDN 来分发规则。
①[jsDelivr](https://www.jsdelivr.com) （有缓存）   
②[ghproxy](https://ghproxy.net) （无缓存）    
③[Fastgit](https://raw.fastgit.org) （无缓存）   
④[b-cdn.net](https://jsdelivr.b-cdn.net) （有缓存）   

从而实现秒秒钟更新所有去广告规则。
                                                                                                                `

## 🍔 使用方法
**⚠️ 注意：** 该规则不是针对网络代理工具的，不要给 Surge、ShadowRocket、Quantumult(X)、Clash(X/A) 等类似工具使用！
直接拷贝下方表格中，对应规则的加速地址，作为去广告工具的订阅规则链接即可。

## 📃 规则列表

| 🥑 规则名称 | 原始地址 | 🚀 国际推荐① | 🚀 国际推荐② | 🚀 国内推荐③ | 🚀 国内推荐④ | 🚀 国内推荐⑤ |
| :----: | :----: | :----: | :----: | :----: | :----: | :----: |
| AdGuard DNS Filter | [原始](https://adguardteam.github.io/AdGuardSDNSFilter/Filters/filter.txt) | [国际推荐①](https://cdn.jsdelivr.net/gh/Bush2021/filters@main/AdGuard_Simplified_Domain_Names_Filter.txt) | [国际推荐②](https://gcore.jsdelivr.net/gh/Bush2021/filters@main/AdGuard_Simplified_Domain_Names_Filter.txt) | [国内推荐③](https://ghproxy.net/https://raw.githubusercontent.com/Bush2021/filters/main/AdGuard_Simplified_Domain_Names_Filter.txt) | [国内推荐④](https://raw.fastgit.org/Bush2021/filters/main/AdGuard_Simplified_Domain_Names_Filter.txt) | [国内推荐⑤](https://jsdelivr.b-cdn.net/gh/Bush2021/filters@main/AdGuard_Simplified_Domain_Names_Filter.txt) |
| AdGuard Base Filter 👍 | [原始](https://filters.adtidy.org/extension/ublock/filters/2_optimized.txt) | [国际推荐①](https://cdn.jsdelivr.net/gh/Bush2021/filters@main/AdGuard_Base_filter.txt) | [国际推荐②](https://gcore.jsdelivr.net/gh/Bush2021/filters@main/AdGuard_Base_filter.txt) | [国内推荐③](https://ghproxy.net/https://raw.githubusercontent.com/Bush2021/filters/main/AdGuard_Base_filter.txt) | [国内推荐④](https://raw.fastgit.org/Bush2021/filters/main/AdGuard_Base_filter.txt) | [国内推荐⑤](https://jsdelivr.b-cdn.net/gh/Bush2021/filters@main/AdGuard_Base_filter.txt) |
| AdGuard Chinese Filter 👍 | [原始](https://filters.adtidy.org/extension/ublock/filters/224_optimized.txt) | [国际推荐①](https://cdn.jsdelivr.net/gh/Bush2021/filters@main/AdGuard_Chinese_filter.txt) | [国际推荐②](https://gcore.jsdelivr.net/gh/Bush2021/filters@main/AdGuard_Chinese_filter.txt) | [国内推荐③](https://ghproxy.net/https://raw.githubusercontent.com/Bush2021/filters/main/AdGuard_Chinese_filter.txt) | [国内推荐④](https://raw.fastgit.org/Bush2021/filters/main/AdGuard_Chinese_filter.txt) | [国内推荐⑤](https://jsdelivr.b-cdn.net/gh/Bush2021/filters@main/AdGuard_Chinese_filter.txt) |
| AdGuard Tracking Protection Filter | [原始](https://filters.adtidy.org/extension/ublock/filters/3_optimized.txt) | [国际推荐①](https://cdn.jsdelivr.net/gh/Bush2021/filters@main/AdGuard_Tracking_Protection_filter.txt) | [国际推荐②](https://gcore.jsdelivr.net/gh/Bush2021/filters@main/AdGuard_Tracking_Protection_filter.txt) | [国内推荐③](https://ghproxy.net/https://raw.githubusercontent.com/Bush2021/filters/main/AdGuard_Tracking_Protection_filter.txt) | [国内推荐④](https://raw.fastgit.org/Bush2021/filters/main/AdGuard_Tracking_Protection_filter.txt) | [国内推荐⑤](https://jsdelivr.b-cdn.net/gh/Bush2021/filters@main/AdGuard_Tracking_Protection_filter.txt) |
| AdGuard Tracking Parameters | [原始](https://filters.adtidy.org/extension/ublock/filters/17_optimized.txt) | [国际推荐①](https://cdn.jsdelivr.net/gh/Bush2021/filters@main/AdGuard_Tracking_Parameters.txt) | [国际推荐②](https://gcore.jsdelivr.net/gh/Bush2021/filters@main/AdGuard_Tracking_Parameters.txt) | [国内推荐③](https://ghproxy.net/https://raw.githubusercontent.com/Bush2021/filters/main/AdGuard_Tracking_Parameters.txt) | [国内推荐④](https://raw.fastgit.org/Bush2021/filters/main/AdGuard_Tracking_Parameters.txt) | [国内推荐⑤](https://jsdelivr.b-cdn.net/gh/Bush2021/filters@main/AdGuard_Tracking_Parameters.txt) |
| AdGuard Annoyances Filter | [原始](https://filters.adtidy.org/extension/ublock/filters/14_optimized.txt) | [国际推荐①](https://cdn.jsdelivr.net/gh/Bush2021/filters@main/AdGuard_Annoyances_filter.txt) | [国际推荐②](https://gcore.jsdelivr.net/gh/Bush2021/filters@main/AdGuard_Annoyances_filter.txt) | [国内推荐③](https://ghproxy.net/https://raw.githubusercontent.com/Bush2021/filters/main/AdGuard_Annoyances_filter.txt) | [国内推荐④](https://raw.fastgit.org/Bush2021/filters/main/AdGuard_Annoyances_filter.txt) | [国内推荐⑤](https://jsdelivr.b-cdn.net/gh/Bush2021/filters@main/AdGuard_Annoyances_filter.txt) |
| AdGuard Annoyances Cookies 👍 | [原始](https://filters.adtidy.org/extension/ublock/filters/18_optimized.txt) | [国际推荐①](https://cdn.jsdelivr.net/gh/Bush2021/filters@main/AdGuard_Annoyances_Cookies.txt) | [国际推荐②](https://gcore.jsdelivr.net/gh/Bush2021/filters@main/AdGuard_Annoyances_Cookies.txt) | [国内推荐③](https://ghproxy.net/https://raw.githubusercontent.com/Bush2021/filters/main/AdGuard_Annoyances_Cookies.txt) | [国内推荐④](https://raw.fastgit.org/Bush2021/filters/main/AdGuard_Annoyances_Cookies.txt) | [国内推荐⑤](https://jsdelivr.b-cdn.net/gh/Bush2021/filters@main/AdGuard_Annoyances_Cookies.txt) |
| AdGuard Popups | [原始](https://filters.adtidy.org/extension/ublock/filters/19_optimized.txt) | [国际推荐①](https://cdn.jsdelivr.net/gh/Bush2021/filters@main/AdGuard_Popups.txt) | [国际推荐②](https://gcore.jsdelivr.net/gh/Bush2021/filters@main/AdGuard_Popups.txt) | [国内推荐③](https://ghproxy.net/https://raw.githubusercontent.com/Bush2021/filters/main/AdGuard_Popups.txt) | [国内推荐④](https://raw.fastgit.org/Bush2021/filters/main/AdGuard_Popups.txt) | [国内推荐⑤](https://jsdelivr.b-cdn.net/gh/Bush2021/filters@main/AdGuard_Popups.txt) |
| EasyList China | [原始](https://easylist-downloads.adblockplus.org/easylistchina.txt) | [国际推荐①](https://cdn.jsdelivr.net/gh/Bush2021/filters@main/EasyList_China.txt) | [国际推荐②](https://gcore.jsdelivr.net/gh/Bush2021/filters@main/EasyList_China.txt) | [国内推荐③](https://ghproxy.net/https://raw.githubusercontent.com/Bush2021/filters/main/EasyList_China.txt) | [国内推荐④](https://raw.fastgit.org/Bush2021/filters/main/EasyList_China.txt) | [国内推荐⑤](https://jsdelivr.b-cdn.net/gh/Bush2021/filters@main/EasyList_China.txt) |
| EasyPrivacy 👍 | [原始](https://easylist-downloads.adblockplus.org/easyprivacy.txt) | [国际推荐①](https://cdn.jsdelivr.net/gh/Bush2021/filters@main/EasyPrivacy.txt) | [国际推荐②](https://gcore.jsdelivr.net/gh/Bush2021/filters@main/EasyPrivacy.txt) | [国内推荐③](https://ghproxy.net/https://raw.githubusercontent.com/Bush2021/filters/main/EasyPrivacy.txt) | [国内推荐④](https://raw.fastgit.org/Bush2021/filters/main/EasyPrivacy.txt) | [国内推荐⑤](https://jsdelivr.b-cdn.net/gh/Bush2021/filters@main/EasyPrivacy.txt) |
| 屏蔽网站的 Cookies 警告 | [原始](https://www.i-dont-care-about-cookies.eu/abp) | [国际推荐①](https://cdn.jsdelivr.net/gh/Bush2021/filters@main/I_dont_care_about_cookies.txt) | [国际推荐②](https://gcore.jsdelivr.net/gh/Bush2021/filters@main/I_dont_care_about_cookies.txt) | [国内推荐③](https://ghproxy.net/https://raw.githubusercontent.com/Bush2021/filters/main/I_dont_care_about_cookies.txt) | [国内推荐④](https://raw.fastgit.org/Bush2021/filters/main/I_dont_care_about_cookies.txt) | [国内推荐⑤](https://jsdelivr.b-cdn.net/gh/Bush2021/filters@main/I_dont_care_about_cookies.txt) |
| CJX's EasyList Lite | [原始](https://raw.githubusercontent.com/cjx82630/cjxlist/master/cjxlist.txt) | [国际推荐①](https://cdn.jsdelivr.net/gh/Bush2021/filters@main/CJX's_EasyList_Lite.txt) | [国际推荐②](https://gcore.jsdelivr.net/gh/Bush2021/filters@main/CJX's_EasyList_Lite.txt) | [国内推荐③](https://ghproxy.net/https://raw.githubusercontent.com/Bush2021/filters/main/CJX's_EasyList_Lite.txt) | [国内推荐④](https://raw.fastgit.org/Bush2021/filters/main/CJX's_EasyList_Lite.txt) | [国内推荐⑤](https://jsdelivr.b-cdn.net/gh/Bush2021/filters@main/CJX's_EasyList_Lite.txt) |
| CJX's Annoyance List 👍 | [原始](https://raw.githubusercontent.com/cjx82630/cjxlist/master/cjx-annoyance.txt) | [国际推荐①](https://cdn.jsdelivr.net/gh/Bush2021/filters@main/CJX's_Annoyance_List.txt) | [国际推荐②](https://gcore.jsdelivr.net/gh/Bush2021/filters@main/CJX's_Annoyance_List.txt) | [国内推荐③](https://ghproxy.net/https://raw.githubusercontent.com/Bush2021/filters/main/CJX's_Annoyance_List.txt) | [国内推荐④](https://raw.fastgit.org/Bush2021/filters/main/CJX's_Annoyance_List.txt) | [国内推荐⑤](https://jsdelivr.b-cdn.net/gh/Bush2021/filters@main/CJX's_Annoyance_List.txt) |
| 乘风通用广告过滤规则 | [原始](https://raw.githubusercontent.com/xinggsf/Adblock-Plus-Rule/master/rule.txt) | [国际推荐①](https://cdn.jsdelivr.net/gh/Bush2021/filters@main/Xinggsf_rule.txt) | [国际推荐②](https://gcore.jsdelivr.net/gh/Bush2021/filters@main/Xinggsf_rule.txt) | [国内推荐③](https://ghproxy.net/https://raw.githubusercontent.com/Bush2021/filters/main/Xinggsf_rule.txt) | [国内推荐④](https://raw.fastgit.org/Bush2021/filters/main/Xinggsf_rule.txt) | [国内推荐⑤](https://jsdelivr.b-cdn.net/gh/Bush2021/filters@main/Xinggsf_rule.txt) |
| 乘风视频广告过滤规则 👍 | [原始](https://raw.githubusercontent.com/xinggsf/Adblock-Plus-Rule/master/mv.txt) | [国际推荐①](https://cdn.jsdelivr.net/gh/Bush2021/filters@main/Xinggsf_mv.txt) | [国际推荐②](https://gcore.jsdelivr.net/gh/Bush2021/filters@main/Xinggsf_mv.txt) | [国内推荐③](https://ghproxy.net/https://raw.githubusercontent.com/Bush2021/filters/main/Xinggsf_mv.txt) | [国内推荐④](https://raw.fastgit.org/Bush2021/filters/main/Xinggsf_mv.txt) | [国内推荐⑤](https://jsdelivr.b-cdn.net/gh/Bush2021/filters@main/Xinggsf_mv.txt) |
| 乘风小众视频视频规则 | [原始](https://raw.githubusercontent.com/xinggsf/Adblock-Plus-Rule/master/minority-mv.txt) | [国际推荐①](https://cdn.jsdelivr.net/gh/Bush2021/filters@main/Xinggsf_minority-mv.txt) | [国际推荐②](https://gcore.jsdelivr.net/gh/Bush2021/filters@main/Xinggsf_minority-mv.txt) | [国内推荐③](https://ghproxy.net/https://raw.githubusercontent.com/Bush2021/filters/main/Xinggsf_minority-mv.txt) | [国内推荐④](https://raw.fastgit.org/Bush2021/filters/main/Xinggsf_minority-mv.txt) | [国内推荐⑤](https://jsdelivr.b-cdn.net/gh/Bush2021/filters@main/Xinggsf_minority-mv.txt) |
