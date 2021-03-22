---
id: crab-crowdloan
title: Kusama 平行链拍卖众贷
sidebar_label: Kusama 平行链拍卖众贷
---

Kusama 允许平行链在去中心化的众贷系统中为平行链竞拍提供 KSM。

任何平行链项目团队都可以为平行链插槽创建新的众贷活动。一次众贷活动需要提供插槽使用时间（即，平行链将竞标的持续时间），上限和众贷的持续时间。在众贷时间范围内可以持续数次拍卖，这意味着团队无需因为没有在第一次尝试中获得插槽而重新开启众贷。

每个已创建的众贷都会有一个 Index。众贷开启后，任何人都可以通过发送一笔包含项目方 Index 的特殊交易来参与。用于参与众贷的 KSM 必须为可交易的状态，不包括任何形式的锁定，如质押、投票或者治理）。

> 重要提示：所有众贷捐款均由众贷模块的逻辑处理。为了准确识别项目方，请填写相应众贷活动的 Index 而非地址。

平行链项目方可以决定是否以及如何奖励那些放弃质押收益的参与者，并选择锁定他们的 KSM 以支持平行链的竞选活动。可以想象，奖励将采用多种形式，并且在各个项目中可能会有很大差异。

在众贷活动的某个阶段，项目方将上传平行链数据。理想情况下，项目方在向参与贡献的用户发放奖励前进行此操作，以便参与的用户可以对其进行验证。在活动过程中，数据只能上传一次，这将作为平行链的 runtime 部署。当然，一旦平行链开始运行，它可以通过升级 rumtime 来更改（由其自身的本地治理确定）。

如果众筹活动成功，该平行链将在 Kusama 网络上线。筹集的KSM在活动期间（最多两年）将被锁定在该平行链账户中。

> 注意：用户的 KSM 不会脱离用户的钱包账户(托管给交易所的除外）

参与者将能够通过以下两种方式之一来收回其 KSM：

- 如果活动成功，则平行链将在其租约结束时进入退出阶段。在此阶段中，参与者可以赎回参与的 KSM。

- 如果竞选未成功，则可以在竞选结束后的退出阶段内，参与者也可以撤回其 KSM。

> 注意，退出 KSM 需要为每个参与者进行交易。任何人都可以进行交易，因此平行链团队可以批量释放每个参与者的 KSM。在一定时间内未撤出的代币将进入 Kusama 国库。