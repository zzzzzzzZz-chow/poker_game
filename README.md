# 项目作者：shaohua ye
---
## Card类
单张扑克牌，有花色（suit）、数字（number）属性，属性用枚举实现。
---
## Poker类
一套扑克牌，还未写，预计其中一个属性为顺序的Card组合和一个随机的Card组合，有一随机化方法，用于生成随机扑克牌。发牌操作，将随机后的扑克牌pop_back一次。
---
## Player类
用于作为玩家和人机，有两张牌槽用于存放手牌，有一个状态用枚举类型实现，类容为“大盲，小盲和庄家“三种。 有资金池属性，用于计算资金，并有相应接口增加和减少。有计算自己与牌池中组合的最大牌型的位置。
---
## Pool类
牌池，共3，1，1张牌，发牌后根据流程依次翻开，翻开前属于不可见状态。
---
## Rule类
控制游戏流程，做洗牌、发牌、下注、翻牌的工作。
---
## Robot类
每个robot控制一个player，有根据自己手牌和牌池计算最大牌可能结果，并且结果越高越有投机下注可能。
