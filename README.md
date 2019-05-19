# Web

### 01-Fibonacci
### 要求：实现Fibonacci数列。函数名为 Fibonacci.of()，静态方法，入参是int，返回值是int。
### 在main函数用循环打印1~200的Fibonacci数列
### 考虑到数值越界问题，故采用BigInteger解决此问题

### 02-德州扑克
一副扑克有52张牌，每张牌由一个花色和一个数字构成。  
花色为以下四者之一：方片 D、黑桃 S、红桃 H、梅花 C
数字为以下13者之一，且大小顺序如下：2, 3, 4, 5, 6, 7, 8, 9, T, J, Q, K, A
花色是大小无序的，但数字有序，2最小，A最大。

一手牌有5张。根据花色和数字的不同，其大小按照以下规则决定。
满足下面规则的手牌会大于满足上面规则的手牌。  
同花顺＞铁支＞葫芦＞同花＞顺子＞三条＞两对＞对子＞散牌

散牌：
不符合其他任何规则的五张牌。 比较最大一张牌的大小，如果相同，比较第二大的牌的牌点数，如果五张牌的牌点数都相同，则为平局。  
对子：
有两张同样大小的牌片。 比较两张大小一样的牌的牌点数，如果相同，依次比较剩余的三张牌大小。若大小都相同，则为平局。  
两对：
有两个对子牌。 比较大对子的大小，若相同，比较小对子的大小，若还相同，比较单张牌的大小，若还相同，则为平局。  
三条：
有三张同样大小的牌片。 比较三张大小一样的牌的牌点数大小。  
顺子：
五张相连的牌。 比较最大的牌点数。若大小都相同，则为平局。  
同花：
五张牌的花色相同。 按照散排规则比较大小。  
葫芦：
三条+对子。 比较三张大小一样的牌的牌点数。  
铁支：
有四张同样大小的牌片。 比较四张大小一样的牌的牌点数。  
同花顺：
同一种花色的顺子。 比较最大的牌的牌的大小。若大小都相同，则为平局。
### 要求：为两手牌判断大小。

### 03-SpringBoot
使用SpringBoot框架，构建一个Restful API，能够完成Todo list的以下功能。  
返回所有Todo任务  
创建一个新的Todo任务  
返回一个指定ID的Todo任务  
删除一个Todo任务  

Todo中一个任务的JSON格式定义为：  
  {  
    "id": 1,  
    "content": "Restful API homework",  
    "createdTime": "2019-05-15T00:00:00Z"  
  }  
进一步的功能提示：需完成的四个功能的Restful API定义如下，实现即可。  
GET /api/tasks/  
POST /api/tasks/  
GET /api/tasks/{id}  
DELETE /api/tasks/{id}  
