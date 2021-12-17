2021最新省市区sql/json 文件

**最近更新（2021年6月19日）**：`master分支`增加了香港、澳门、台湾相关数据~



> [联动效果演示](https://gaohuazi.github.io/china_regions/)  
>
> [国内备用演示](https://static-16bf85f1-2181-4870-ac73-b170c68d178c.bspapp.com/)
>
> [淘宝领券浏览器插件（广告）](https://static-f7d1f66d-b388-4ba9-82f5-1d8ffc10e3ab.bspapp.com/)




> 分支说明：
> - `master分支`：3级联动-包括省、市、区，数据来源[腾讯位置服务（行政区划）API](https://lbs.qq.com/service/webService/webServiceGuide/webServiceDistrict)
> - `level5分支`：5级联动-包括省、市、区、街道、社区，数据来源于[国家统计局](http://www.stats.gov.cn/tjsj/tjbz/tjyqhdmhcxhfdm/)，数据比较old



### 目录结构描述
<pre>
├── json                        // json文件目录
│   ├── province.json           // 省
│   ├── city.json               // 市
│   ├── area.json               // 区
│   └── region.json             // 包含所有省市区数据
│   └── world.json             // 世界各个国家已经港澳台
├── sql                         // mysql文件目录
│   ├── province.sql            // 省
│   ├── city.sql                // 市
│   ├── area.sql                // 区
│   ├── init.sql                // mysql表结构文件, 需要5张表  
│   └── region.sql              // 包含所有省市区数据,只需1张表
├── LICENSE                     // MIT
└── Readme.md                   // help
</pre>

```mysql
# 导入sql时报错时可以尝试以下方式导入
mysql -uroot -p --default-character-set=utf8 dbname < /path/community.sql
```



### 克隆来源 https://gitee.com/gaohuazi/china_regions
