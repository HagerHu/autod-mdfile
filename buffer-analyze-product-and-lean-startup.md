---
title: "梦想远大，行动务实，打造最小可爱产品之路"
date: 2023-06-06T15:24:20+08:00
draft: false
Summary: Tom Redman 和他的团队在 Buffer 内建立的社交分析解决方案 Buffer Analyze，并且很幸运地发现了产品/市场契合的早期迹象。这篇文章可以看做精益创业在 Buffer Analyze 实践，如何在限制条件下工作，如何确定新产品特性的范围，以及如何为客户构建和发布价值。
Description: Tom Redman 和他的团队在 Buffer 内建立的社交分析解决方案 Buffer Analyze，并且很幸运地发现了产品/市场契合的早期迹象。这篇文章可以看做精益创业在 Buffer Analyze 实践，如何在限制条件下工作，如何确定新产品特性的范围，以及如何为客户构建和发布价值。
keywords: ["湾区周报","精益创业","Buffer Analyze","产品范围","用户故事","工程范围","敏捷开发"]
categories:
  - "走向独立"
tags:
  - "记录量化"
  - "精益创业"
  - "Buffer Analyze"
image: "https://buffer.com/resources/content/images/size/w2000/format/avif/wp-content/uploads/2018/10/Buffer-product-process-product-scoping-and-user-stories.jpg"
---

