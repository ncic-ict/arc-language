ARC v0.1.0
===========
*Arc means Readable Configuration*

Purpose
-------

- ARC 是一种可读的序列化格式, 可以作为配置文件和日志文件
- ARC 可以无歧义地映射为哈希表, 其他语言能很容易的解析出封装的数据结构.
- ARC 被设计成能压缩成单行, 也就是说换行和空格是无所谓的.

Table of Contents
-----------------
- [字符串](#standard-string)
- [键值对](#user-content-keyvalue-pair)
- [字典](#standard-dict)
- [列表](#standard-list)


[字符串](#standard-string)<a id="user-content-string">&nbsp;</a>
------------------------------------------------------------------------------------------------------------------------
用成对符号 `" "` 括起的部分是字符串, 支持使用 `\"` 逃逸.


[键值对](#user-content-keyvalue-pair)<a id="user-content-keyvalue-pair">&nbsp;</a>
------------------------------------------------------------------------------------------------------------------------

> ARC 被设计成可以无歧义地映射为哈希表

因此 ARC 最基本的构成单元是键值对。

键名在等号的左边而值在右边, 键名和键值周围的空白会被忽略。  
