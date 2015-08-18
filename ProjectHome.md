基于位置的服务(Location Based Service，LBS)，它是通过电信移动联通等运营商的无线电通讯网络（如GSM网、CDMA网）或外部定位方式(如GPS)获取移动终端用户的位置信息（地理坐标，或大地坐标），在GIS(Geographic Information System，地理信息系统)平台的支持下，为用户提供相应服务的一种增值业务。

Open-JLBS是一个纯Java开发的LBS基础系统。它实现了LBS的基本功能，包括但不限于：<br />
1.定位数据的存储，删除及查找（CRUD）<br />
2.用户签到checkin<br />
3.用户UGC地理位置POI数据生成<br />
4.根据指定范围查找附近用户及POI<br />
5.定位最后一次签到lastcheckin数据<br />

为适应高并发及高可用性，本系统使用了ActiveMQ及Memcached进行读写及缓存操作，关于相关的开源软件，请参考以下url：<br />
http://activemq.apache.org/<br />
http://code.google.com/p/spymemcached

本系统特点：<br />
1.可以方便的以spring SOA服务的方式发布<br />
2.基于Spring3.x的高可用性系统<br />
3.多数据库支持，目前打算实现MySQL，mongodb等<br />
4.查找附近使用多种算法实现<br />
5.高并发下可选同步或者异步操作<br />

本系统下一步打算实现的功能：<br />
1.完成多数据库支持<br />
2.附近群组功能引入<br />
3.定位例程提供<br />
4.查找附近使用空间地理位置等多种算法实现<br />
5.加权排序算法<br />

请笑纳开源社区的这朵小花。