![gap-between-goal-and-real](https://circle-picgo.oss-cn-shanghai.aliyuncs.com/img/CleanShot%202023-06-04%20at%2022.07.49@2x.png)

这篇文章来自 Buffer Blog，文章内容可以看作精益创业在 Buffer Analyze 实践。讲述了如何在限制条件下工作，如何确定新产品特性的范围，以及如何为客户构建和发布价值。如果你想阅读英文，点击 [Dream Big, Go Small, and the Path to a Minimum Lovable Product](https://buffer.com/resources/product-scope/) 阅读英文原文。

---

过去一年里，我和我的团队一直在Buffer内建立一个全新的社交分析解决方案，叫做 Buffer Analyze。我们尽力将研究、数据和直觉融合成一个精简、可爱的解决方案，并且我们很幸运地发现了产品/市场契合的早期迹象。

（目前，Analyze beta 版本对 [Buffer for Business](https://buffer.com/business?ref=buffer.com) 客户开放。您可以 [在这里](https://buffer.com/analyze?utm_source=open-blog&utm_campaign=scope-post) 了解更多关于Analyze 的社交分析功能。）

我们有很多想要在 Analyze 上实现的功能，因为我们相信有很多东西会带来价值。同时，我们也受到了作为 Buffer 内非常小团队的资源限制。

老实说，我不希望有其他的方式。紧密的限制迫使我们在产品设计和开发中采取创造性、有纪律和批判性的方法。

这个产品是在权衡取舍的微妙平衡下产生的。

我很兴奋地分享更多关于这些取舍的信息：我们如何在限制条件下工作，如何确定新产品特性的范围，以及我们如何为客户构建和发布价值。

## 在确定范围之前：先追求宏伟目标，然后再着手细节

当涉及到实现产品特性时，我通常会先追求宏伟目标，然后再着手细节。

一旦我认为已经确定了我们最大的机会（这是一个值得单独一篇文章的过程！），我就会与我们的 Analyze 设计师 James 一起审查几个潜在的解决方案。最终，我们会选择一个我们认为符合要求的设计，详细阐述许多细节，并原型化相关的工作流程。在这个过程中，我们也总是包括工程师，以便及早获得对设计和想法的反馈。

例如，这是我们探索新的hashtag分析工具的一个解决方案。我们最终构建了完全不同的东西！

![[Pasted image 20230606145207.png]](https://buffer.com/resources/content/images/wp-content/uploads/2018/10/product-scope-early-wireframe-mockup.jpeg)

![[Pasted image 20230606145216.png]](https://buffer.com/resources/content/images/wp-content/uploads/2018/10/produt-scope-early-mockup-prototype.png)

这种探索的结果通常是一个可点击的原型，以及我们在这个过程中所做选择的详细规范，我们简称为“specs”（规范）。 （我们的规范是非传统的：我们的规范不是长篇的高度技术化、结构化的文档，而是用自然语言编写的，具有我们提出解决方案的合理分解。）

**设计和规范通常代表了特性的理想版本，即如果我们可以做到完美，我们会这样做的版本。**

**但是，当然，我们不能做到完美...也不应该这样做！**

在一个资源有限、机会成本高的小团队中，为了最大化价值而不是完整性，对我们的用户最有利。

很多时候，特性的完整性并不能直接服务于核心工作，而是提供便利。便利本身并不是没有价值的，但当一个产品处于非常早期的阶段时，通过提供核心价值来找到产品/市场契合是至关重要的。_验证您正在构建正确的东西比其他任何事情都更重要。_

因此，有了我们功能齐全、方便实用的原型，现在是时候退后一步，审视设计了。

我们需要建造所有这些吗？

几乎所有时候的答案都是不需要的；我们不需要所有这些来提供核心价值。

在实际构建特性之前，我们经历了三个阶段的范围确定：
- 产品范围确定
- 技术范围确定
- 周期范围确定

是时候开始确定范围了！


## 第一步：产品范围确定和用户故事

在产品范围确定阶段，产品经理和设计师一起设计我们想要在即将到来的开发周期中解决的特性或特性集。最终我们得到的是一个具体、功能齐全、如果我们可以做到完美的版本。这个范围几乎总是比我们最初要构建的范围大。

一旦我们设计好了特性，我们会明确地花时间缩小范围，确定最小可爱版本，即仍然为用户提供实质价值的最小版本。

**任何比最小可行版本更小的东西都不能完成任务，因此不值得构建。**

--- 
小贴士！

你几乎总是可以发布比最初想象的更小的版本！在快速发布和更快学习的精神下，努力做到更小。

举个例子：当我确定 Analyze 的最小版本时，我的研究和直觉都告诉我，我们需要一个简单的比较工具作为基线最小特性。我相信没有这个功能，没有人会为我们的产品付费，但我错了。比较功能的构建时间比我们计划的要长一些，我们决定在没有它的情况下发布 Analyze，看看会发生什么。结果，我们即使没有比较工具，也赢得了第一批满意的付费客户！

这是一个很好的机会，_测试我的假设，即人们需要比较工具才能获得足够的价值，而这个假设被愉快地否定了_。这种经验使我渴望深入质疑每个新产品或特性的“必备”方面。

---

例如，我们发现用户可以从更好地了解他们的 hashtag 如何影响用户触达和参与中获得很多价值。经过几次设计探索，我们得出了这个功能齐全、如果我们可以做到完美的 Hashtag 分析模块：

![[Pasted image 20230606134633.png]](https://buffer.com/resources/content/images/wp-content/uploads/2018/10/product-scope-mockup-full-feature.png)

<p style="text-align: center;">This is the full-featured, if-we-could-do-it-all version of our Hashtag Analysis module</p>

以下是我们实际构建的内容：

![[Pasted image 20230606134704.png]](https://buffer.com/resources/content/images/wp-content/uploads/2018/10/Hashtag-performance-feature-Buffer-Analyze.png)

<p style="text-align: center;">And this is the version that we actually built</p>

请注意，范围大大缩小，但它提供的价值几乎相等。**我非常相信80/20法则，并且它适用于这里：这个特性的最小版本的大小是初始范围的20％，但它提供了预期价值的80％。** 这已经足够提供足够的价值来解决我们用户的挑战（了解 hashtag 的表现）。在产品开发领域，这是一个不错的权衡。

一旦我们确定了我们的功能齐全的解决方案，我会将其分解成用户故事。

用户故事是用户可见价值的离散块。我们使用以下格式：

_“作为一个<用户类型>，我想要<某种目标>，以便<某个原因>”_

然后附加设计、细节和验收标准。

有时一个故事足以代表一个完整的特性，但更常见的情况是一个特性会成为几个用户故事：每个故事都是一个离散的、可交付的价值块。

![[Pasted image 20230606134809.png]](https://buffer.com/resources/content/images/wp-content/uploads/2018/10/user-stories-example-screenshot.png)

<p style="text-align: center;">Example of a user story: One of our three user stories for Analyze’s upcoming Audience section</p>

然后，我们将完整的用户故事列表缩小到一个更小的子集，这将代表我们的最小可爱版本。例如，原型可能会产生五个用户故事，但我们的最小版本将只包含其中的两个。

## 第二步：技术范围确定和估算

准备好设计、产品规范和我们缩小的用户故事后，我们作为一个整体团队会聚在一起，一起浏览用户故事。工程师经常会提出澄清问题，我们将根据需要一起调整故事的细节。

一旦工程师满意地认为他们完全理解了问题和我们提出的解决方案，他们将把用户故事分解为工程任务。

**工程任务是离散的任务，用一个故意粗略的可能估计集来估算：一天、三天或一周**。估计工作超过一周的任何任务都应该进一步分解。

估计是由工程师合作得出的，具有两个主要目的：

1. 确保所有工程师在每个任务所需的工作量方面大致上保持一致

2. 为产品经理提供周期规划的一般直觉检查。

估计不用作工程师的责任衡量标准。我们只想知道我们在估算工程任务方面做得还不错（这是一个众所周知的难以做好的事情！），并且我们都同意任务的内容。

## 第三步：周期范围确定和规划

现在我们有了用户故事列表和代表其现实的工程任务，我使用这些信息来规划我们的开发周期。我们目前正在进行六周的开发周期，但我只打算在一开始规划前四周。在周期的第三周，我会审视我们的进展情况，重新排序事项，并规划周期的下半部分。

<mark style="background: #FF5582A6;">有了工程任务，我能够在可用时间的背景下优先考虑我们的用户故事。</mark>我们通常会同时处理两个甚至三个特性，估计将帮助我决定哪个应该先做。

例如，如果我们有三个用户故事，如果“最小价值”的那一个比其他两个需要的时间少得多，我仍然可能选择这个。这可以更快地为我们的用户提供价值。

请容忍我，我还会将一些故事的范围扩大到我们的最小可爱版本之外。

我知道，我知道！我一直在宣扬范围缩小的优点，然后再进一步缩小范围。

但是想象一下一个可以容纳五块石头的罐子。即使你不能放第六块石头，五块石头之间仍然有空间，也许我们可以在那个空间里放十个小石子。

在这个类比中，罐子是我们 的六周周期，石头是满足我们最小可爱特性要求所需的用户故事，小石子是超出我们最小要求的更小的用户故事或工程任务。这是一个很好的方式，可以为特性或产品增加一些“惊艳因素”，而这些因素并不严格要求提供价值。

![[Pasted image 20230606135010.png]](https://buffer.com/resources/content/images/wp-content/uploads/2018/10/jar-of-rocks-and-pebbles-product-scope-742x1024.png)

归根结底，**周期范围确定在很大程度上是平衡尽快为用户提供价值和提供最大价值的问题**（有时候你会很幸运，这两个因素是一样的！）。这种平衡影响我们构建什么以及何时构建它。

## 让我们回顾一下

### 产品范围确定（由产品经理负责）
- 设计解决方案以解决当前问题
- 为解决方案创建规范细分
- 将此规范转化为用户故事
- 要小而精：定义能够提供价值的最小版本特性

### 技术范围确定（由工程经理负责）
- 使整个团队对规范和用户故事达成完全一致和理解
- 将用户故事分解为技术任务
- 估计技术任务

### 周期范围确定（由产品经理负责）
- 根据估算，选择哪些故事和任务将在当前开发周期内完成
- 将所有其他故事和任务留到另一天

如果你好奇这个范围确定过程中谁负责什么，它看起来像这样：

![[Pasted image 20230606135127.png]](https://buffer.com/resources/content/images/wp-content/uploads/2018/10/product-scoping-accountabilities.png)

<p style="text-align: center;">How we break down the accountabilities for new feature development on Buffer Analyze</p>

## 现在轮到你了

这个过程是许多迭代的结果，它随着时间的推移不断发展。它绝不是产品开发的最佳方法，但我们发现它在我们特定的产品开发周期中非常有效。话虽如此，我们始终在积极寻找方法来改进我们的流程，使团队更加舒适和高效。
