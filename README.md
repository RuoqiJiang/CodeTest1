# CodeTest1
# Bundle Calculator

## Context
Social media Influencers have been basing the price of their social 
media post on a single post basis. 
社交媒体网红按照发一个post来收费
So If a brand required 10 posts (for example spread over a period) 
then they would be charged 10x the cost of a single post. 
所以，如果一个品牌需要10个帖子（在过去的一段时间内散播），那么他们将被收取单个帖子
10倍的成本
One company has decided to allow social media influencers to sell 
posts in bundles and charge the brand on a per bundle basis. 
一家公司决定让网红来捆绑销售他的帖子，按照捆绑销售的模式来收费
So if the Influencer sold image based posts in bundles of 5 and 10 and 
brand ordered 15 they would get a bundle of 10 and a bundle of 5.
因此，如果网红以5张和10张为一组来卖带图的帖子，而这个品牌定了15张，
则会分别获得10张和5张的捆绑销售

The company currently allows the influencer to monitize the following
submission formats:
公司允许网红赚钱的提交模式：

Submission format | Format code | Bundles
----------------- | ----------- | -------
Image             |    IMG      | 5 @ $450 10 @ $800     //5个450/10个800
Audio             |    Flac     | 3 @ $427.50 6 @ $810 9 @ $1147.50 //3个427.50 /6个810 /9个1147.50
Video             |    VID      | 3 @ $570 5 @ $900 9 @ $1530 //3个570 /5个900 /9个1530


## Task
Given a brands order, you are required to determine the cost and bundle
breakdown for each submission format. For simplicity, each order should 
contain the minimal number of bundles.
在给定品牌订单的情况下，需要确定每种提交模式的成本和捆绑明细
为简单起见，每个订单应包含最少数量的捆绑包5/3/3

### Input:
Each order has a series of lines with each line containing the number 
of items followed by the submission format code
每个订单都有一系列行，每行都包括项目数量和format code
An example input:
```
10 IMG
15 FLAC
13 VID
```

### Output:
A successfully passing test(s) that demonstrates the following output: 
(The format of the output is not important)
成功通过的测试演示以下输出，格式不重要
```
10 IMG $800
  1 x 10 $800
15 FLAC $1957.50
  1 x 9 $1147.50
  1 x 6 $810
13 VID $2370
  2 x 5 $1800
  1 x 3 $570
```
