---
title: 两个月的某大厂手机商城外包开发
categories:
  - 工作
tags:
  - web
---

说实话，这是开始干前端后第一次做“大厂，大项目”，而从公司神秘的召集了几个人开会的那一天就觉得这项目会有点坑。

两个月前，小老板大老板召集了七八个人，其中就我和另外一个“无臂少年”是前端，我猜应该是那个实际报七八个人的工作量，但是只有一两个人干活的套路了。这之后的两个月每天都晚上12点左右才走，开发路程异常艰辛。

## 关于项目

项目用了之前之看了一眼，没实际用过的nuxt，开发起来其实还行。可能大坑还没遇到。主要注意点是是服务端和客户端渲染，ui框架我随便提了一个vuetify，最后居然就用这个了，很多ui组件样式都有覆盖重写，感觉提高了开发效率，但也没有完全提高。

此商城有一个后台，几乎所有数据都是通过一个固定编码请求接口然后渲染，测试环境配置测试数据着实扯了一番皮，因为是外包套外包，所以不能直接和“大厂”那边沟通，这两个月把所有能骂的脏话都骂了。

## 外包套外包

最后实际开发的真就只有我和无臂少年，还有一个说是刚学前端的后端，没有参与实际开发。一手外包那边有三个势力，总负责人、设计、一个前端架构师，架构师似乎是他们的懂代码的，来和大厂那边沟通技术问题。由于项目很急，设计稿开发了半个多月才有部分定稿，大厂那边的后台文档问题经常一问三不知，最坑的问题就是整个页面数据逻辑，到临交付还要大改一遍，真不知道这个前端架构师怎么和那边确认的。最傻的还是我们反馈的开发问题，他们和大厂一聊完全不是一个问题，最后还是开会我们一起开才稍微解决一些问题。

## 爹妈不疼的pc网站项目

这次开发最神奇的还是属于要我们参考m站——一个已经上线的手机web站，经常是看着m站的请求，来猜测这里应该用什么接口，参数是啥，这个返回是什么意思。一个搜索接口由于m站的不符合需求，前后改了半个月，最后用这个新做的接口。其次就是各种请求到的数据里的链接，五花八门，我一开始以为需要他们运营自己配，然后测起来，问为啥都是跳m站了，有的跳旧pc站，有的跳app链接，我想你他妈让我们用的都是旧接口，人家还没针对新pc做兼容和配置，可不是瞎几把跳么。后来也不知道怎么着，要把所有链接转化成新pc站链接，整个就很扯。

## 最后

整个项目几乎没有用什么新技术（ nuxt 除外），ts也仅限于基本类型注释，其他基本都是写没什么技术含量的业务代码，和对着设计图扣扣扣，然后给设计指指点点的css。另外还有埋点是头一遭，一开始被 ublock 把埋点的 jsdeliver cdn 屏蔽了，差点给整懵逼，所以说，以后还是继续开着 ublock 冲浪吧，不然你在他们页面干点啥，他都得统计。

大厂项目其实就这，外包到最后轮到我这菜鸡来做，这项目就凉一半了，做到最后无臂哥已经跑路了，本来最恶心的商详和购物流程是他负责的，害，前途茫茫……