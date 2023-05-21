+++

author = "i0Ek3"
date = "2023-02-11"
title = "Write To The Freshmen Who Want To Enter The Internet Company" 
tags = [
    "Sharing",
]
categories = [
    "PK",
]

+++

# 写给想要进入互联网大厂的应届生们

如果你之前从来没有过任何实习、工作经验，那么我的这篇文字可以给你一个参考，让你知道互联网大厂内部的一些基本流程是什么样的，以及你如何才能更快上手工作，让你的 mentor 以及你的 leader 对你刮目相看。

## 建议

如果你可以出去实习，一定要去，去之前可以先看看我写的这篇文字，多少会能帮到你。不同大厂情况不同，但万变不离其宗。如果你能很早（比如大一或者大二）就出去实习，一定要珍惜这样的机会。大学四年，你就有多个大厂的工作经验。直接出生在了罗马，还是很香的。至于如何达成这个目标，需要大家各显神通了。而本篇文字，主打的就是快速上手。

## 基础

刷题和八股还是必要的，该背背，该刷刷。

基本的专业课程，如计算机网络，操作系统，数据结构，软件工程，这几个你能有个基本的认知就可以了，当然越深入越好。

编程语言，你一定要有一到两个很深入的，如果能了解到底层代码，那会更好。其他语言多少了解一些或者能用即可。

IDE 使用，或者 Vim 或者 VS 都可以，只要开发顺手就行。

Linux 的基本操作，如基本命令，配置文件修改等，你还是要非常熟悉的。毕竟入厂后，很多部分还是要和服务器打交道的。

数据库，你可以深入学习一下。尤其是如何连接数据库，如何写 SQL 语句，以及如何设计一张表，为何这么设计，以及内部的一些技术原理，你要有基本的认知。无论你是要做研发、测试、产品还是运营，会数据库操作就是不一样。

中间件，了解常用中间件的基本原理，如果有过实际使用能知道坑点所在以及如何解决，那么面试官一定会很喜欢你。如常见的 Redis、Kafaka、ElasticSearch、K8S、Docker、Jaeger 等。切记，除了原理你还要知道如何使用。

当然，上面说的这些如果你能在你的项目中有所体现，那一定会受到面试官的青睐的。

## 整合

上面的基础是必要，如果你能把基础整合起来，也就是串在你的项目中，那说明你的学习能力也是很强的。我们自己写项目可能不一定会想的很深，但是公司里面的项目结构是非常复杂的，比如接口的设计，数据库表的设计，架构的设计都是非常复杂的，都会经过技术选型的。为什么使用这个而不用别的，都是做了相应的权衡和考虑的。你的项目中也应该是这样的，要有你的深度思考，而不是为了写而写。

你可以多多发现生活中的需求，多记录，最后整合一下，写成一个项目。可以按照下面的研发流程来，走过一遍之后，你就知道公司内部大概的流程是什么样的了，只不过现在是你一个人而已，而公司内部是分工明确的不同角色，增加了沟通成本。

## 流程

大部分计算机相关专业的学生可能学过软件工程这个课程，这个课程其实真的很重要。一是告诉你软件开发流程，二是告诉你软件设计模式等。后者可能需要有较深的功力来贯穿整个职业身涯，这里我们主要先说前者。

软件开发流程无非就是需求确认、技术评审、开发测试、上线回归、复盘总结几个方面。等你真正来了公司，你会经历这其中的每一个流程。跟产品去对需求和排期，和技术老大以及产品们沟通技术方案，然后进行开发测试。测试分为自测和 QA 测试，没问题之后就要上线观测，看看是否存在异常，没有异常那么这一次开发就差不多结束了，复盘总结好的和不好的方面。如果代码出了 bug，那就需要改 bug，重新走一遍之后的流程。如果上线出了问题，那么看是回滚还是如何解决。这一步最容易出问题，因为考虑不周或者部署在各地的机器问题，导致上线故障，很可能会背一个 P 级别故障，那就比较尴尬了。所以，一定要仔细。

