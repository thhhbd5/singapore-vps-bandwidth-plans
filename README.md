# 新加坡大带宽VPS推荐：1Gbps 还算大带宽吗？端口、月流量、超限限速怎么算，五家全套餐对比与按场景选型（含优惠码、退款期对照）

新加坡机房里 1Gbps 端口早就是标配，2Gbps、3Gbps 也不稀奇，所以“大带宽”这三个字放在新加坡这个节点上，本身几乎不构成差异。真正把体验拉开的是另外三件事：回程走哪条线、月流量池有多大、流量跑完之后被限成什么样。这篇按这三条把 GoMami、ByteVirt、荫云、搬瓦工和 LisaHost 五家的新加坡在售套餐摊开对比，最后给一张“你的情况该买哪台”的对照表。

## 赶时间的话

> - **要大陆三网晚高峰稳、正经建站** → GoMami SIN Pulse，年付 8 折循环，Nano 折合每月约 $23.2
> - **极致低价跑量、要 40TB / 100TB 这种真大流量** → ByteVirt 标准版的大流量档
> - **做 TikTok、Shopee、店铺账号，要新加坡原生 IP** → LisaHost，68 元起，48 小时可退
> - **只要国际线路、预算能压多低压多低** → 荫云，7 折后 $7/月拿到 1Gbps + 2TB + 双原生 IP
>
> 👉 [查看 LisaHost 新加坡原生 IP 套餐（48 小时不满意无条件退款）](https://lisahost.com/aff.php?gid=15&aff=1587)

## 先把“大带宽”拆成三件事

**端口带宽**是理论峰值。1Gbps 折合约 125MB/s，5Gbps 约 625MB/s。但这是机房到交换机那一侧的数字，不是你从国内拉文件的速度。同样标 1Gbps，共享出口的机器晚高峰能跑出 50Mbps，精品回程的机器能贴着标称值跑，两者的月付价差可能就是两三倍。

**月流量池**决定这个端口你能用多久。ByteVirt 标准版最便宜那档给 500Mbps 端口配 500GB 月流量，按满速算两个多小时就见底——端口数字很漂亮，实际能跑的量被流量池卡住了。同一家的 VPS-2C4G100T-KVM-SG 是 1Gbps 配 100TB，满速跑要九天多才跑得完，那才叫大带宽。这两台机器放在一张表里都写“1Gbps”，含义完全不同。

**超流量之后被限成什么样**，这一条比端口是 1G 还是 2G 更影响实际体验，但绝大多数测评文章不写。GoMami 的出站流量超限后限到 20KB/s，一个月顶多再挤出 50GB 左右；ByteVirt 标准版限到 1Mbps，折合约 128KB/s，一个月还能跑 330GB 上下。同样叫“限速”，差六倍多。

按流量算单价，差距更直白：GoMami Nano 月付 $29 买 500GB，折合 $58/TB；ByteVirt 的 100TB 档 $100 一个月，折合 $1/TB；荫云 7 折后 $7 得 2TB，$3.5/TB；LisaHost 基础版 68 元给 6000GB，每 TB 约 11 元。建站机买的是线路和稳定性，跑量机才该盯这个数字，两者不该用同一套标准打分。

## 全套餐对比

以下价格均为各家官方标价，实际以下单页为准。美元标 $，LisaHost 单独用人民币计价。

### GoMami SIN Pulse（全系 AMD EPYC 7763，600Gbps DDoS 防护）

| 套餐 | 配置 | 月流量 | 端口 | 超流量 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- |
| Nano | 2核 / 2GB / 40GB NVMe | 500GB | 1Gbps | 出站超限 20KB/s | $29/月；$348/年，8折 $278.4（约 $23.2/月） | [入手 Nano 年付，折合每月约 $23](https://bit.ly/Gomami) |
| Mini | 2核 / 4GB / 60GB NVMe | 1TB | 1Gbps | 同上 | $49/月；$588/年，8折 $470.4（约 $39.2/月） | [查看 Mini 套餐与年付折扣](https://bit.ly/Gomami) |
| Air | 4核 / 8GB / 80GB NVMe | 2TB | 1Gbps | 同上 | $89/月；$1068/年，8折 $854.4（约 $71.2/月） | [选 Air 跑电商站与 API](https://bit.ly/Gomami) |
| Pro | 8核 / 16GB / 100GB NVMe | 5TB | 3Gbps | 同上 | $169/月；$2028/年，8折 $1622.4（约 $135.2/月） | [看 Pro 的 3Gbps 端口与 Windows 支持](https://bit.ly/Gomami) |
| Ultra | 12核 / 32GB / 300GB NVMe | 10TB | 5Gbps | 同上 | $338/月；$4056/年，8折 $3244.8（约 $270.4/月） | [查看旗舰 Ultra 配置](https://bit.ly/Gomami) |

线路是去程电信 163、联通 10099、移动 CMI，回程电信 CN2、联通 9929、移动 CMIN2。第三方测评站 DigVPS 的记录里，电信约 60–80ms、联通约 70–90ms、移动在相近区间。Nano、Mini、Air 不能装 Windows，Pro 及以上可以。

### ByteVirt SG-China Optimized（中国优化线）

| 套餐 | 配置 | 月流量 | 端口 | 超流量 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- |
| VPS-512-KVM-Premium-SG | 1核 / 512MB / 15GB NVMe | 500GB | 500Mbps | 未标注 | $15/季 | [看最低配 Premium 季付](https://bytevirt.com/aff.php?aff=1107&pid=38) |
| VPS-1024-KVM-Premium-SG | 1核 / 1GB / 30GB NVMe | 1TB | 800Mbps | 未标注 | $10/月 | [选 1024 Premium，1TB 流量甜点档](https://bytevirt.com/aff.php?aff=1107&pid=39) |
| VPS-2048-KVM-Premium-SG | 2核 / 2GB / 50GB NVMe | 1.5TB | 1Gbps | 未标注 | $15/月 | [查看 2048 Premium 配置](https://bytevirt.com/aff.php?aff=1107&pid=40) |
| VPS-4096-KVM-Premium-SG | 2核 / 4GB / 50GB NVMe | 2TB | 1Gbps | 未标注 | $20/月 | [入手 4096 Premium](https://bytevirt.com/aff.php?aff=1107&pid=41) |
| VPS-8192-KVM-Premium-SG | 4核 / 8GB / 50GB NVMe | 5TB | 1Gbps | 未标注 | $50/月 | [看 8192 Premium 的 5TB 流量](https://bytevirt.com/aff.php?aff=1107&pid=42) |
| VPS-16384-KVM-Premium-SG | 8核 / 16GB / 100GB NVMe | 10TB | 1Gbps | 未标注 | $100/月 | [查看 16384 Premium 顶配](https://bytevirt.com/aff.php?aff=1107&pid=43) |

### ByteVirt VPS-SG-KVM（标准版，超流量限速 1Mbps）

| 套餐 | 配置 | 月流量 | 端口 | 超流量 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- |
| VPS-512-KVM-SG | 1核 / 512MB / 8GB NVMe | 500GB | 500Mbps | 限速 1Mbps | $16.88/年 | [年付 $16.88 的入门档](https://bytevirt.com/aff.php?aff=1107&pid=44) |
| VPS-1024-KVM-SG | 1核 / 1GB / 10GB NVMe | 750GB | 500Mbps | 限速 1Mbps | $22/年 | [选 1024 标准版年付](https://bytevirt.com/aff.php?aff=1107&pid=45) |
| VPS-2048-KVM-SG | 2核 / 2GB / 20GB SSD | 1TB | 500Mbps | 限速 1Mbps | $8/季 | [看 2048 标准版季付](https://bytevirt.com/aff.php?aff=1107&pid=46) |
| VPS-2560-KVM-SG | 2核 / 2.5GB / 20GB NVMe | 1.5TB | 500Mbps | 限速 1Mbps | $3.5/月 | [月付 $3.5 的 2.5GB 内存档](https://bytevirt.com/aff.php?aff=1107&pid=47) |
| VPS-4096-KVM-SG | 2核 / 4GB / 40GB NVMe | 2TB | 500Mbps | 限速 1Mbps | $5/月 | [入手 $5 月付的 4GB 档](https://bytevirt.com/aff.php?aff=1107&pid=48) |
| VPS-2C4G80G-KVM-SG | 2核 / 4GB / 80GB NVMe | 2TB | 500Mbps | 限速 1Mbps | $9/月 | [看 80GB 存储版本](https://bytevirt.com/aff.php?aff=1107&pid=49) |
| VPS-8192-KVM-SG | 4核 / 8GB / 60GB NVMe | 2.5TB | 800Mbps | 限速 1Mbps | $12/月 | [查看 4核8G 标准版](https://bytevirt.com/aff.php?aff=1107&pid=50) |
| VPS-16384-KVM-SG | 8核 / 16GB / 120GB NVMe | 5TB | 1Gbps | 限速 1Mbps | $30/月 | [选 8核16G 标准版](https://bytevirt.com/aff.php?aff=1107&pid=51) |
| VPS-4096-KVM-SG-150G-40T | 4核 / 4GB / 150GB SSD | 40TB | 1Gbps | 限速 1Mbps | $66/月 | [看 40TB 大流量档](https://bytevirt.com/aff.php?aff=1107&pid=52) |
| VPS-2C4G100T-KVM-SG | 2核 / 4GB / 80GB NVMe | 100TB | 1Gbps | 限速 1Mbps | $100/月 | [入手 100TB 跑量机型](https://bytevirt.com/aff.php?aff=1107&pid=53) |
| VPS-KVM-10C10G-SG-200G-100T | 10核 / 10GB / 200GB SSD | 100TB | 1Gbps | 限速 1Mbps | $129/月 | [查看 10 核 100TB 顶配](https://bytevirt.com/aff.php?aff=1107&pid=54) |

ByteVirt 的延迟记录：电信约 80–145ms（部分地区走 163，部分走 4837）、联通约 82–115ms（AS4837）、移动约 60–90ms（CMI）、新加坡本地约 2.58ms。路由描述里，电信从广州出口直连，联通从北京出口经日本节点，移动从上海出口经香港节点——所以“三网直连”这个标签不太站得住，看具体路由更实在。IP 不是原生，但 Netflix、TikTok、ChatGPT 的解锁表现尚可。

### 荫云（国际线路，双原生 IP）

| 套餐 | 配置 | 月流量 | 端口 | 原价 | 7折后 | 购买 |
| --- | --- | --- | --- | --- | --- | --- |
| 入门 | 1核 / 1GB / 10GB | 2000GB | 1Gbps | $10/月 | $7/月 | [看荫云 $7 入门档](https://t.co/j2RgxyPl9x) |
| 标准 | 2核 / 2GB / 20GB | 4000GB | 1Gbps | $16/月 | $11.2/月 | [查看 2核2G 方案](https://t.co/j2RgxyPl9x) |
| 进阶 | 4核 / 4GB / 50GB | 6000GB | 2Gbps | $30/月 | $21/月 | [选 2Gbps 端口的中档](https://t.co/j2RgxyPl9x) |
| 高配 | 8核 / 8GB / 100GB | 10000GB | 2Gbps | $45/月 | $31.5/月 | [看 8核8G 双原生 IP 方案](https://t.co/j2RgxyPl9x) |

共同点是 IPv4 + IPv6 双原生 IP、国际线路非大陆优化、不提供 DDoS 防御；前两档只支持 Linux，后两档可选 Windows。超流量后的处理方式资料里没写明。

### 搬瓦工（参考位）

新加坡有两条线，性质完全不同。SG_8 是独立套餐，月付 $49.99 起，走 CN2 GIA-E。SG_1（CN2 GIA）不单独出售，得先买香港 CN2 GIA Ultra 套餐，再在 KiwiVM 里选 Migrate 迁移到 `SG: Singapore (CN2GIA) [SG_1]`，迁移免费、数据保留、IP 会更换，耗时几分钟到几十分钟。想直接下单 SG_1 的人会卡在这一步。

### LisaHost 丽萨主机（新加坡原生 IP，人民币计价）

| 套餐 | 配置 | 月流量 | 端口 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- |
| 基础版 | 1核 / 1GB / 10GB NVMe | 6000GB | 300Mbps | 68元/月（特价限售） | [看 68 元基础版是否还有货](https://lisahost.com/aff.php?gid=15&aff=1587) |
| 进阶版 | 2核 / 2GB / 20GB NVMe | 10000GB | 500Mbps | 88元/月 | [选 500Mbps 进阶版](https://lisahost.com/aff.php?gid=15&aff=1587) |
| 豪华版 | 4核 / 4GB / 40GB NVMe | 20000GB | 1000Mbps | 388元/月 | [查看 1Gbps 豪华版](https://lisahost.com/aff.php?gid=15&aff=1587) |
| 不限流量 Lite | 2核 / 2GB / 40GB NVMe | 不限 | 200Mbps | 398元/月 | [看 200Mbps 不限流量方案](https://lisahost.com/aff.php?gid=15&aff=1587) |
| 不限流量 Pro | 4核 / 4GB / 80GB NVMe | 不限 | 500Mbps | 898元/月 | [查看 500Mbps 不限流量方案](https://lisahost.com/aff.php?gid=15&aff=1587) |
| 特价年付版 | 1核 / 1GB / 10GB NVMe | 2000GB | 300Mbps | 466元/年（合每月约 38 元） | [入手 466 元/年特价档](https://lisahost.com/aff.php?gid=15&aff=1587) |

这套套餐最值得注意的不是价格，是流量给得大方：68 元配 6000GB，合每 GB 约一分一；388 元的豪华版直接给到 20TB 和 1Gbps 端口，每 TB 约 19 元。在同价位里，这个流量池很不常见。

## 按人群推荐

**个人博客、小站、轻量代理。** ByteVirt 标准版 VPS-4096-KVM-SG 月付 $5 给 2核4GB、2TB 流量、500Mbps 端口，跑 WordPress 和几个静态站绰绰有余，代价是 500Mbps 共享出口和超流量后的 1Mbps 限速。预算再紧一点，年付 $16.88 那档 512MB 也能撑起一个纯静态站。👉 [从 $5 月付这档开始试](https://bytevirt.com/aff.php?aff=1107&pid=48)

**跨境电商独立站。** 客户在东南亚、后台在国内，GoMami Mini 的 2核4GB 配 1TB 流量是这条需求里的稳妥选择，回程三网各自精品，晚高峰不至于掉到拨号水平。年付 8 折后约 $39.2/月，比月付省两成。👉 [选 Mini 年付，折合 $39.2/月](https://bit.ly/Gomami)

**TikTok、Shopee、店铺与广告账号运营。** 这一类要的不是带宽，是 IP 属性。LisaHost 官方写明默认分配新加坡原生 IP（测评资料里进一步称其为 ISP 住宅原生 IP），流媒体全解锁，支持 TikTok、ChatGPT、Shopee、Netflix，还送 5 个原生 IPv6。68 元起、48 小时可退，试错成本很低。👉 [查看 LisaHost 新加坡原生 IP 套餐](https://lisahost.com/aff.php?gid=15&aff=1587)

**API 服务、小程序后端。** 吃单核性能和响应稳定性，GoMami Air（4核8GB、2TB、1Gbps）或 ByteVirt Premium 的 VPS-2048（2核2GB、1.5TB、1Gbps、$15/月）都够用。前者贵在回程线路，后者贵在便宜。👉 [对比一下 ByteVirt 2048 Premium](https://bytevirt.com/aff.php?aff=1107&pid=40)

**跑量下载、中转、镜像。** 这个场景别看端口，看流量池和限速策略。ByteVirt 的 40TB 档 $66/月、100TB 档 $100/月，是全场每 TB 单价最低的两台，超流量后限 1Mbps 也不至于直接断网。👉 [看 100TB 跑量机型](https://bytevirt.com/aff.php?aff=1107&pid=53)

**要大陆晚高峰稳的企业站。** 走 CN2 GIA 这一类精品回程，GoMami 或搬瓦工的 CN2 GIA 系列都在这个范畴，代价是月付价在新加坡属于中高档。这类需求没有便宜解，只有贵得值不值。👉 [查看 GoMami 全系套餐](https://bit.ly/Gomami)

**纯国际业务、预算压到最低。** 荫云 7 折后 $7/月给 1Gbps、2TB、双原生 IP，是低价锚点。但它是国际线路、非大陆优化、无 DDoS 防御，别指望国内访问有多快。👉 [看荫云 7 折方案](https://t.co/j2RgxyPl9x)

## LisaHost 单独说：它卖的不是带宽

把 LisaHost 放进“大带宽”这个选题里其实有点错位。它的端口是 300Mbps 到 1Gbps，在今天的榜上不算突出；它真正值钱的是 IP。

官方产品描述里，这条线是新加坡 BGP 国际网络、默认分配新加坡原生 IP，TikTok 运营数据好、IP 纯净，支持装 Windows，还附送 5 个原生 IPv6。做账号矩阵的人都懂，IP 干不干净、是不是住宅段，比端口跑 300 还是 1000 影响大得多——账号被封一次，省下的那点月付钱全赔进去。

代价也写得很直白：**非中国大陆直连优化，建议通过香港或日本中转使用**。第三方测评的 traceroute 记录把这个短板量化得很清楚：广州电信回程绕经 Cogent 走马赛、巴黎、法兰克福，延迟 400ms 上下；上海电信更差，接近 500ms；联通经美国洛杉矶回国，230ms 左右；移动走香港 CMI，70ms 上下还能接受。这个数字不是商家的问题，是新加坡普通国际线路的共性——大陆方向没有优化，绕路是必然。

所以判断很简单：**如果你的核心诉求是国内访问快，它不该进你的候选名单**；如果你要的是一个干净的东南亚原生 IP 来跑账号、跑店铺、跑流媒体，顺带用香港或日本的中转节点把访问速度补回来，那它在 68 元这个价位上很难被替代。48 小时不满意无条件退款，够你把 IP 段和中转方案都验一遍。

品牌层面，LisaHost 是 2017 年成立的国人自营商家，总部在香港新界，全中文界面，支持支付宝付款，主要面向跨境电商、TikTok、流媒体解锁这类出海需求。对国内用户来说，付款和沟通都不设门槛。

## 限制与不适合的人

**ByteVirt 标准版超流量后限到 1Mbps。** 这个速度能刷文字、能跑 SSH，但别想再看视频。买之前先算清自己的月流量，尤其是拿它做中转或下载的。

**GoMami 出站超限限到 20KB/s，而且 Nano、Mini、Air 不能装 Windows。** 20KB/s 基本上等于停摆，一个月只能再挤 50GB 左右。入站流量不计费这点是加分项，但出站才是大多数业务的真实消耗。另外它的月付价在新加坡属于中高档，$29 起的 Nano 不是最便宜的入场券。

**荫云是国际线路，不提供 DDoS 防御。** 它的定位就是便宜大碗的国际流量，别拿它当国内优化机用，也别把暴露在攻击下的业务放上去。

**搬瓦工 SG_1 不能直接买。** 必须先持有香港 CN2 GIA Ultra 套餐再迁移，流程多一步，而且迁移会换 IP。

**LisaHost 不是大陆直连优化线路。** 电信方向 400ms 级别的延迟是硬伤，必须配中转。它解决的是 IP 属性问题，不解决速度问题。

**所有价格以下单页为准。** 本文列的是各家官方标价，促销、库存、限售名额随时会变，尤其 LisaHost 的基础版标注了特价限售。

如果你只想要“大陆低延迟 + 不想折腾”，直接去看 CN2 GIA 类产品的月付价，然后接受它比国际线路贵两到三倍这个事实。中间路线在新加坡这个节点上基本不存在。

## 优惠码与退款对照

| 商家 | 优惠码 | 内容 | 备注 |
| --- | --- | --- | --- |
| GoMami | `GOMAMI365` | 全系年付循环 8 折，续费同价 | 只有这个码值得记，续费不涨价是真优势 |
| ByteVirt | `4XCFWA2AC3` | 新购 20% off | 流传较广，优先试 |
| ByteVirt | `9YNBMBB805` | 全场 10% off | 新老用户可用 |
| ByteVirt | `WELCOME25` | 首购 25% off | 仅首次购买 |
| ByteVirt | `BV2026` | 年付 8 折 | 来源自述可用性待验证，别当确定项 |
| 荫云 | `gwvpsceping` | 永久 7 折 | 折后 $7 / $11.2 / $21 / $31.5 |
| 搬瓦工 | `BWHCGLUKKB` | 6.77% | 折扣力度一般 |

优惠码一律以下单页校验结果为准，填进去不生效就是失效了。

退款政策横向看，差距比价格差距更值得注意：

- **LisaHost：48 小时不满意无条件退款**，窗口最长，条款最干净。
- **GoMami：24 小时无条件退款**，但 24 小时内流量超 10GB 不退、遭 DDoS 攻击不退、欺诈滥用不退，退款要扣支付手续费，且退款后账号不能再申请第二次。
- **ByteVirt：有限退款范围**，需开工单确认，没有明确的无条件窗口。
- **荫云：资料中未说明退款政策**，下单前建议先问清楚。

对抱着“先买一台试试”心态的人，48 小时和 24 小时的区别不只是 24 小时——GoMami 那条“超 10GB 不退”意味着你没法拿它跑一轮完整的带宽测试再退。

## 常见问题

**1Gbps 实际能跑多少？**
理论峰值约 125MB/s。实际取决于共享比例、回程线路和对端。第三方测评里，GoMami 在晚高峰电信和移动方向基本能贴近标称值，联通偶有波动但多线程能拉满；ByteVirt Premium 标称 500Mbps 到 1Gbps，实测上下行接近 500Mbps。这些都是别人的测点和时段，你自己的结果可能不同。

**为什么晚高峰会掉速？**
国际出口在晚间拥塞。走 CN2、9929、CMIN2 这类精品回程的机器受影响小，走普通国际线路的机器受影响大。这也是为什么同一台机器白天测速好看，晚上八点后可能腰斩。

**原生 IP 和广播 IP 差在哪？**
原生 IP 的注册地和机房所在地一致，广播 IP 是把别处的 IP 段宣告到本地机房。差别体现在风控上：流媒体、电商平台、支付和账号系统会校验 IP 归属，广播 IP 更容易触发验证或被判异常。ByteVirt 新加坡的 IP 不是原生，但解锁能力尚可；LisaHost 和荫云都提供原生 IP，荫云还是 IPv4 + IPv6 双原生。

**流量跑完会停机还是限速？**
ByteVirt 标准版是限速到 1Mbps，不停机。GoMami 是出站超限限到 20KB/s，也不停机，但基本等于不可用。荫云和 LisaHost 的公开资料里没有写明超流量处理方式，买大流量套餐前建议先确认。

**能不能装 Windows？**
GoMami 的 Pro 和 Ultra 可以，Nano、Mini、Air 不行。荫云的 4核4GB 和 8核8GB 两档支持 Linux/Windows。LisaHost 官方描述明确写了支持安装 Windows。ByteVirt 资料里没有相关说明。

**支持支付宝吗？**
LisaHost 支持支付宝，全中文界面。ByteVirt 支持支付宝和云闪付。GoMami 的付款方式包含 Stripe Alipay。荫云资料里未提及。

## 三句话的决策路径

要国内访问快，就在 GoMami 和 CN2 GIA 类产品里挑，接受它的价格。要极致的流量单价，去 ByteVirt 的 40TB 和 100TB 档。要干净的东南亚原生 IP 跑账号，LisaHost 的 68 元基础版加一个香港或日本中转，是这套组合里成本最低的起点。

👉 [从 LisaHost 新加坡原生 IP 套餐开始，48 小时内不满意可以全额退](https://lisahost.com/aff.php?gid=15&aff=1587)