这里还有两个点，一个是代码开发。这个就比较考验你的功力了，你的代码是否优雅，是否性能更好，是否可复用可抽象，这都是你要考虑的问题。当然，刚开始会有人给你 CR 指导。另一个就是排期。这个需要你有效沟通，甚至需要反复沟通对齐，才能有一个好的结果。所以说，沟通也很重要。而公司里面，写代码的时间占比其实不多的，更多地是如何沟通、如何设计。只有清晰地沟通才能更好地设计，才能更快写出优雅的代码。

## 监控

大厂内部，项目上线后，都会有对应的软件进行业务指标监控，如果你能很快熟悉如何观察监控指标，那么一定会被刮目相看。所以你要知道目前市面上都有哪些监控组件，有哪些监控指标，这些指标都是什么意思？如 QPS、平响等。这样你就可以更快定位问题以及解决问题了。

## 能力

这里主要说独立思考以及解决问题的能力，这个不要求你多么地突出，工作中可以慢慢训练。但如果这方便你真的很突出，那会更好。工作中经常会遇到很多问题，有的是别人已经遇到过的，内部 wiki 可以搜搜看或者询问别人，前提是你做了功课，而不是遇到问题直接就去问。有的则是别人也没有遇到过，可能需要你自己定位问题然后解决问题，并记录在内部分享。这个过程才是真正的成长，你应该多经历才对。

那如何定位以及解决问题？当某个服务上线后报错，那你得先知道是报什么错，谁报的，什么时间报的，涉及的上下游服务是什么？IP 范围是什么？如果有部署，那涉及的实例有哪些？这个服务具体是调用了代码的什么接口，请求参数是什么？异常 case 是什么？持续时间多久？最近是否有什么操作？还是外部网络问题？你要有一个基本认知，然后确定是否需要和相关部门的研发沟通，请求对方帮助进行排查问题。如果自己实在解决不了的，及时跟你的 mentor 和 leader 沟通，他们会有对应的资源来解决这个问题。

当你想要往更高职级晋升时，那么独立解决问题的能力是必备的，并且你还要有大局意识，能横向 cover 住多个项目。

## 分享

内部会有很多分享，也可能会让你进行分享一个阶段的学习成果，那你会怎么进行这次分享呢？或者说考察你这个阶段的学习成果，叫你给组内的其他同事讲你学到的东西，你的结构会是什么样的呢？

结构很重要，不然是要挨怼的，所以无论是给别人讲东西还是要分享东西，都要有一个合理的结构。你可以从以下几个方面进行：业务流程，技术实现，模型设计。

业务流程就是你对某个业务的理解，背景、功能以及具体的流程。技术实现就是讲这个业务流程是如何通过技术实现的，技术选型是怎么做的。模型设计也很重要，就是说当前这个业务流程中的数据库表的定义是什么样的，为何要这么设计，每个字段都有什么意义。

你可以从宏观角度给大家讲一下这几个点的理解，然后细分的去讲每一部分。比如先大体介绍下你最近熟悉的业务是啥，它的模型设计是什么样子的，然后具体到业务流程中，是怎么操作的，会修改哪些表的那些字段，为什么要这样去做，有什么意义等。然后再从技术角度说明一下这个业务流程的实现，基本上你的整个流程就算是通了。

所以，如果你要进行分享，一定要有结构，多问自己为什么这样而不是那样，直到你能问到自己没有疑问了，那么别人在你的分享上大概也不会问出什么花样了，也会给别人留下好印象。

## 心态

实习也好正式工作也罢，你要转变心态，从学生的角色转变为打工人。这么说可能有点残酷，毕竟我还没毕业，但是你可以比别人更快适应环境，比别人有更多地机会，这就是卷吧。

另外，细心且大胆很重要。不要不敢去问，但要学会提问。不用在意别人对你的评价，你来这的目的要么学习东西，要么来赚钱的，所以其他的看淡一点，也就少很多烦恼。

挨怼不可怕，千万不要玻璃心。不要把事情往严重了想，出了问题总会有解决办法，不必压抑自己，事后总结复盘就好，下次不要再犯。总之，不要害怕。

## 模式

这个模式主要说几个方面吧，就是你要有逻辑思维能力以及目标为导向的意识。

什么意思呢？前者好说，就是你能把一个事情给对方讲清楚，逻辑结构层次分明。比如某个服务的业务流程，你能快速想到的是，首先这个服务是干什么的，有什么作用和功能，它存在的意义和背景是啥，用来解决什么问题，如何解决的，效果收益如何。

后者说的是，在公司里面，不管过程如何，我们要的是结果。说句不好听的，我不管你死活，把结果拿来给我。也就是说，不管你利用什么资源，自己加班熬夜还是跟别人请教，只要你能把我交代给你的事情拿出成果，那就好说。虽然很残酷，但确实也残酷，所以也要做好心理准备。

## 目标

这个目标说的是你对自己的规划，公司有对你的培养机制，你也要有对自己的目标，这并不冲突。如果你只是按部就班上下班，你很难获得更多地东西。如果你想要晋升，你就要做更多的事情来证明你的能力。

另一方面，现在的环境无法给你非常肯定的答案，你至少要有自己的目标给自己背书，不至于突然被 cut 掉而举足无措。所以对自己的提升很重要，你需要好好计划以实现定下的目标。

## 其他

你刚进去公司，mentor 会给你一些文档让你查看，这个时候你要知道怎么去看文档。就是反复去读，然后去查去了解对应知识点，直到文中没有你不清楚的东西。如果你只是囫囵吞枣的看文档，你会错过很多细节。而实际上，这些东西足够你了解全面了。因为后面一个月、两个月再回过头来看，你会发现，如果当时仔细点看这些文档，就不会走那么多弯路了。

进去公司的第一天，最好找人带你熟悉一下周围的环境，去哪吃饭，去哪领办公用品，周围的通勤车在哪，内部的活动以及福利如何开展，基础设施的使用等。不然等你自己发现，一是要很长时间，二是也会错过很多，三是很久之后依然不知道某个事件怎么操作以及怎么加入。

至于是否要加班，看你自己情况吧。一般对实习生没有特别多的要求，毕竟也不一定会留下。如果你觉着目前实习的部门不错，对个人发展和人员相处都有利，那就该花时间就花时间了解。如果你还有更好地选择，这里只是一个备胎，该面试就多面试，不要吊死在一棵树上。还是那句话，现在的环境没办法给你肯定的答案，多为自己考虑也是合理的。

再就是通过实习也可以想清楚和了解到这种环境是否是自己喜欢的，以及自己以后想做什么。趁着年轻，可以多经历一些事情。不过你要记着一点，很多事情不一定是你的问题，不需要自责。可能是整个公司架构就有问题，甚至是业务无法维持，甚至你的 leader 就喜欢 PUA 别人，以及你的同事就是不好相处等。你要搞清楚自己的定位，你来这的目的是什么，其他都是次要的。

## 最后

虽然说的是写给应届生的，但是很多东西都是通用的。如果你是经验丰富的老鸟，可以不必理会。对于初入职场的新人（比如你是跨行来的），可以参考。

核心就是你的竞争力要一直有，别人告诉你的东西要多思考，多质疑，不要全盘接收或者立刻否定，辩证的去看所有人和事。切记工作只是你的谋生手段，不要把所有重心都放在工作上，毕竟工作会发生变动。你要明白的是，这份工作会给你带来什么样的收益（能力、金钱、其他观念），以及你能撬动什么样的资源。

如果还有，那就未完待续。如果无了，那就后会有期。